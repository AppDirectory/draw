# EtherDraw on Sandstorm

This branch ports EtherDraw to Sandstorm. To use it:

1. Run `bin/installDeps.sh` once after cloning the repo. Note that in the main branch, this is done automatically by `run.sh`, but in the Sandstorm branch that line has been removed because it doesn't make sense inside the sandbox.
2. Run `bin/run.sh` once, let Etherpad start, and then ctrl+C it. This does some first-time setup, creating some necessary files. If you do not do this, you'll get `EROFS` errors when Etherpad tries to create these files inside the sandbox.
3. You may now run `spk dev` as described in the [Sandstorm porting guide](https://github.com/sandstorm-io/sandstorm/wiki/Porting-Guide).

# Original Etherpad README follows

------------------------------------------------------------------

![alt text](https://f.cloud.github.com/assets/220864/730169/feb98294-e24b-11e2-903d-b3cbc68f3a48.gif "Action Video")

## An intuitive collaborative drawing web based tool.
Collaborative real-time drawing, sketching & painting

Fast, light weight, easy to maintain.  Try the [demo] (http://draw.etherpad.org).

Demo
----
[Etherdraw Demo site](http://draw.etherpad.org)

Installation
------------
  1. Install Requirements. ``sudo apt-get update && sudo apt-get install libcairo2-dev libjpeg62-turbo-dev libpango1.0-dev libgif-dev build-essential g++``
  2. Install EtherDraw `` git clone git://github.com/JohnMcLear/draw.git ``
  3. Enter the EtherDraw folder `` cd draw ``
  4. Run EtherDraw `` bin/run.sh `` 
  5. Make a drawing!  Open your browser and visit `` http://127.0.0.1:9002 ``

Requirements
------------
 * [NodeJS] (http://nodejs.org/)
 * Lib Cairo
 * Lib Jpeg
 * Lib Gif

License
-------
Apache 2 License

Donations
---------
Donate to the [Etherpad Foundation] (http://etherpad.org/#links)
