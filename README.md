# gan_face_generation
Using Deep Convolutional GANs to generate new faces according [DC-GAN](https://arxiv.org/pdf/1511.06434.pdf) paper.

My aim with this project was to get some practice and experience with GANs 
in Tensorflow.

I started this project for an assignment for Udacity's excellent [Deep 
Learning Nanodegree](https://www.udacity.com/course/deep-learning-nanodegree--nd101),
 which I would highly recommend. After one epoch of training the GAN could 
 generate faces such as these:
 
<img src="https://user-images.githubusercontent.com/24551758/44003150-449e97fc-9e46-11e8-8b60-c41504b4669d.png" alt="drawing" width="200px"/>

# How to run
Once you have installed the packages in _requirements.txt_ then running the 
jupyter notebook should be self-explanatory.

# Downloading the data
- The `download_extract` function in `helper.py` downloads the MNIST dataset
from Yann Lecun's [website](http://yann.lecun.com/exdb/mnist/) and the faces
 dataset from a Udacity AWS server.  It extracts them and puts them in the 
 `/data` folder. From its URL the faces dataset appears to be the CelebA 
 dataset, which is available from it's [original site](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) or from this [Kaggle competition page](https://www.kaggle.com/jessicali9530/celeba-dataset).

# Ideas for improvements
- The Udacity coursework only allowed the GAN to run for one epoch on the 
faces dataset, and further running would certainly help performance.
- I would be interested to see whether transfer-learning the first 
convolutional layers of the discriminator would help, or whether that would 
make the discriminator too good too quickly, and so hinder the training of the 
generator.

# Acknowledgements
- The data and original code came from Udacity.  The idea with this 
coursework is that you fill in the gaps in the notebook.  All 
the helper functions are unchanged.
