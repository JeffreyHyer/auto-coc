# Clash of Clans Bot
*Cooler name coming soon...?*

This is my Clash of Clans bot. Built to play Clash of Clans on the [BlueStacks](http://www.bluestacks.com/app-player.html)
Android emulator for Windows (built and tested on Windows 8). It is powered by
[SikuliX v1.0.1](http://www.sikuli.org/).

See below for setup and usage instructions



## Feature Overview
This bot is fully featured and is capable of amazing things when left to it's
own devices. This includes (but is not limited to):

* Donate troops to clan members
* Train troops, auto-balanced between all barracks
* Collect resources from Elixir Collectors, Gold Mines, and Dark Elixir Drills
* Accurately parse statistics from your village (Gold/Elixir/DE levels, Gems, etc.)
* Raid other villages according to configurable farming goals
	* Gold/Elixir/DE heavy emphasis
	* Balanced loot
	* Etc.
* Track raid statistics for later review and analysis
* Find and clear obstacles (trees, bushes, gem boxes, etc.)

## Initial Setup
To get setup you'll need:
* Bluestacks App Player
* A copy of SikuliX v1.0.1 (**NOT v1.1.0**) installed (either the IDE or the command line utility)
* A copy of the files in this repository

#### BlueStacks
Download and install the [BlueStacks App Player](http://www.bluestacks.com/app-player.html)

Once installed, open the player and install Clash of Clans. You'll need to set it up and link it to your account
so you can pick up where you left off on your phone/tablet or you'll need to start a new village.

#### SikuliX
* Download [SikuliX](https://launchpad.net/sikuli/sikulix/1.0.1/+download/sikuli-setup.jar) v1.0.1 (.jar file)
* Move the downloaded file (sikuli-setup.jar) to an empty folder
* Double-click the `sikuli-setup.jar` file to run the installer.
* Choose **Option 1** for the full IDE *-or-* **Option 4** for just the command-line utility (I recommend Option 1)

#### This repository
Download the files in this repository [here](https://github.com/JeffreyHyer/auto-coc/archive/master.zip) and extract
it wherever you want. Just keep in mind the folder name must end in `.sikuli`, for example `auto-coc.sikuli`. You'll also need to change the name of the python script from `attack-and-rebuild-troops.py` to the name of the folder, `auto-coc.py`.

## Usage
*Option 1* (Using the SikuliX IDE)
* Open the `auto-coc.sikuli` folder (or whatever you named it) in the SikuliX IDE and run it (Ctrl + R)

*Option 2* (Using the command line)
* Open your command prompt
* Execute the command `[Sikuli Base Dir]/runIDE -r [/path/to/auto-coc.sikuli] -s`

The easiest way to run/debug the script is through the IDE. You also have the added benefit of the IDE loading
and displaying all of the referenced images for you.

You may need to tweak the settings/reference images to match your base/setup. Sikuli is very sensitive in it's
matching algorithms so what works on my machine may not work on yours, just update the images to match your
BlueStacks/COC setup and you should be fine.

If you run into any problems please [submit an issue](https://github.com/JeffreyHyer/auto-coc/issues). If you get creative and fix it yourself or add some
new functionality to the original script please [submit a pull request](https://github.com/JeffreyHyer/auto-coc/pulls)



## Changelog
* v0.0.1a
	* Initial release.
	* Works well on my machine but untested on other machines/setups
* v0.0.2a
	* Better attack strategy (works on ~99% of bases)



## Roadmap
* Add support for dark troops
	* Donations
	* Training
* Fix support for minimum Dark Elixir when raiding
* Test on other base configurations
* Implement "game loop" and time tracking
