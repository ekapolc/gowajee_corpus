# Gowajee corpus
Thai smart home corpus with "Gowajee" hotword

## Corpus Description

The corpus was collected in the Automatic Speech Recognition class offered at Chulalongkorn University as a homework assignment. The corpus comprises of the recordings from the Spring 2017 and Spring 2018 course offerings. The students were asked to form a group of up to six people. Each group were asked to come up with an example smart home application. Each group will record the same set of sentences that they came up with. More specifically, the students were instructed to:

* Collect 101 utterances per person (same sentences for each group)
* The first utterance is "Gowajee". This is designated as the wakeword.
* The second utterance must start with "Gowajee" with an accompanying command
* 16k Hz, 16 bit depth, mono
* The students were encouraged to record with the provided uni-directional microphones. However, this is not enforced.
* They are no other specifications about the recording environment

For the full instructions used for the collection, see [here](https://github.com/ekapolc/ASR_course/tree/master/HW3)

## Benchmarks

We kept the recordings from one group of students aside as a dev set, and the rest of the groups as the training set. The language model was trained from the combined dev and training set (this is cheating, but this benchmark serves more as a pre-liminary evaluation). Using the voxforge recipe in Kaldi (up to the neural network model), we achieved around XX% WER. 

The training-dev split is included in the provided file.

## Directory structure

XX


## Version 0.9

There are XX utterances collected from XX speakers. XX are males, while XX are females. The total length of the corpus is XX hours. The vocabulary size is XX words with a total of XX words.

### Download

[Version 0.9](https://drive.google.com/file/d/1OjC5NCgYzgbZ5iEffc1ssWIVm8PWfDxX/view?usp=sharing)

## Citing

Please cite the following be sure to include the version number of the corpus

```
@techreport{gowajee,
     title = {{Gowajee Corpus}},
     author = {Ekapol Chuangsuwanich and Atiwong Suchato and Korrawe Karunratanakul and Burin Naowarat},
     year = {2018},
     institution = {Chulalongkorn University, Faculty of Engineering, Computer Engineering Department},
     month = {06},
     Date-Added = {2018-06-11},
     url = {https://github.com/ekapolc/gowajee_corpus}
     note = {Version 2018-1}
}
```

