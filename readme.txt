# from carla doc
apt-get install python3-pyqt5.qtsvg python3-rdflib pyqt5-dev-tools libmagic-dev liblo-dev libasound2-dev libpulse-dev libx11-dev libgtk2.0-dev libgtk-3-dev libqt4-dev qtbase5-dev libfluidsynth-dev

# needed too
apt-get install libsndfile1-dev libavcodec-dev libavformat-dev

# get the sources
git clone https://github.com/falkTX/Carla.git
cd Carla
git checkout v2.2.0

# patches required: cpu specific cc options for armhf or arm64
#patch -p1 < /compile/doc/carla/carla-armv7l.patch
#patch -p1 < /compile/doc/carla/carla-aarch64.patch

# to check
make features

# to build
make

# to install
make install

# tar
#tar cvzf /tmp/carla-2.2.0.armv7l.tar.gz /usr/local/lib/carla /usr/local/lib/pkgconfig/carla* /usr/local/lib/vst/carla.vst /usr/local/lib/lv2/carla.lv2 /usr/local/bin/carla* /usr/local/share/mime/packages/carla.xml /usr/local/share/carla /usr/local/share/applications/carla* /usr/local/share/icons/hicolor/*/apps/carla* /usr/local/include/carla
#tar cvzf /tmp/carla-2.2.0.aarch64.tar.gz /usr/local/lib/carla /usr/local/lib/pkgconfig/carla* /usr/local/lib/vst/carla.vst /usr/local/lib/lv2/carla.lv2 /usr/local/bin/carla* /usr/local/share/mime/packages/carla.xml /usr/local/share/carla /usr/local/share/applications/carla* /usr/local/share/icons/hicolor/*/apps/carla* /usr/local/include/carla
#tar cvzf /tmp/carla-2.2.0.x86_64.tar.gz /usr/local/lib/carla /usr/local/lib/pkgconfig/carla* /usr/local/lib/vst/carla.vst /usr/local/lib/lv2/carla.lv2 /usr/local/bin/carla* /usr/local/share/mime/packages/carla.xml /usr/local/share/carla /usr/local/share/applications/carla* /usr/local/share/icons/hicolor/*/apps/carla* /usr/local/include/carla

# running carla
it requires

apt-get install python3-pyqt5 python3-pyqt5.qtsvg liblo7 libfluidsynth1

to run
