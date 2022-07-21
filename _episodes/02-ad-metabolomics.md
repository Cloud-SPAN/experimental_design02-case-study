---
title: "AD metabolomics example"
teaching: 20
exercises: 10
questions:
- Replication - types and number
- Controls types of
objectives:
- understand the difference between biological and technical replication   
- important of controls
keypoints:
- "X,Y,Z are important and should be looked at when deigning experiments"

---


# Metabolomics data from anerobic digestion

The following experimental design is shown below. In this experiment metabolite samples were prepared from sewage sludge which has been taken from anaerobic digesters. Anaerobic digestion is the process of using microbes to break down organic material to generate biogas which can be used as a renewable energy source. The samples are prepared to use on a mass spectrometer, which will generate an abundance and the charge/mass ratio for each metabolite it detects. Generating this metabolomic data, or generating other datasets on mass spectrometers often requires liquid chromatography prior to the mass spectrometer, hence you may have heard proteomic/metabolomic data referred to as LCMS data (Liquid chromatography mass spectrometry). Due to the metabolites in this case, or digested proteins in proteomic data, being seperated through liquid chromatography first, we have additional experimental design concerns to consider compared to seqeuncing based experiments.


## Insert image here of a design

## Interbatch variation in mass spectrometry

There is greater interbatch variation with LCMS data and a higher level of background noise. This is partly due to all samples and the solvent having to be injected and passed through one chromatography column prior to ionisation. This increases the occurance of contamination between samples. To circumvent this, before samples are injected, the column is conditioned by using multiple rounds of QC/ control samples first, followed by multiple rounds of blanks. This can vary by machine, however for use on the Orbitrap mass spectrometer you would typically perform 15 injections of a QC, followed by 7 blanks, followed by additional QC injections prior to the first samples. This should try and minimise anything bound to the column from previous experiments. Over time there is drift that occurs, which can reduce the accuracy of the quantification. To reduce both the carryover contamination, and to reduce drift, QC samples are injected every 7 samples to allow for normalisation of peaks in the analysis downstream.

### QC sample pooling

There are several methods for quantifying peak intensity in mass spectrometry data. You can inject samples with metabolites of a known concentration and structure to normalise concentration of unknown peaks. Here we are mentioning pooled sample QCs.  These are literally a pool of all samples ran. These do not give you an identity, but they are used to normalise samples and can be used to reduce background noise and contaminants that may be in individual samples. Mass spectrometry is not inheritantly quantitive unless you have a calibration against a known quantity as mentioned above. There are different methods to do this, and labelling strategies. However we will not be covering these today. As with sequencing, we are typically more concerned with the relative abundance of metabolites.

### Randomisation of sample order

Randomisation in blocks is important. Complete randomisation can result in drift due to accidental severe imbalances in groups. 
