# m2i
Simple BASH script for converting a .mov video to an image sequence and extracting its audio (if any) to a .wav file within the same directory.

# What it does
It converts all .mov files in the current working directory to image sequences in a subdirectory, and demuxes audio for use in video editors and compositors which prefer image sequences to compressed video (such as Blackmagic Design's Fusion).

It depends heavily on ffmpeg and requires ffprobe
