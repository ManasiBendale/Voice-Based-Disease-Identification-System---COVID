# Voice-Based-Disease-Identification-System-COVID
**Project Introduction**

The analysis of the human voice has arisen as an important area of study for its various applications in medical as well as engineering sciences. Voice analysis basically deals with extraction of some parameters from voice signals for processing of voice in desirable applicability by using suitable techniques.

This project gives the importance to the voice signals given by the patients and by holding the characteristics of sound to detect the chances whether the patient has COVID-19 or not.

**Project Objective**

We address this problem by investigating the distinctness of path morphological alterations in the respiratory system induced by COVID-19 infection when compared to other respiratory infections. We propose to develop a solution for detecting the chances of COVID-19 infection using Machine Learning.

The results shown by this project can distinguish among COVID-19 coughs and the cough of a healthy person with an accuracy of 79 %. 

**Data Description**

This dataset has been taken from the Pfizer Digital Medicine Challenge.

Early detection of respiratory tract infections can lead to timely diagnosis and treatment, which can result in better outcomes and reduce the likelihood of severe complications.

Respiratory sounds carry rich information that can be mined to develop automated approaches for detection of sickness behaviors like coughing and sneezing.



**Model building**

For feature Extraction - MFCC, Filter Banks

How to find these Coefficients?
-> A signal goes through a pre-emphasis filter.
    Then gets sliced into (overlapping) frames
    A window function is applied to each frame
    Afterwards, we do a Fourier transform on each frame (or more specifically a Short-Time Fourier Transform)
    Calculate the power spectrum;
    And subsequently compute the filter banks.
    To obtain MFCCs, a Discrete Cosine Transform (DCT) is applied to the filter banks retaining a number of the resulting coefficients while the rest are discarded.
    A final step in both cases, is mean normalization.

Model used - RNN with LSTM
