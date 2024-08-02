# Classification-Of-Viral-DNA

Greetings!

The purpose of this project was to implement efficient classification of nucleic acid sequences of Flaviviridae viruses for hypothetical improvement of standard methods for viral nucleic acid sequences analysis.

The data for the project was initially obtained from the National Center for Biotechnology Information (https://www.ncbi.nlm.nih.gov). In order to form a proper dataset for analysis I needed to come up with a preprocessing technique, that is implemented in the 'data_preprocessing.ipynb' file. The final dataset consists of genetic material of five Flaviviridae viruses: Yellow fever, Dengue, Zika, Japanese encephalitis, and West Nile. 5 files with sequences of every listed virus respectively can be found on my google drive (https://drive.google.com/drive/folders/1rBW6k3ZHD3jtW_QH0TWmsH_s5ZGX77Vq?usp=sharing).

I chose to explore CNN models for classification for several reasons:
- ability to detect local patterns and structures of the input data using sliding filters;
- efficient automatic feature selection in a complex dataset, which is fundamental for high accuracy of the model;
- unlike RNNs, convolutional networks are much less sensitive to the problem of the vanishing gradient on long sequences;
- ability to process different sections of the sequence in parallel thanks to the nature of convolutional layers.

I've attempted to implement 2 one-dimensional convolutional neural networks based on architectural principals of LeNet and VGG networks. I was able to reach classification results of good quality (97% accuracy) for both models through experimental studying of hyperparameters and architectural modifications. You can find all this in the "" file.

Enjoy exploring the project!

