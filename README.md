# gif-encoder

A simple Linux script to convert videos to GIFs.

## Introduction :point_up:

Having wanted to include moving pictures in my GitHub READMEs, I set out to look for a way to upload mp4 files. [This](http://stackoverflow.com/questions/4279611/how-to-embed-a-video-into-github-readme-md) discussion on StackOverflow told me I cannot put a video in GitHub markdown. But GitHub markdown accepts GIFs. [This](http://blog.pkh.me/p/21-high-quality-gif-with-ffmpeg.html) webpage highlighted how to make high quality GIFs from videos using [ffmpeg](https://ffmpeg.org/). So I decided to try my BASH scripting skills out. :smile:

## Version History :package:

**latest** 	[gifenc.sh v1.0.0](https://github.com/joshua-kairu/gif-encoder/releases/download/v1.0.0/gifenc.sh) 	Monday, June 6, 2016 

This repo tries its best to follow the [Semantic Versioning](http://semver.org/) guidelines.

## How To Use :wrench:

* :zero: Download the latest release.
* :one: In a terminal, change directories to where the ```gifenc.sh ``` file is. 
* :two: You can then the script can be run by writing:

```$ sudo sh gifenc.sh /path/to/video /path/to/GIF```

* :three: To make the script work like any other command line script,
    1. Make the script executable by writing: 
    `$ chmod +x gifenc`
 
    2. Open up `.bashrc` using your favorite text editor
    `$ nano ~/.bashrc`
    
    3. At the bottom of `.bashrc` write a line that looks like:
    `alias gifenc='/path/to/gifenc.sh'`
    
    4. Save changes.
    
    1. Make the terminal understand the changes by writing:
    `source ~/.bashrc`

## Abilities :muscle:

This script can:
* Convert a couple of video formats to corresponding GIFs. Video formats tested so far are *.mp4. (And the webpage above tried it out with *.mov)

## Limitations :worried:

This script has issues such as:
* It does not provide a ```--help``` argument for quick help.

## Possible Future Work :fast_forward:

```gifenc``` can be expanded to:
- [ ] Provide more help on the console.
- [x] Avoid having to use ```sudo``` every time. Solved on Monday, 09. January 2017.

## Other things :books:

Big thanks to the folks at the following sites for their nice tutorial. Wouldn't be the same without these.
* http://blog.pkh.me/
* http://askubuntu.com/questions/229589/how-to-make-a-file-e-g-a-sh-script-executable-so-it-can-be-run-from-termina

## License :lock_with_ink_pen:

This repository is licensed under the [GNU General Public License Version 3](http://www.gnu.org/licenses/gpl-3.0.en.html).
