# from carla doc
apt-get install python3-pyqt5.qtsvg python3-rdflib pyqt5-dev-tools libmagic-dev liblo-dev libasound2-dev libpulse-dev libx11-dev libgtk2.0-dev libgtk-3-dev libqt4-dev qtbase5-dev libfluidsynth-dev

# needed too
apt-get install libsndfile1-dev libavcodec-dev libavformat-dev

# patches required: cpu specific cc options for armhf or arm64

# to check
make features

# to build
make
