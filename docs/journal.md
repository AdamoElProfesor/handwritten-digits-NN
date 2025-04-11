### Data to use 

10.04.2025

I need to figure out, where I'm getting the data from. There is the famous MNIST dataset, but I don't 
know if there are other options. I'm trying to find all my options, list them, and find the most 
suitable for me.

First let's try to list important infromation about the MNIST dataset : 

- images are 28x28 (784 total pixels)
- 60'000 images
- grayscale


There is the NIST Dataset, which is actually the original version, the MNIST is an extended version.

This dataset is a little more "raw" and has no preprocessing done. That means that MNIST already did 
the preprocessing job on the NIST dataset. It would be less of a harsh using the MNIST dataset.


There is the EMNIST dataset, but it is basically derived from the NIST dataset. Basically it is the 
same as MNSIT but with more data (280'000 images).


After some more research I concluded, that the MNIST database is really the mainstream dataset for 
handwritten digits. I'll not try to complicated things and I'm going to use it.

---

11.04.2025

Until now, I never realized why the webstie "http://yann.lecun.com/exdb/mnist/" always showed up empty.
Using web.archive.org I found out that the website shows up empty since Febuary 2025.

So with this url " https://web.archive.org/web/20250103144930/https://yann.lecun.com/exdb/mnist/" I can go back to 2025 in 
january and find all the data I need.


MINST dataset info : 

- 60'000 images for training
- 10'000 images for testing
- derived from NIST dataset (basically every digit have been recentered, and resized to the same size)
- no need of preprocessing the data (it is already done)
- images 28x28
- grayscale


Actually, I went back to 2023 to download the MNIST dataset files. It didn't work for 2025.

There are 4 files, and they are all binary files.

- Training set images
- Training set labels
- Testing set images
- Testing set labels

I wanna add that they add the error rate of methods that have been tested on the dataset.

For example on neuralnetowrks, with a lot of variants, they have at max an error rate of 4.7%, and a minimum of 0.35%.
The 4.7% error rate is with a 2-layer NN, 300hidden units, using mean square error as a loss function.

That just shows that my goal of 80% of accurracy is more than doable.

That makes the data research an end here.


