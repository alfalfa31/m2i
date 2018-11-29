# m2i
Simple BASH script for converting a .mp4 video to an image sequence and extracting its audio (if any) to a .wav file within the same directory.

# Usage
1. Place the file in your $PATH and make it executable.
2. CD to a directory containing one or more MP4 files and type m21
3. 
4. Profit

# What it does
It converts all .mp4 files in the current working directory to image sequences in a subdirectory, and demuxes audio for use in video editors and compositors which prefer image sequences to compressed video (such as Blackmagic Design's Fusion).

It depends heavily on ffmpeg and requires ffprobe.

It would be pretty easy to extend it to whatever use case you can think of, for instance making it smarter on mime types.
