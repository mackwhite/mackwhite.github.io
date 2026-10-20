smallmouth-buffalo-drone.mp4 is the home page background video: a 32-second loop
cut from 0:24-0:57 of the April 6, 2019 drone flight, with the last second faded
into the first so the loop has no jump. 1280x720, no audio, about 11 MB.
smallmouth-buffalo-poster.jpg is its first frame, shown while the video loads.

To swap in a different clip, keep the same file names and keep it small:

  ffmpeg -i YOUR_CLIP.MP4 -ss START_SECONDS -t 30 -an -vf "scale=1280:-2,fps=30,format=yuv420p" -c:v libx264 -crf 28 -preset slow -movflags +faststart smallmouth-buffalo-drone.mp4

Then re-render the site (quarto render) and push.
