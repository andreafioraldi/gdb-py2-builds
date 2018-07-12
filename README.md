# gdb-py2-builds
GDB .deb pakages built with python2 support

## how to build

```
sudo apt install python2.7-dev python2.7
sudo apt build-dep gdb
sudo apt source gdb
cd gdb*
sed -i -E "s|python3|/usr/bin/python2.7|" debian/rules
dpkg-buildpackage -uc -us -j4
```
