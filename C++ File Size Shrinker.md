# C-File-Size-Shrinker
 - Shrinks the Sile Size of Videos, Gifs, and Images, without destroying Quality

you need one of these
ARM64: https://aka.ms/vc14/vc_redist.arm64.exe
x86: https://aka.ms/vc14/vc_redist.x86.exe
x64: https://aka.ms/vc14/vc_redist.x64.exe

--- HOW TO USE ---
Put your Videos or Images in the MEDIA folder
Run the File Size Shrinker file
When done, your exports are in the OUTPUT folder

--- JSON SETTINGS ---
The json is named "settings" and is in the ASSETS folder, this holds the ffmpeg speed preset, worker count, and crf value


Worker count can be changed in the settings json

Standard x264/x265 Presets:
 - ultrafast = Fastest encoding, lowest compression
 - superfast
 - veryfast
 - faster
 - fast
 - medium = Default
 - slow
 - slower
 - veryslow = Highest compression, slowest
 - placebo = Max compression, extremely slow, usually not practical

Notes:
 - Faster presets = less CPU usage, bigger files.
 - Slower presets = smaller files, higher CPU usage.
 - “Placebo” is mostly for testing; usually not worth the extra time.
 - Presets are not quality settings—they just affect compression efficiency. For quality, you use -crf with x264/x265.

CRF
 - crf is the quality that the frames are passed through ffmpeg
 - 12-16 is visually lossless
 - 1 is as low as it can go, 0 will corrupt the video
 - 51 is the highest it can go
 - lower number means more quality, higher number means less quality
