# Data Science Take Home Assignment
Data Science Take Home Assignments used in Sandvik CODE's recruitment process.

## Introduction

Welcome to Sandvik CODE's take-home assignment repository, part of our data science recruitment process. The following assignment will let you extract, explore and analyze audio data from English speaking male and females, and build learning models aimed to predict a given person's gender using vocal features, such as mean frequency, spectral entropy or mode frequency.

Contrary to most online communities that share datasets for data science, machine learning and artificial intelligence applications, readymade datasets rarely exist out in the wild, and you will have to explore one or more ways of downloading and extracting meaningful features from a raw dataset containing thousands of individual audio files. The assignment is designed to test your ability to tackle the full range of responsibilities you will have as a data scientist at Sandvik CODE.

## Dataset

The raw data consists of 62,440 audio samples of male and female speakers speaking in short English sentences. The raw data has been downsampled from 44.1kHz. Total size of the dataset is approximately 12.5 GB once it has been uncompressed. The file format is `.wav` with a sampling rate of 16kHz and a bit depth of 16-bit. The raw dataset can be found **[here][2]**.

We recommend that you follow a data pre-processing procedure along the following lines:

1. Automate the raw data download using web scraping techniques
2. Pre-process data using audio signal processing packages such as [WarbleR](https://cran.r-project.org/web/packages/warbleR/vignettes/warbleR_workflow.html), [TuneR](https://cran.r-project.org/web/packages/tuneR/index.html), [seewave](https://cran.r-project.org/web/packages/seewave/index.html) for R, or similar packages for other programming languages
3. Consider, in particular, the ([human vocal range][1]), which typically resides within the range of **0Hz-280Hz**
3. To help you on your way to identify potentially interesting features, consider the following (non-exhaustive) list:
  - Mean frequency (in kHz)
  - Standard deviation of frequency
  - Median frequency (in kHz)
  - First quantile (in kHz)
  - Third quantile (in kHz)
  - Inter-quantile range (in kHz)
  - Skewness
  - Kurtosis
  - Mode frequency
  - Peak frequency

  [1]: https://en.wikipedia.org/wiki/Voice_frequency#Fundamental_frequency
  [2]: http://www.repository.voxforge1.org/downloads/SpeechCorpus/Trunk/Audio/Main/16kHz_16bit/

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

A good presentation presents potential caveats, findings and insights about the dataset and an analysis of the goodness of fit metrics, including benchmarking on the performance of different learning models.

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
