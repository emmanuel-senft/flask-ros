Flask-Ros
=========

Web server to display video from a ros topic

Usage:
------
`roslaunch video_stream_opencv camera.launch video_stream_provider:=*x*'
`gunicorn --threads 5 --workers 1 --bind *your_ip*:8080 app:app'
- Replace *x* by the number of the video feed to open /dev/videox.
- Replace *your_ip* by the machine's ip.

Prerequisite:
-------------

Flask, Ros, Gunicorn

