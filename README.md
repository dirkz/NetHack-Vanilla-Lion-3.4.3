NetHack Vanilla 3.4.3 with patches for Lion

/* Copyright (c) Stichting Mathematisch Centrum, Amsterdam, 1985. */  
/* NetHack may be freely redistributed.  See [license] (iNetHack/blob/master/dat/license "License") for details. */  

Changes you have to make yourself:

sys/unix/Makefile.top:

    ...
    PREFIX	 = /Users/dirk/local # your own install directory
    ...
    GAMEUID  = dirk # your username

include/config.h:

    // This #define should reflect PREFIX/GAMEDIR from Makefile.top
    #define HACKDIR "/Users/dirk/local/games/lib/nethackdir"

After that it's the usual:

cd sys/unix
sh setup.sh bb
cd ../..
make
make install

Happy nethacking!

October 2011  
Dirk Zimmermann (me AT dirkz DOT com) [http://blog.dirkz.com] (http://blog.dirkz.com "http://blog.dirkz.com")
