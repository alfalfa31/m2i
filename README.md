# m2i
Simple BASH script for converting a .mp4 video to an image sequence and extracting its audio (if any) to a .wav file within the same directory.  It works on any Linux system with FFMPEG and FFPROBE installed (which is pretty much all default installs). 

# Usage
1. Place the file in your $PATH and make it executable.
2. CD to a directory containing one or more video files and type the command 'm2i'
3. 
4. Profit

# What it does
It converts all video files (of the following types: avi|mpg|mov|flv|wmv|asf|mpeg|m4v|divx|mp4|mkv|webm) in the current working directory to image sequences (up to 999,999 frames in length) in a subdirectory. It also demuxes audio for use in video editors and compositors which prefer image sequences to compressed video such as Blackmagic Design's Fusion, KDEnLive, DaVinci Resolve (which is still codec crippled on Linux).

It depends heavily on ffmpeg and requires ffprobe.

It would be pretty easy to extend it to whatever use case you can think of, for instance making it smarter on mime types.  Pay special attention to the source media's frame rate so that you can match the audio to the video in your editor.
