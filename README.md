# NetHack Vanilla 3.4.3 with patches for Lion

    /* Copyright (c) Stichting Mathematisch Centrum, Amsterdam, 1985. */  
    /* NetHack may be freely redistributed.  See [license] (iNetHack/blob/master/dat/license "License") for details. */  

By default, this install uses ~/NetHack as your installation directory.
This is pretty much a single-player-installation.

*If you'd prefer a multi-user installation you might want to change some
of the following:*

sys/unix/Makefile.top:

    ...
    PREFIX	 = ... # your own installation directory
    ...
    GAMEUID  = ... # installation username
    ...
    CHOWN = chown
    CHGRP = chgrp
    ...

*After that it's the usual:*

cd sys/unix  
sh setup.sh bb  
cd ../..  
make  
make install  

Happy nethacking!

October 2011  
Dirk Zimmermann (me AT dirkz DOT com) [http://blog.dirkz.com] (http://blog.dirkz.com "http://blog.dirkz.com")
