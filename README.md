# Cardiotocography Analysis

**Goals:** 

• Obtaining a cardiotocography analysis for infants to decide whether the baby is to be delivered through
caesarean section or assisted vaginal birth.

• Continually assessing a huge dataset of Cardiotocogram features to keep tabs on the health of the
fetus during labor.


**Introduction and Scope:**

The fetal heart rate fluctuations and their temporal correlation with uterine contractions are captured by cardiotocography (CTG). The goal of obtaining a cardiotocography analysis is to identify infants who may be anemic (hypoxic) in order to direct further evaluations of fetal welfare or decide whether the baby is to be delivered through caesarean section or assisted vaginal birth. A major problem today lies in assessing the efficiency and method of labor delivery and continuous cardiotocography acts as a technique for keeping tabs on the health of the fetus during labor.

Using clinical data that was routinely gathered in a large tertiary hospital, we investigated whether infants with "severe compromise" at delivery had fetal heart rate anomalies in their first hour CTGs and/or other clinical risks, recorded as per regular treatment. Intermittent auscultation for the intrapartum surveillance of low-risk pregnancies—defined as the absence of any prenatal or intrapartum, fetal, maternal, placental, medical, or obstetric problems or risk factors—was and is the current national recommendation. Obstetricians have long urged that CTGs be read objectively and automatically. A CTG diagnostic assistance system has undergone adequate improvement, but practical performance has not yet been fully attained. One explanation for this is that postnatal outcomes were not the focal point of earlier investigations, which instead concentrated on local wave patterns (extracted features considered to signify poor fetal status). Such aberrant CTG features that have been annotated by humans are not always consistent with harmful postnatal effects. Here, we will use various Machine Learning techniques to directly predict the perinatal outcomes of newborns from intrapartum CTG patterns.
The diagnostic features were measured and automatically processed from 2126 fetal cardiotocograms (CTGs). Three knowledgeable obstetricians classified the CTGs as well, and they each received a consensus categorization label. A, B, C, etc.) morphologic pattern and fetal condition were used to classify the samples (N, S, P). Therefore, the dataset can be applied to trials with 10 classes or 3 classes.


**Attribute Information:**

LB - FHR baseline (beats per minute)

AC - # of accelerations per second

FM - # of fetal movements per second

UC - # of uterine contractions per second

DL - # of light decelerations per second

DS - # of severe decelerations per second

DP - # of prolonged decelerations per second

ASTV - percentage of time with abnormal short term variability

MSTV - mean value of short term variability

ALTV - percentage of time with abnormal long term variability

MLTV - mean value of long term variability

Width - width of FHR histogram

Min - minimum of FHR histogram

Max - Maximum of FHR histogram

Nmax - # of histogram peaks

Nzeros - # of histogram zeros

Mode - histogram mode

Mean - histogram mean

Median - histogram median

Variance - histogram variance

Tendency - histogram tendency

CLASS - FHR pattern class code (1 to 10)

NSP - fetal state class code (N=normal; S=suspect; P=pathologic)

Data Cleaning and Exploratory Data Analysis are initially done on the raw dataset. A dataset named CTGDataCleaned.csv ( cardiotocographyanalysis/CTGDataCleaned.csv ) is the resultant dataset after cleaning and processing.
