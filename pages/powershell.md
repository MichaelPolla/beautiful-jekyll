# PowerShell

## References

Book "Learn Windows PowerShell in a Month of Lunches", 3rd edition, Donald W. Jones.

[The Scripting Guys blog](https://devblogs.microsoft.com/scripting/): lot of useful scripts

## First steps

### Help

PowerShell doesn't ship with included help.

Use `Update-Help`
PowerShell must be running under elevated privileges (Administrator).

`Save Help`: get a local copy, that can be used for other computers that may not have internet access.
`Update-Help -Source` to use it.

`Help` : wrapper functions that calls `Get-Help` producing a paged view (same as `Get-Help | More`).

`man` : alias for `Help`.

Note : in PowerShell ISE, help is always displayed all at once no matter the command used.

Finding commands example : `Help *log*`

`Help about*` : list all "about" topics. These are interesting information that are not related to a specific cmdlet.

Useful parameters : `-Full`, `-Examples`, `-Online`

`Get-Command *keyword*`  
alias: `Gcm`  
Example: `Gcm *Event*`

A better approach is to use the -Noun or -Verb parameters. Because only cmdlet
names have nouns and verbs, the results will be limited to cmdlets. Get-Command
-noun *event* returns a list of cmdlets dealing with events; Get-Command -verb
Get returns all cmdlets capable of retrieving things. You can also use the -Command-
Type parameter, specifying a type of cmdlet: Get-Command *log* -type cmdlet
shows a list of all cmdlets that include log in their names, and the list won’t include
any external applications or commands.

`CommandA | Get-Member`: list of all the available properties of an object produced by a command named *CommandA*.

## Providers

`Get-PSDrive`: list the available drives (env, registry, etc.)

`Set-Location` : same as `cd` command (`cd` is also an alias for it)
`Set-Location -Path C:\Windows`

`New-Item -Name MyFolder -ItemType Directory`: create a new directory MyFolder at the current location.

Navigate in the registry :
`Set-Location -Path hkcu:`

`HKCU:\software\microsoft\Windows> Set-ItemProperty -Path dwm -Name EnableAeroPeek -Value 0`


## Best Practices

- Prefer single quotes over double quotes

## Keyboard shortcuts

`Esc`: clear the command line

## Misc (to be reordered later)

`$PSVersionTable`: Get the PowerShell and related components versions.

PowerShell treats all comma-separated lists as arrays of values.

`Get-EventLog -LogName "Windows PowerShell" | ConvertTo-Html | Out-File pslog.htm`
`start pslog.htm`: open file (in browser)

### Comparing files

Remember to run the corresponding command (like Import-* or Get-Content) first on the files, before making any comparison.

`Compare-Object -ReferenceObject (Import-Clixml .\ref.xml) -DifferenceObject (Get-Process) -Property Name`

Two text files:  
`diff -ReferenceObject (Get-Content .\file1.txt) -DifferenceObject (Get-Content .\file2.txt)`

### Export logs

`Get-Eventlog -LogName security -newest 5 | export-csv events.csv`

### Manipulating processes

Kill all processes with a name beginning with "firef" (like firefox):
`Stop-Process -InputObject (Get-Process firef*)`

### Listing files and folders

[List files in folders and subfolders](https://devblogs.microsoft.com/scripting/list-files-in-folders-and-subfolders-with-powershell/)

## Modules

PowerShell automatically discovers and loads modules from the paths set.

`Get-Content Env:\PSModulePath`: see where PowerShell is looking for modules.

 `Get-Module *trouble* -ListAvailable`

PowerShell Gallery : https://www.powershellgallery.com/

Set up a repository : `Register-PSRepository`
`Find-Module`


## Profile scripts

Create a `WindowsPowerShell` folder in the Documents folder.
Create a new `profile.ps1` file.

