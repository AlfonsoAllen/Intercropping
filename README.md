# Intercropping
This repository contains the files and data used to prepare the manuscript entitled "Improving intercropping strategies for sustainable pest control in agriculture", by Alfonso Allen-Perkins and Ernesto Estrada (2018)

The codes are released under an opensource license: GNU General Public License v3.0 (see: https://choosealicense.com/licenses/gpl-3.0/). To run the codes, Python and Jupyter Notebook are needed. It is possible to install Python and Jupyter Notebook, using the Anaconda Distribution (see: http://jupyter.org/install).

The code perform the SIR (markovian) calculations using NetworkX 1.9 (see: https://networkx.github.io/). 

"Data_Generation_for_(Suppl_)FigX.ipynb" files produce "(Suppl_)FigX.xlsx" files that contain the data (100 random realizations) for preparing the rainplots in (Supplementary) figure "X" (see main text and Supplementary Information of our manuscript).

On the other hand, "Panels_for_(Suppl_)FigX.ipynb" files generate the figures for each arrangement in (Supplementary) figure "X" (see main text and Supplementary Information). To prepare the random intercrop panels, the "predefined_random_arrangement.txt" file is needed. 

"Calculations_for_SIR_thresholds_X.ipynb" files generate the data in "SIR_thresholds_Y.txt":  the average stationary fraction of dead susceptible plants, $R(\beta,\mu)$, for 50 logarithmically spaced values of $\beta$, between 0.02 and 1.0, when a given arrangement "Y" is used (under the conditions indicated in "X"), and $\mu=0.5$. Finally, "Figures for SIR epidemic thresholds and thresholds estimations.ipynb" file generates the main panels in Fig 0.6 and the corresponding threshold values. To run this file, "SIR_thresholds_mean_Y_X.txt" files  are needed. These files contain the the average stationary fraction of dead susceptible plants for 50 logarithmically spaced values of $\beta$, averaged over various realizations, when a given arrangement "Y" is used (under the conditions indicated in "X"), and they can be easily obtained from various "SIR_thresholds_Y.txt" files, using "Calculations_for_SIR_thresholds_X.ipynb".
