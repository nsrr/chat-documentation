# Dataset Introduction

The [CHAT dataset](:files_path:/datasets) posted on the NSRR has gone through various post-processing steps in order to prepare the data for more widespread sharing. The source data are from the CHAT Data Coordinating Center at the University of Pennsylvania. Changes and updates to the source data and have been coordinated in the [chat-data-dictionary repository](https://github.com/sleepepi/chat-data-dictionary).

**Disclaimer:** These data are not perfect. Known implausible or impossible values have been tracked and documented in our [KNOWNISSUES list](https://github.com/sleepepi/chat-data-dictionary/blob/master/KNOWNISSUES.md). Please [submit issues](https://github.com/sleepepi/chat-data-dictionary/issues) for any new problematic findings.

## Structure of the Dataset

The dataset is broken down into `baseline` and `followup` files, each of which contain 453 rows. Participants who withdrew or did not complete the protocol will have a greater prevalence of missing data in the `followup` file. Use [**nsrrid**](https://sleepdata.org/datasets/chat/variables/nsrrid), the CHAT subject identifier, to link datasets with [raw polysomnography data](:pages_path:/polysomnography-introduction.md).

*Note:* EDF/XML files are available for `nonrandomized` CHAT subjects (i.e. those who did not meet all eligibility criteria to be randomized). Covariate data for the `nonrandomized` group are also available.

If you have additional questions about the CHAT dataset, please contact <a href="mailto:support@sleepdata.org">support@sleepdata.org</a>.
