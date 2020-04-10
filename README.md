# py-behav-box
Python Behavioral Box
Installation

We use the following code in a batch file to open the GUI.

cd "PATH_TO_GUI"
python BEH_GUI_MAIN.py

GUI Image
Edit the Box for your project!

daqAPI.py correlates port numbers to input/output responses.
Protocols

See "all about protocols" file in PROTOCOLS folder.

Basic Overview:

[EXPERIMENT]

    set path and names

[SETUP]

    anything is setup is ran prior to the clock starting

[PROTOCOL]

    The experimental parameters, runs similar to a for loop

[Conditions]

    correlates an input from chamber to an output along with timing

Coding style overview

Two classes: GUI and Experiment

Gui holds GUI information and handles communication with behavioral box. Only to be updated if new GUI element needed to either show a new box input/output or if want to show new information.

Experiment handles running the testing. Should be changed to add new options in protocol.

Uses ZMQ to communicate with Open Ephys plugin-GUI. Need updated event broadcaster plugin from development branch (as of April 2019).
Info

This is being actively developed by the TNE-Lab at the University of Minnesota - Twin Cities.

Contact dasilvaf@umn.edu or schat107@umn.edu for more information
