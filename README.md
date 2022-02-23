# Coffee-Leaves-Multi-Label-Classification Project

## Contents
<ul> 
  <li>Data</li>
  <li>Model</li>
  <li>Installation</li>
  <li>Results</li>
</ul>
 
## Data
The data consists of a total of 1747 images of coffee entire leaves, including healthy leaves and diseased leaves, affected by
one or more types of biotic stresses. The dataset contains the following stresses: leaf miner, rust, brown leaf spot and cercospora leaf spot. 
The images were labeled in relation to the predominant biotic stress of each leaf and its severity

<img src="sample images.PNG">

## Model
I have implementred a model consists of **VGG16** as feature extractor and on top of it there is **6 head consists of fully connected layers** 
which are used for the following :
- The **first** and the **second** heads are used to classify the severity and the predominant stress present in tha images
- The other **four** heads are used to classify the four stresses present in the images
So i have 6 output from the network as it is **Multi-Label Classification** 

## Installation
To pull the repository on your machine
```
git clone https://github.com/EhabIbrahim758/Coffee-Leaves-Multi-Label-Classification.git
```

if you need to download the trained model use this line
```
git lfs pull
```

You should have torch and torchvision

## Results
This table have all accuracy of the 6 heads 
<img src = "accuracy results.PNG" />


