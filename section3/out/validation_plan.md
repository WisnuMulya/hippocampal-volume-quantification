# Validation Plan: Hippocampal Volume Quantification Algorithm

## Intended Use
The intended use of this algorithm is for assisting the radiologist in the
quantification of hippocampus volume from T2 MRI image scans.

## Dataset Collection and Label
The training data is obtained from the hippocampus data of the Medical 
Decathlon Competition, which can be accessed here: [http://medicaldecathlon.com/](http://medicaldecathlon.com/).
The dataset contains 260 MRI images with label consisting of two regions: 
anterior and posterior. It is acquired from the Vanderbilt University Medical
Center, Nashville, US.

The hippocampus dataset was cropped by the team at [Udacity](https://www.udacity.com/)
to yield a subset consisting a small patch of the brain volume containing
the hippocampus.

## Performance
From 260 MRI volumes, 70% are used for training, whilst the rest 15% for
validation and another 15% for testing. The training yields the average 
result of 90.15% of [DICE score](https://en.wikipedia.org/wiki/Dice-S%C3%B8rensen_coefficient)
and 82.18% of [Jaccard index](https://en.wikipedia.org/wiki/Jaccard_index)
in the training dataset.

The real world performance would be estimated following the this average
result on the testing dataset.

## Limitation
The algorithm will perform well on MRI T2 scans that has similar resolution
to the one in the training dataset. Other than that, the algorithm may face
some limitation in its performance.
