# CGflow2D-desktop-demo-version
CGflow2D is a command based 2D-Laminar Navier Stokes equations solver.  
CGﬂow2D desktop version  
Cartesian Grid ﬂow solver  
Desktop based Computational Fluid Dynamics simulation  

1 What’s this:  
CGﬂow2D v0.0 demo version is a free to use desktop based CFD
simulation executable. Unlike mobile app based CGﬂow2D there is
no GUI for desktop version instead it is fully command based. Once
you run the executable, it will automatically request for user inputs
that are required to run the simulation. Once the run completes
all the primitive quantities, inputs supplied and mesh ﬁle will be
written out as text ﬁle. Later these ﬁles can be used to view the
results in Gnuplot.

Since this is a demo version user can run ﬁve standard cases for now,
1D- Shocktube
2D- Cases:
1. Flowpast square
2. Pipeﬂow
3. Backward facing step
4. Lid driven cavity
5. Shocktube

2 Commands required for Gnuplot:
1. To view the Line plot for 1D case:
p ’ﬁlename.txt’ using 1:2 w lp lt 6 pt 7 ps 1.5
2. To view the 2d mesh:
plot ’ﬁlename.txt’ u 1:2:(0.2*($3)) w circles lc rgb ”red”
3. To view the contour plots:
splot ’ﬁlename.txt’ matrix with image

2.1 Setting views in Gnuplot:
In the Gnuplot terminal type the following:
set view 180,90,1.5
set size square

3 How to run the exe:
1. Double click exe, a command window will open and waiting for
user input.
2. Navigate to 2D Examples folder, open one of the cases and you
will ﬁnd a text ﬁle with name ”Input settings.txt”.
3. Use these input details and manually enter the values in the
command window one by one.
4. At the end of run the command window will automatically close
and dumps several text ﬁles. Later these ﬁles can be used to view
the simulation results using Gnuplot.  
![Alt text](https://github.com/ganeshkumar89/CGflow2D-desktop-demo-version/blob/master/2D%20Examples/Flowpast%20Square/MagVelocity.PNG?raw=true "Flowpast square")
![Alt text](https://github.com/ganeshkumar89/CGflow2D-desktop-demo-version/blob/master/2D%20Examples/Lid%20driven%20cavity/magvelocity.PNG?raw=true "Lid driven cavity")
![Alt text](https://github.com/ganeshkumar89/CGflow2D-desktop-demo-version/blob/master/2D%20Examples/Backward%20facing%20step/uvelocity.PNG?raw=true "Backward facing step")
![Alt text](https://github.com/ganeshkumar89/CGflow2D-desktop-demo-version/blob/master/2D%20Examples/Pipeflow/Magvelocity.PNG?raw=true "Pipeflow")
![Alt text](https://github.com/ganeshkumar89/CGflow2D-desktop-demo-version/blob/master/2D%20Examples/Shocktube/density.PNG?raw=true "Shocktube")
