 ============
 = Overview =
 ============

Here you will find the set of Python scripts I have written for use with the text, along with instructions for installation and a guide to usage. These scripts are used in the Workbook problems, they allow the reader to reproduce essentially all the calculations and figures in the text, and they provide a basic toolkit for original research. Before delving into this material, you should first take care of a basic Python installation and obtain some familiarity with the language

For an quick summary of what you need, see Quick Start. For experts, Quick Start may be sufficient. The material below covers the same territory in more detail. A tarfile of the complete collection of courseware is here. Eventually I will also provide access to a cvs repository on sourceforge or some similar server.

The most recent courseware update was July 11, 2011.

 ======================
 = Courseware Modules =
 ======================

These are utilities used throughout the courseware. They should be put in a search path where Python can find them regardless of which directory you are working from. See the Quick Start page for some notes on how to do that, or the Python portal page for a somewhat more extensive discussion of where Python looks for modules. These courseweare modules are not really meant to be modified by the student, but one can always make a personal copy and customize if desired. Wherever they are put, the student will be able to read them and see how they work. Freedom to Tinker Rules!

    ClimateUtilities.py : This is the universally needed handy collection of utilities used throughout the courseware. It provides support for reading and writing files, data manipulation, plotting, and numerical analysis.
    ClimateGraphics.py : This is imported by ClimateUtilities.py. It contains the actual plot functions, which in this version is set up to use PyNgl. If you are using a different graphics package to make plots, this is the only module you need to customize. MatPlotLib graphics is supported by the version below. See the Python Python Graphics page for details.
    ClimateGraphicsMPL.py : This version of ClimateGraphics uses MatPlotLib instead of PyNgl to produce graphics. It is imported automatically if PyNgl is not found on your system, and the rest of your scripts will work without any modifications. If you have both PyNgl and MatPlotLib on your system, but prefer to use MatPlotLib, just delete ClimateGraphics.py from your installation (or edit the import statement at the top of ClimateUtilities). See the Python Graphics page for details.
    DummyGraphics.py : This allows the Chapter scripts to be run without modification on systems for which no graphics implementation can be found.
    phys.py : Contains physical constants, properties of gases, and functions needed to compute physical properties (e.g. saturation vapor pressure or moist adiabats)
    planets.py : Contains characteristics of Solar System objects, including all planets and selected satellites. (the Sun isn't yet in there, but I will put it there eventually).