Clean up notebooks
check parameters for everything that's reported
split notebooks into thresholding, generating results, generating data

get everything into main branch as the most updated one
create one branch for paper submission
three files in the paper submission branch
software carpentry time!

check signal2noise and windowing

do unit and integration tests for all merges
double check with jonah and his thesis


WPT-cavitation repo

--- Main ---
- decide which notebooks to remove from repo
- removed unused and commented out code
- move all notebooks out of main into other repos
- move saved data and figures out of git

- test notebooks
- fix add_noise
- branch from main into 3 other branches (see below)
- main should contain all latest code that is shared by branches?

--- Public-release ---
- thoroughly tested, working code. 
- notebooks with example code. 
- keep example figures at root directory
* No .py files for saving data or notebook plotting code.

--- kmeans-paper --- 
* branch off main
* contains notebooks and .py files that generate results for notebook and files that plot and save data

--- Active cavitation detection --- 
* branch off main
* contains notebooks and .py files that generate acd simulation data.