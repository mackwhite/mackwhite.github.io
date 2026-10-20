Put the hero video here as: smallmouth-buffalo-drone.mp4

Keep it small so the page loads fast (aim for under ~15 MB, 1080p, 15-30 seconds, no audio).
If you have ffmpeg, this converts a raw drone clip:

  ffmpeg -i YOUR_CLIP.MOV -t 25 -an -vf "scale=1920:-2,fps=30" -c:v libx264 -crf 26 -preset slow -pix_fmt yuv420p -movflags +faststart smallmouth-buffalo-drone.mp4

Then re-render the site (quarto render) and push.
