# Managing Earthquakes Better with AI

### Introduction
As an engineer I have always been pasionate about using tehcnology to improve human lives. When I started my first formal Data Science course I decided to work on a capstone porject that can show how powerful AI is and how we can use it solve real world issues. 
Being a resident of British Columbia I know that British Columbia lies on biggest fault line in Canada and there is a constant threat of a major earthquake that can hit this piece of land anytime. This was where my motivation came from. I decided to work on a project which could detect early earthquakes and predict high pressure waves a little before time. More work can be done on this project to predcit earthquakes well before time and take all precautinary measures to minimize life and property losses.

### Dataset
I got access to open source data of 3-component siesmograms labelled as noise and earthquake from different parts of the world. 
Data can be found here:
https://zenodo.org/record/3648232#.YHTo3OhKhPY

                                              3-Component Earthquake Seismograms
![3-component EQ](https://user-images.githubusercontent.com/70457881/114481335-58c9f500-9bd2-11eb-9255-ae03f2bc186c.jpg)

                                              3-Component Noise Seismograms
![3-component noise](https://user-images.githubusercontent.com/70457881/114481702-194fd880-9bd3-11eb-8f86-0e6f44900a08.jpg)

### Data Preprocessing and Training 
The data was in from of numpy arrays. I plotted seismograms and concatenated all the 3 components and saved it as asingle jpeg image after removing all the irrelevant informaiton. After preprocessing images looked like this:
                                                 
                                                 3-component Siesmogram Image Indicating an Earthquake
![13](https://user-images.githubusercontent.com/70457881/114484849-edcfec80-9bd8-11eb-92fd-f42e3a5c878f.jpg)

These images were fed into a ResNet model and the model was trained to identify each image as noise or earthquake.

### Testing Accuracy
I tested the model for almost 1000 images and I got AUC = 96%

### Conclusion
This was my first independent Data Science project and I enjoyed working on it through out. It was a great learning eaxperience. We can further improve results by making accurate predictions well before time. This can be achieved by using LSTMs and RNNs. This model can also help us in understanding earth activity better which can help us in minimizing damage caused by earthquakes.











