# data

* `0-raw_data` stores all of the raw data of individual samples. One "sample" represents one position/location on a chicken leg model; each sample is saved in one subdirectory with various files. Multiple sites on several chicken legs were used. Each data sample was collected over 100 sampling iterations over 50 seconds of 0.5-second sampling intervals. Data is available in CSV file format or in HDF5 file format. Under HDF5 file format, the data keys include "osc" and "spec" for data collected from the oscilloscope and spectrometer, respectively. In CSV format, the filenames are appended by "osc_data" or "spectra_data" to indicate data collected from the oscillorscope or spectrometer, respectively. Both sources should have the same data.

* `1-aggregate_data` stores aggregated optical emission spectra (OES). This directory contains CSV files that have aggregated all of the OES from the raw data into a single file to be used for processing.

* `2-image_generation` contains the Lissajous figures generated from the raw data.

* `3-model_inputs` contains the full dataset after it has been processed into machine learning model input-output format.

* `tmp` stores model checkpoints when training the neural network.