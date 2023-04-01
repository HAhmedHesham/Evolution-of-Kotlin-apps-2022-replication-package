# ICT4S 2023 – Replication package

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7648592.svg)](https://doi.org/10.5281/zenodo.7648592)

This repository contains the replication package and dataset of the paper published at ICT4S 2023 with the title **Evolution of Kotlin Apps in terms of energy consumption: An Exploratory Study**.

This study has been designed, developed, and reported by the following investigators:

- Hesham Ahmed (Vrije Universiteit Amsterdam)
- Alina Boshchenko (Vrije Universiteit Amsterdam)
- Dmitriy Knyajev (Vrije Universiteit Amsterdam)
- Niaz Ali Khan (Vrije Universiteit Amsterdam)
- Dinara Garifollina (Vrije Universiteit Amsterdam)
- [Gian Luca Scoccia](https://gianlucascoccia.github.io/) (Università degli Studi dell'Aquila)
- [Matias Martinez](http://www.martinezmatias.com/) (Universitat Politècnica de Catalunya-BarcelonaTech)
- [Ivano Malavolta](https://www.ivanomalavolta.com) (Vrije Universiteit Amsterdam)

For any information, interested researchers can contact us by sending an email to any of the investigators listed above.
The full dataset including raw data, mining scripts, and analysis scripts produced during the study are available below.


### Overview of the replication package
---

This repository is structured as follows:


```
    /
    .
    |--- AndroidRunner/       		A copy of the source code of the Android Runner framework, which we used and customized for running our experiment.
    |--- Replication Package/           The folder containing all the Python source code we used for the experiment, its raw data, R analysis scripts, etc.

```


This replication package is structured as follows:


```
    /
    .
    |--- 01 Data/       	         Contains a list of 87 mobile apps that represents the initial pool of apps to choose from. Also, it contains the list after applying the inclusion and exclusion criteria. Finally, it contains the data that were collected after each trial of the experiment.
    |--- 02 Tests/                       Contains the tests(recorded keystrokes) that were used on each release of each application.
    |--- 03 Source code/                 Contains scripts for android-runner and the required android-runner config file.
    |--- 04 Figures/                     Contains the plots created after running the statistical tests.
    |--- 05 Analysis/                    Contains R scripts to perform statistical tests.

```

Each of the folders listed above are described in details in the remaining of this readme.

### 01 Data

```
    /
    .
    |--- Anki-Android/       	          The data the was collected after running each trial of the experiment for the application Anki-Android.
    |--- UHabit/                          The data the was collected after running each trial of the experiment for the application UHabit.
    |--- wifianalyzer/                    The data the was collected after running each trial of the experiment for the application Wifianalyzer.
    |--- List of apps - Subjects Selection.xlsx/       An xlsx file that contains the initial pool of apps after appying the exclusion and inclusion criteria.

```


### 02 Tests

```
    /
    .
    |--- Anki-Android/       	         Contains the tests that are associated with each release of the application Anki-Android.
    |--- UHabit/                         Contains the tests that are associated with each release of the application UHabit.
    |--- wifianalyzer/                   Contains the tests that are associated with each release of the application Wifianalyzer.
    

```

### 03 Source code
---
```
    / 
    .
    |--- config.json   				The configuration file of the Android Runner environment    
    |--- Scripts/ 
	    |--- after_experiment.py		The sequence of actions after the completion of the experiment
	    |--- after_launch.py		The sequence of actions after launching Android Runner
	    |--- after_run.py 			The sequence of actions after launching the application
	    |--- before_close.py		The sequence of actions before closing the application
	    |--- before_experiment.py 		The sequence of actions before running the experiment
	    |--- before_run.py			The sequence of actions before starting the application
	    |--- interaction.py			The sequence of actions while the application is running
```
The listed scripts can be copied to original Android Runner environment in order to repeat the experiment.


### 04 Figures
---
```
    	/
   	.
	|--- AnkiAndroid-analysisGraph.png
	|--- CL_AnkiAndroid.png
	|--- CL_Uhabits.png
	|--- CL_WifiAnalyzer.png
	|--- UHabit-analysisGraph.png
	|--- wifianalyzer-analysisGraph.png      
	|---Exploratory figures           
	│   |--- CodeReview/ 				Contains files for checking the number of lines of Kotlin code in each of the releases
	│   |--- Debug GPU overdraw/			Contains screenshots of GPU overdraws described in the article 
```
### 05 Analysis
---
```
    	/
    	.
	|--- analysis.Rmd				R script for generating analysis graphs

```

