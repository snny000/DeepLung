First download LIDC-IDRI dataset (https://wiki.cancerimagingarchive.net/display/Public/LIDC-IDRI) and check the data folder to prepare dataset 

Details:
For nodule classification, first clean the data from LIDC-IDRI. Use the ./data/extclsshpinfo.py to extract nodule labels. humanperformance.py is used to get the performance of doctors.
dimcls.py is used to get the classification based on diameter. nodclsgbt.py is used to get the performance based on GBM, nodule diameter and nodule pixel. pthumanperformance.py is used for patient-level diagnosis performance. kappatest.py is used for kappa value calculation in the paper.
For classification using DPN, use the code in main_nodcls.py. Use the testdet2cls.py to test the trained model. You may revise the code a little bit for different test settings.
