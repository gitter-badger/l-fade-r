# L Fade R

Real-time spatial audio filter with [Pure Data](http://puredata.info). 
Discover your favorite records in a whole new perspective. You can interactively fade between the __left__ and __right__ 
channels, and __L Fade R__ will mix the modified mix into a single __mono__ channel.

I created this simple audio tool for my [interactive YouTube guitar videos]() and also for practicing. I am a guitar 
player, and I like to practice my favorite songs while I listen to the music itself. With __L Fade R__ I am be able to 
filter out the main guitar parts from most of the records I listen to _without any quality loss_. The actual result depends on the mix.

<img src="https://raw.githubusercontent.com/tiborsimon/l-fade-r/master/docs/l-fade-r-gui.png" alt="L Fade R GUI" width=178 />

# Requirements

- [Pure data](http://puredata.info)
- Route your system audio into __Pure Data__

# Installing Pure Data

Excerpt from the official __Pure Data__ site:

>
Pure Data (aka Pd) is an open source visual programming language. Pd enables musicians, visual artists, performers, 
researchers, and developers to create software graphically, without writing lines of code. Pd is used to process and 
generate sound, video, 2D/3D graphics, and interface sensors, input devices, and MIDI.
>

You can install __Pure Data__ with the installers downloaded from it's official website. I have tested the currently 
(2015.04.01) available release (0.46.7) for Windows and OS X and they worked fine for me. I used the _vanilla_ release because it is a much smaller package than the feature packed _extended_ release.

Follow this link to download your copy of __Pure Data__: http://puredata.info/downloads

# Routing your system audio to Pure Data

To process your system sound with __Pure Data__, you need to route your system audio to it first. For this purpose I 
use [Virtual Cable]() on Windows and [Soundflower]() on OS X. There are alternative solutions also.

Download and install the latest __Soundflower__ release from GitHub: https://github.com/mattingalls/Soundflower

Download and install the latest __Virtual Cable__ from it's official website: http://vb-audio.pagesperso-orange.fr/Cable/

## Setting up Virtual Cable on Windows

After you installed __Virtula Cable__ on your machine, you have to go to the _Control Panel_ -> _Sound_ settings, and select _CABLE Input_ as your playback device. Then in Pure Data go to _Media_ -> _Audio Settings_ and choose _CABLE Output_ as the input. It is a good idea to turn off any sound enchancement as it can mix the left and right channels together, and you can't achieve a full left-right separation.

<img src="https://raw.githubusercontent.com/tiborsimon/l-fade-r/master/docs/win-settings-01.png" alt="L Fade R GUI" width=178 />
<img src="https://raw.githubusercontent.com/tiborsimon/l-fade-r/master/docs/win-settings-02.png" alt="L Fade R GUI" width=178 />
<img src="https://raw.githubusercontent.com/tiborsimon/l-fade-r/master/docs/win-settings-03.png" alt="L Fade R GUI" width=178 />

## Setting up Soundflower on OSX

After you installed __Soundflower__ on your machine, you have to go to the _System Preferences_ -> _Sound_ settings, and select _Soundflower (2ch)_ as your output. Then in Pure Data go to _Media_ -> _Audio Settings_ and choose _Soundflower (2ch)_ as your input.

<img src="https://raw.githubusercontent.com/tiborsimon/l-fade-r/master/docs/osx-settings-01.png" alt="L Fade R GUI" width=178 />
<img src="https://raw.githubusercontent.com/tiborsimon/l-fade-r/master/docs/osx-settings-02.png" alt="L Fade R GUI" width=178 />

# Contribute




