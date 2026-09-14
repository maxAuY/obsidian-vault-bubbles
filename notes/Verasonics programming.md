---- important ----
Find simulated intensity
Deal with numacq being changed. which processing funcs does it affect? (filterRF uses it)
make beamforming algorithm to bypass 4ppwl limit

----- testing ----
Test focal distance calculation
Test b mode for all scripts
Test centre portion imaging

---- ideas ---
Need to try different apodisation and tgc.
Calculate exactly how long rcv has to be?

---- qol / refactoring ----
Stop using evalin('base'). very hard to deal with expanding codebase
Add min range slider

Add option to show plots in main
Move ui stuff to main, add harmonics to main

Switch to amp mod or pulse inversion through gui
Save rfdata and save img should be different functions

Focus and xoffset in mm (and mb some other params)
Make display window fatter (img)

---- verasonics team notes ----
Receivelut
Set filter banks from symmetric to all pass
Trans.frequency to double transmit frequency
Simulated pressure field does not relate directly to actual pressure
4 points per wavelength is a limitation of the beamforming algorithm

--- 02 11 25 exp ---
Default tcg and IMG processing
49p3V, 32 focus 
6 to 12 no filter except for 0p25 nds