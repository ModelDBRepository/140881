This simulation was tested/developed on LINUX systems, but may run on Microsoft Windows or Mac OS.
To run, you will need the NEURON simulator (available at http://www.neuron.yale.edu)
Unzip the contents of the zip file to a new directory.
to compile & run:
 nrnivmodl *.mod
 nrngui mosinit.hoc -

Simulation will run for 1 s and spike output from excitatory cells of each column will be displayed. The spike
raster is arranged with y-axis as cell identifier and x-axis as time in milliseconds.
The y-axis is further arranged in order of layer/type, where each type is displayed
with a different color (black:layer 2/3, red:layer 4, green:layer 5a, blue:layer 5b).

Reference:
 This simulation is Figure 2 in
 Neocortical simulation for epilepsy surgery guidance: Localization and intervention,
 by William W. Lytton, Samuel A. Neymotin, Jason C. Wester, and Diego Contreras
 in Computational Surgery and Dual Training, Springer, 2011

Changelog
---------
202205: Updated MOD files to contain valid C++ and be compatible with the upcoming
        versions 8.2 and 9.0 of NEURON. Updated to use post ~2011 signature of
        mcell_ran4_init function.
