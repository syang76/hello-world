Assessment IRI EDP: Create a C-based modeling and simulation program that drive IRI model Fortran code. 
The code should capture and generate vertical EDP (Electron Density Profile) for a given time and location of interest.  

Makefile creates lib_iri.so for the fortran files.
"icc -c c_plot.c ; icc -o iri c_plot.o lib_iri.so" creates the executable iri.
EDP.png was generated by running iri.
fort.70 is the data file generated by running iri, which contains EDP values for the parameters specified in the c_plot.c
plot_script.gp is the gnuplot command script generated by c_plot.c
