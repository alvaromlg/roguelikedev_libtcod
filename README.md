# Compile libtcod

```
 sudo apt-get install mercurial autoconf libsdl2-2.0 libsdl2-dev libtool
 hg clone ssh://hg@bitbucket.org/libtcod/libtcod
 cd libtcod/build/autotools
 autoreconf -i
./configure
make
``` 

Once everything is compiled just copy these libraries to the project where you will use libtcod
```
cp -dr build/autotools/.libs/libtcod.so* python/libtcodpy data/fonts/arial10x10.png ~/project/
```

More info to how to install libtcod
http://www.roguebasin.com/index.php?title=Complete_Roguelike_Tutorial,_using_python%2Blibtcod,_part_1

# Run
```
python engine.py
```
