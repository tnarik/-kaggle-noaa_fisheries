# Kaggle: NOAA Fisheries Steller Sea Lion Population Count

## Details

* URL: [https://www.kaggle.com/c/noaa-fisheries-steller-sea-lion-population-count](https://www.kaggle.com/c/noaa-fisheries-steller-sea-lion-population-count)
* Timeline/Deadlines (11:59 PM UTC):
  * Joining after the fact, but run for 3 months.

## Description

teller sea lions in the western Aleutian Islands have declined 94 percent in the last 30 years. The endangered western population, found in the North Pacific, are the focus of conservation efforts which require annual population counts. Specially trained scientists at NOAA Fisheries Alaska Fisheries Science Center conduct these surveys using airplanes and unoccupied aircraft systems to collect aerial images. Having accurate population estimates enables us to better understand factors that may be contributing to lack of recovery of Stellers in this area.

Currently, it takes biologists up to four months to count sea lions from the thousands of images NOAA Fisheries collects each year. Once individual counts are conducted, the tallies must be reconciled to confirm their reliability. The results of these counts are time-sensitive.

In this competition, Kagglers are invited to develop algorithms which accurately count the number of sea lions in aerial photographs. Automating the annual population count will free up critical resources allowing NOAA Fisheries to focus on ensuring we hear the sea lion’s roar for many years to come. Plus, advancements in computer vision applied to aerial population counts may also greatly benefit other endangered species.

## Evaluation

RMSE from the human-labelled ground truth, averaged over the columns.

The submission file should contain a header and have the following format:

```
test_id,adult_males,subadult_males,adult_females,juveniles,pups
0,1,1,1,1,1
1,1,1,1,1,1
2,1,1,1,1,1
...
```

### File descriptions

The file `KaggleNOAASeaLions.7z` is an encrypted 7-zip archive. An identical file is available via BitTorrent. 

The archive contains the following items:

* `sample_submission.csv`: an example valid submission file
* `Train/*.jpg`: a set of training images, with each filename corresponding to a train_id
* `Train/train.csv`: a list of ground-truth counts for each train_id
* `TrainDotted/*.jpg`: copies of the training images with markings showing where each animal is (see below)
* `Test/*.jpg`: a set of test images, with each filename corresponding to a test_id

**Note :** Some training images do not match their equivalents in TrainDotted. A list is posted in the `MismatchedTrainImages.txt` file.

`TrainSmall2.7z` is an archive containing the regular and dotted versions of training images 41 to 50, plus the sample submission file.

To assist you in locating individual sea lions, the TrainDotted folder contains the same images as in the Train folder, but with colored dots placed over the animals. The color scheme of the dots is:

* red: adult males
* magenta: subadult males
* brown: adult females
* blue: juveniles
* green: pups

## Benchmarks

Competition already finished. There were 385 teams and the best score (public/private) was 10.98446/10.85645.

With just 23.80683/22.65168 it would be enough to get a bronze medal.

There is an 'All Zeros Benchmark' with scores 29.08704/28.09320.

## Notes


## Structure
### Data

Data are not provided in this repo, please obtain them from the [competition data page](https://www.kaggle.com/c/noaa-fisheries-steller-sea-lion-population-count/data) and transfer them to the `data` subfolder.

### Code

This is a Python repository (at least initially). Requirements and additional information comes from an environment repo [https://github.com/tnarik/env-machine_learning](https://github.com/tnarik/env-machine_learning). It includes a `requirements.txt` file, which can be easily used with `Virtualenv` and `pip` to create a consistent working environment. Please use Python 3.

There are several folders:

* `develop` : this is for "lab notebooks". Consider them scratchpads. We will use a naming convention: `[start date]-[user]-[2_to_4_word_description].ipynb`. An example of this would be `20170320-tnarik-visualisation_exercise.ipynb`
* `deliver` : this is for final analysis or otherwise fully shareable notebooks.
* `src`? : for additional sources?
* `figures`? : for figures?
* `something_else`? : who knows?
