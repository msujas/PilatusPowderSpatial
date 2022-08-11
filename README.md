# PilatusPowderSpatial
Jupyter notebooks fitting Pilatus2m detector module geometry, edited from Jon Wright's notebook using an Eiger4m.
I've added an algorithm for finding gaps and generating the offset and module size variables. It also removes a 
lot of Eiger4m specific hard coding from the original so should be easier to use with other detectors.

Usage for those not familiar with ImageD11 (as I wasn't):
The module spatial peak search notebook generates .flt file. These are then read into ImageD11 to generate .par
detector calibration files. https://imaged11.readthedocs.io/en/latest/. I found the gui quite easy to use. It
should be located at <python dir>/Scripts/ImageD11_gui.py. Click Transformation>load filtered peaks, and the 
rest should be easy to figure out.