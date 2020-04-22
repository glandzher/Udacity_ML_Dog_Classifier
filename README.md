[//]: # (Image References)

[image1]: ./images/sample_dog_output.png "Sample Output"
[image2]: ./images/vgg16_model.png "VGG-16 Model Layers"
[image3]: ./images/vgg16_model_draw.png "VGG16 Model Figure"


## Project Overview

Welcome to the Convolutional Neural Networks (CNN) project in the AI Nanodegree! In this project, you will learn how to build a pipeline that can be used within a web or mobile app to process real-world, user-supplied images.  Given an image of a dog, your algorithm will identify an estimate of the canine’s breed.  If supplied an image of a human, the code will identify the resembling dog breed.  

![Sample Output][image1]

Along with exploring state-of-the-art CNN models for classification and localization, you will make important design decisions about the user experience for your app.  Our goal is that by completing this lab, you understand the challenges involved in piecing together a series of models designed to perform various tasks in a data processing pipeline.  Each model has its strengths and weaknesses, and engineering a real-world application often involves solving many problems without a perfect answer.  Your imperfect solution will nonetheless create a fun user experience!

## Problem Statement
How many dog breeds could you recognize? 5? 10? Maybe you are a dog lover and can go up to 50! You may not realize it, but this is what I would call domain knowledge, or specialized knowledge. This type of knowledge is not common knowledge and most people can live a happy life without ever being able to identify 50+ breeds of dogs, or flowers, or <insert animal/electronic component/car model/…>. 
You may one day be in need to identify a dog’s breed though. Maybe it’s down to a disagreement with a friend on identifying the breed of the dog you are looking at. Or maybe you are living in May 2020 and are struggling to find food due to Covid-19 and are wondering if the beautiful wild mushroom you are looking at is safe to eat? Yeah, maybe stay away from that mushroom anyway.
Let’s think about how you might want to solve this problem if it’s a disagreement with a friend: you might have a few species in mind and therefore head for Wikipedia/Google image to get more information about that breed and check if it is or not the one you think it is. You see a bunch of images, some correlating your point, some others are not about the dog you are looking for (“Manchester terrier” was bound to give you some hits about the city in the UK). You decide that some description of the breed might help, exactly where Wikipedia comes into play. 15 minutes later and you are no closer to the answer, and most likely your friend has done the same thing and has counter arguments to the new ones you may have.
What if, through an app, you could take a photo or two of the dog in question and were given the breed back within a few seconds? Great user interface, simple, easy. A great product.
This kind of product is the type that can be developed using Convolutional Neural Network as they are very good at gathering specialized knowledge and could answer these specialized questions. 
 This is what we are going to work on in this project: firstly, differentiating humans from dogs, and, if the picture is of a dog, try to identify the breed itself.



## Project Instructions

### Instructions

1. Clone the repository and navigate to the downloaded folder.
	
	```	
		git clone https://github.com/udacity/deep-learning-v2-pytorch.git
		cd deep-learning-v2-pytorch/project-dog-classification
	```
    
__NOTE:__ if you are using the Udacity workspace, you *DO NOT* need to re-download the datasets in steps 2 and 3 - they can be found in the `/data` folder as noted within the workspace Jupyter notebook.

2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/dogImages`.  The `dogImages/` folder should contain 133 folders, each corresponding to a different dog breed.
3. Download the [human dataset](http://vis-www.cs.umass.edu/lfw/lfw.tgz).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 
4. Make sure you have already installed the necessary Python packages according to the README in the program repository.
5. Open a terminal window and navigate to the project folder. Open the notebook and follow the instructions.
	
	```
		jupyter notebook dog_app.ipynb
	```

__NOTE:__ While some code has already been implemented to get you started, you will need to implement additional functionality to successfully answer all of the questions included in the notebook. __Unless requested, do not modify code that has already been included.__

__NOTE:__ In the notebook, you will need to train CNNs in PyTorch.  If your CNN is taking too long to train, feel free to pursue one of the options under the section __Accelerating the Training Process__ below.



## (Optionally) Accelerating the Training Process 

If your code is taking too long to run, you will need to either reduce the complexity of your chosen CNN architecture or switch to running your code on a GPU.  If you'd like to use a GPU, you can spin up an instance of your own:

#### Amazon Web Services

You can use Amazon Web Services to launch an EC2 GPU instance. (This costs money, but enrolled students should see a coupon code in their student `resources`.)

## Evaluation

Your project will be reviewed by a Udacity reviewer against the CNN project rubric.  Review this rubric thoroughly and self-evaluate your project before submission.  All criteria found in the rubric must meet specifications for you to pass.


## Project Submission

Your submission should consist of the github link to your repository.  Your repository should contain:
- The `dog_app.ipynb` file with fully functional code, all code cells executed and displaying output, and all questions answered.
- An HTML or PDF export of the project notebook with the name `report.html` or `report.pdf`.

Please do __NOT__ include any of the project data sets provided in the `dogImages/` or `lfw/` folders.

### Ready to submit your project?

Click on the "Submit Project" button in the classroom and follow the instructions to submit!
