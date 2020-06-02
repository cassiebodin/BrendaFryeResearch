# BrendaFryeResearch

### This repository will contain code and other research done for Dr. Brenda Frye's research group. *Jan 2019-May 2020*

"ClusterMembersG165" contains research on the galaxy cluster G165. My research focused on identifying additional cluster members to Dr. Frye's original list. Data that was originally used is in the Brenda_data file. All additional data that I added is found in Cassie_data
 * The first set of members were identified by creating a range of radial velocities based on the determined redshift of the cluster, 0.35. Data outside this range was elliminated. The data set was recorded in G165_combo_Frye_Cass.txt.
 * In order to filter this data I created a histogram of the redshifts of the data in G165_combo_Frye_Cass.txt, see G165_HistogramCM_2019-2020.ipynb. More data was eliminated based on the shape of the histogram (first histogram) and was recorded in the file G165_zrange_342_355.txt.
 * From this reduced data I replotted a second histogram (second histogram on G165_HistogramCM_2019-2020.ipynb), and calculated the mean and standard deviation of the data. I plotted the mean and (+ and -) 3 times the standard deviation, or 3 sigma, on the histogram. Further data was eliminated if it lay outside + and - 3 sigma, the results were recorded in G165_zrange_3sig.txt.
 * All data was organized and recorded in the excel files G165_alldata_colorcoat.xlsx and G165_upperlowerdata_colorcoat.xlsx
    * G165_alldata_colorcoat.xlsx contains all the data colorcoded to match the ds9 files containing all of the data
    * G165_upperlowerdata_colorcoat.xlsx contains the data in 3 sigma split up between + and - 3 sigma that matches the ds9 files
        * note : ds9 files not in this repository because the files exceed the size limit
 * Used data from G165_zrange_3sig.txt to calculate the Velocity Dispersion and subsequently the Dynamical Mass in the code DynamicalMassProgram.ipynb.
    * Some more data points were eliminated based on the calculated velocity dispersion.
 
"QuasarIdentification" contains research done on identifying quasars around previously identified protoclusters.  In comparison to a protocluster, quasars emit a lot of light radiation. So, in order to study protoclusters spectroscopically, quasars in the nearby regions must be identified and their light pollution subtracted.
 * I worked on identifying these quasars using SDSS.  Any quasar I found that was within 2 arcsec from one of our target protocluster, I took note of and gathered data for location (RA, dec), the redshift, and the spectra. 
     * Each file contains quasar data around a different protocluster, the file names are the protocluster names. 
 * I then wrote some code which plotted the spectrum for each quasar and identified key molecular markers in each of the spectra, specifically for Lyman Alpha, Carbon IV, and Magnesium II.
