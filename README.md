# R-GAMM-LabPhon18

This includes a step by step tutorial analyses of ultrasound tongue imaging data presented for the workshop [New Developments in Speech Sensing and Imaging](http://labphon16.labphon.org/se-04.html) held in Lisbon as a Satellite wrkshop to LabPhon 18. The code for the tutorial is [available here](https://jalalal-tamimi.github.io/R-GAMM-LabPhon18/GAMMsLabPhon.nb.html). 

10/08/2022: This [notebook](https://jalalal-tamimi.github.io/R-GAMM-LabPhon18/GAMMsLabPhon2022.nb.html) is now updated to include the two datasets used for the [demo linear vs GAMs](https://github.com/JalalAl-Tamimi/R-GAMM-LabPhon18/blob/master/dataProd_duud.csv) and then the [actual dataset for running GAMs](https://github.com/JalalAl-Tamimi/R-GAMM-LabPhon18/blob/master/resultsFull.c_NoRelNoz.csv). A couple of updates to the code are added as well, including: 

1. Declaring parallel computing to speed up computation; note that this does not seem to affect the processing time for the ML model, which will heavily depend on the size of your model.
2. Hard coding interaction term. the consonant:vowel interaction does not work anymore; using interaction(consonant, vowel) instead
3. Added gam.check to evaluate the k number (knots). 
4. Added system information for packages used.

Unfortunately, the gganimate function is not working as it should be; the previous animation on the original notebook is not working anymore. 
The whole notebook ran in around 5 hours using 10 CPUs. We gratefully acknowledge support from the CNRS/TGIR HUMA-NUM and IN2P3 Computing Center (Lyon - France) for providing computing and data-processing resources needed for this work


