# Data Science Take Home Assignment
Data Science Take Home Assignments used in Sandvik CODE's recruitment process.

## HUGO: Introduction

Welcome to Sandvik CODE's take-home assignment repository, part of our data science recruitment process. The following assignment will let you extract, explore and analyze audio data from English speaking male and females, and build learning models aimed to predict a given person's gender using vocal features, such as mean frequency, spectral entropy or mode frequency.

Contrary to most online communities that share data sets for data science, machine learning and artificial intelligence applications, readymade datasets rarely exist out in the wild, and you will have to explore one or more ways of downloading and extracting meaningful features from a raw data set containing thousands of individual audio files. The assignment is designed to test your ability to tackle the full range of responsibilities you will have as a data scientist at Sandvik CODE.

## VANJA: Dataset

This dataset is used to identify a voice as male or female, based upon certain properties of voice and speech. The dataset consists of 62,440 recorded voice samples, collected from male and female speakers. 

### Overview
Total size of the dataset is approximately 12.5 GB once uncompressed. File format is .wav, sampling rate 16kHz and bitrate 16-bit.

### Source URL
The dataset can be found here:
http://www.repository.voxforge1.org/downloads/SpeechCorpus/Trunk/Audio/Main/16kHz_16bit/

### Data
Feel free to utilize any programming language, tool, method or skillset to solve the challenge to the best of your abilities. However, we do recommend taking the following steps:
1. Use scraping techniques to obtain data from dataset URL, make sure to explore it in detail 
2. Pre-process data using R packages, such as WarbleR, TuneR, seewave or equivalent
-- Consider analyzing a particularly important frequency range of **0Hz-280Hz** ([human vocal range][1])
3. Determine potentially interesting features, such as:
  - **meanfreq**: mean frequency (in kHz)
  - **sd**: standard deviation of frequency
  - **median**: median frequency (in kHz)
  - **Q25**: first quantile (in kHz)
  - **Q75**: third quantile (in kHz)
  - **IQR**: interquantile range (in kHz)
  - **skew**: skewness (see note in specprop description)
  - **kurt**: kurtosis (see note in specprop description)
  - **mode**: mode frequency
  - **peakf**: peak frequency (frequency with highest energy)

  [1]: https://en.wikipedia.org/wiki/Voice_frequency#Fundamental_frequency


## Question Set

The following are reference points that should be taken into account in the submission. Please use them to guide the reasoning behind the feature extraction, exploration, analysis and model building, rather than answer them point blank.

1. How did you go about extracting features from the raw data?
2. Which features do you believe contain relevant information?
  1. How did you decide which features matter most?
  2. Do any features contain similar information content?
  3. Are there any insights about the features that you didn't expect? If so, what are they?
  4. Are there any other (potential) issues with the features you've chosen? If so, what are they?
3. Which goodness of fit metrics have you chosen, and what do they tell you about the model(s) performance?
  1. Which model performs best?
  2. How would you decide between using a more sophisticated model versus a less complicated one?
4. What kind of benefits do you think your model(s) could have as part of a enterprise application or service?

## Submission

### Deadline

You have **7 days** to complete the assignment from the time that you have received the email containing the link to this GitHub repository.

> **Note:** Your submission will be judged with this timeframe in mind, and that we do not expect the equivalent of a month's worth of work.

### Requirements

A 3 to 5 page presentation, in **HTML or PDF format**, that clearly and succinctly walks us through your approach to extracting features, exploring them, uncovering any potential constraints or issues with the data in its provided form, your choice of predictive models and your analysis of the models' performance.

A good presentation presents potential caveats, findings and insights about the data set and an analysis of the goodness of fit metrics, including benchmarking on the performance of different learning models.

A great presentation tells a visual, potentially even interactive, story about the data and how specific insights can be used to guide our product development so that non-technical colleagues can understand and act upon them.

## Code of Conduct

At Sandvik CODE, we give the people we hire a high level of autonomy in how they want to work, and value personal integrity highly. This autonomy only works if we can trust our colleagues to be honest about the work they are responsible for and the results they achieve. We trust that you do not collaborate with other people as part of this assignment, nor that you make use of readymade machine learning models without being able to properly argue for why they are applicable. The same goes for your choice of features and understanding of what type of information they provide.

If we realize, at any point during the recruitment process or following a successful hiring, that you have broken the trust we now place in you, we will terminate your application or employment immediately.

By accepting this take-home assignment, you are actively choosing to abide to this code of conduct.

## Frequently Asked Questions

1. **Can I use <Insert SDK or Framework here> for the take home assignment?**
  > **Answer:** Yes, you are free to make use of the tools that you are most comfortable working with. We work with a mix of frameworks, and try to use the one best fit for the task at hand.
2. **Where do I send my assignment upon completion?**
  > **Answer:** You should have received an email with instructions about this take home assignment that led you to this repo. If you have been invited to the take home assignment, but haven't received an email, please email us at *digitaljobs[at]sandvik.com*.
