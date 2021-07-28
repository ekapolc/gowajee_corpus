# Gowajee corpus
Thai smart home corpus with "Gowajee" hotword

## Corpus Description

The corpus was collected in the Automatic Speech Recognition class offered at Chulalongkorn University as a homework assignment. The corpus comprises of the recordings from the Spring 2017-2021 course offerings. The students were asked to form a group of up to six people. Each group were asked to come up with an example smart home application. Each group will record the same set of sentences that they came up with. More specifically, the students were instructed to:

* Collect 101 utterances per person (same sentences for each group)
* The first utterance is "Gowajee". This is designated as the wakeword.
* The second utterance must start with "Gowajee" with an accompanying command
* 16k Hz, 16 bit depth, mono
* In the first two years (2017-2018) the students were encouraged to record with the provided uni-directional microphones. However, this is not enforced. For the latter years, the students were encouraged to record using the hardware they wish to demo on.
* They are no other specifications about the recording environment

For the full instructions used for the collection, see [here](https://github.com/ekapolc/ASR_course/tree/master/HW3)

## Benchmarks

Using the voxforge training script, tri3b (speaker dependent) got 14.91% on the dev set and 8.82% on the test set.

## Directory structure

dataset
* audios
    * 2017 
    * 2018
    * 2019
    * 2020
    * 2021
* dev
    * spk2utt
    * text
    * utt2spk
    * wav.scp
* lu
    * spk2utt
    * text
    * utt2spk
    * wav.scp
* train
    * spk2utt
    * text
    * utt2spk
    * wav.scp
* test
    * spk2utt
    * text
    * utt2spk
    * wav.scp

We kept the recordings from three groups of students aside as a dev set, two group for the test set, and the rest of the groups as the training set.

The train/dev/test set splits is included in the provided file.

## Version 0.9.2

There are 17597 utterances collected from 166 speakers. 142 are males, while 24 are females. The total length of the corpus is 14 hours and 40 minutes. The vocabulary size is 2129 words with a total of 98253 words.

One group recorded "ภาษาลู", a teenage slang version of Thai. This is separated into its own set.

### Download

[Version 0.9.2](https://drive.google.com/file/d/1cN-pDwBVrguhHE6uEh4v6xLOa6qSjaWA/view?usp=sharing)

## Citing

Please cite the following be sure to include the version number of the corpus

```
@techreport{gowajee,
     title = {{Gowajee Corpus}},
     author = {Ekapol Chuangsuwanich and Atiwong Suchato and Korrawe Karunratanakul and Burin Naowarat and Chompakorn CChaichot
and Penpicha Sangsa-nga and Thunyathon Anutarases and Nitchakran Chaipojjana},
     year = {2020},
     institution = {Chulalongkorn University, Faculty of Engineering, Computer Engineering Department},
     month = {12},
     Date-Added = {2021-07-20},
     url = {https://github.com/ekapolc/gowajee_corpus}
     note = {Version 0.9.2}
}
```

