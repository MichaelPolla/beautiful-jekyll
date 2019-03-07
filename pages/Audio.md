<!-- markdownlint-disable MD028 -->

# Audio

## Definitions & Documentation

### Decibels

["What is 0 dB in digital audio ?"](https://sound.stackexchange.com/a/25533/23406) : detailled answer on sound.SE, with historical references. Talks about the different Decibels systems (dBm, **dBFS**...).

[dBFS - Decibels relative to full scale](https://en.wikipedia.org/wiki/DBFS)

> dBFS is a unit of measurement for amplitude levels in digital systems which have a defined maximum peak level.
> **The level of 0 dBFS is assigned to the maximum possible digital level**.

### Root Mean Square (RMS)

[Root Mean Square (RMS) in Audio](https://www.audiorecording.me/understanding-what-does-rms-stands-for-in-audio-definition-details.html) : nice article explaining the RMS value in digital audio. FAQ at the end.

>The easiest way to understand RMS is simply it’s just an unique way of finding out the **“average”**.

> Like any properties of a continuous signal such as audio or electrical signals. It can be characterized as having a maximum, minimum and average. In audio waveforms, these maximum is often called “peak” signal and often measured in dB in digital. In digital audio, the maximum allowable is 0dB. If it exceeds that amount, distortion would occur.

> Between the minimum (the quietest sections of the audio) and the loudest section (towards 0dBFS, the peak) is where the RMS value can be found.

> Human ears cannot detect exactly where the peaks and nulls occur in the waveform but we can say how loud or soft the music is. This is why **RMS is the most often used measurement in perceived loudness**. As RMS value gets closer to 0dB (maximum), the perceived loudness would also be getting louder.

## Tools

[Audiocheck.net](http://www.audiocheck.net/index.php) : lot of tools to test audio devices and to generate test sounds.