## Data
The dataset contains imperfections - images of flowers in odd places, or as a backdrop to modern machinery.
The task is to build a classifier than can see past all that, to the flowers at the heart of the images and classfiy them into the categories accurately.


This competition provides its files in TFRecord format. The TFRecord format is a container format frequently used in Tensorflow to group and shard data data files for optimal training performace. Each file contains the id, label (the class of the sample, for training data) and img (the actual pixels in array form) information for many images.

* train/*.tfrec - training samples, including labels.
* val/*.tfrec - pre-split training samples w/ labels intended to help with checking your model's performance on TPU. The split was stratified across labels.
* test/*.tfrec - samples without labels - you'll be predicting what classes of flowers these fall into.
* sample_submission.csv - a sample submission file in the correct format
* id - a unique ID for each sample.
* label - (in training data) the class of flower represented by the sample
