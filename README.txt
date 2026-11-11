Faable deployment package for the Rose project (performance-adjusted)

Upload these files to the root of the Faable project:
main.py, requirements.txt, Procfile.

The app uses one MJPEG stream instead of repeatedly requesting PNG frames.
This avoids overlapping render requests and limits rendering to 4 frames/sec.
The original rose geometry, palette, animation and signature are retained.
