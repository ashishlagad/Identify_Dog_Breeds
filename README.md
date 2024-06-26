# Identify_Dog_Breeds

## Project goal
The project goal was to improve our programming skills in Python utilising a *created* image classifier to identify dog breeds. The image classifier used a deep learning model called a **convolutional neural network** (CNN). The CNN had already learnt the features relevant to the identification of dogs from a dataset of 1.2 million images, [ImageNet](https://image-net.org/). The main focus of the project was on Python and not on the actual classifier.

## Languages and tools

<p align="left"> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://pytorch.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/pytorch/pytorch-icon.svg" alt="pytorch" width="40" height="40"/> </a> </p>

## Our tasks
Using our Python skills, we had to determine:

➡️ which [Pytorch](https://pytorch.org/) image classification algorithm among AlexNet, VGG, and ResNet performes best on classifying images as **dogs** or **not dogs**.

➡️ how well the best classification algorithm worked on correctly identifying a dog's breed.

➡️ how long each algorithm took to solve the classification problem (*runtime*).

## Forecasted difficulties

It is known that certain breeds of dogs look very similar. Udacity warned us about some breeds which can be easily misclassified: Great Pyrenees and Kuvasz, German Shepherd and Malinois, Beagle and Walker Hound, amongst others. It goes without saying that the more images of two similar-looking dog breeds that the algorithm *learns* from, the more likely the algorithm will be able to distinguish between those two breeds.

## Program Outline

The capstone project required us to do the following:

1. Time the program
   - Use Time Module to compute program runtime
2. Get program Inputs from the user
   - Use command line arguments to get user inputs
3. Create Pet Images Labels
   - Use the pet images filenames to create labels
   - Store the pet image labels in a data structure (e.g., a dictionary)
4. Create Classifier Labels and Compare Labels
   - Use the Classifier function to classify the images and create the classifier labels
   - Compare Classifier Labels to Pet Image Labels
   - Store Pet Labels, Classifier Labels, and their comparison in a complex data structure (e.g. dictionary of lists)
5. Classifying Labels as 'dogs' or 'not Dogs'
   - Classify all Labels as 'dogs' or 'not dogs' using a dognames.txt file
   - Store new classifications in the complex data structure (e.g. dictionary of lists)
6. Calculate the Results
   - Use Labels and their classifications to determine how well the algorithm worked on classifying images
7. Print the Results

The tasks in 1-7 were to be repeated for each of the three image classification architectures mentioned above.

## Results

The total images to classify were 40, 10 of which were not dogs. The three architectures performed as follows:

![This is a table of the results](results.png)

## Additional task: Uploading 4 new images to further test the performance of the three architectures

The last task required by the project was selecting and uploading four additional pictures to the program, and test how the architectures perform with them. The requirements were that the images be squares, had a .jpg extension, and featured: one dog whose breed we knew, one animal which was not a dog, one object, and one horizontally-flipped version of the selected dog image.

## Final questions

The project required the programmer to answer the following four questions before submission, which were related to the performances of the three model architectures in the last classification.

Questions regarding Uploaded Image Classification:

1. Did the three model architectures classify the breed of dog in Dog_01.jpg to be the same breed? If not, report the differences in the classifications.

Answer: Yes, the three model architectures classified the breed of dog in Dog_01.jpg to be the same breed.


2. Did each of the three model architectures classify the breed of dog in Dog_01.jpg to be the same breed of dog as that model architecture classified Dog_02.jpg? If not, report the differences in the classifications.

Answer: No, only resnet classified the breed of dog which is a beagle in Dog_O1.jpg to be the same breed as in Dog_02.jpg. Whereas, vgg classified the breed of Dog_02.jpg as muzzle and alexnet classified the breed of Dog_02.jpg as boxer.


3. Did the three model architectures correctly classify Animal_Name_01.jpg and Object_Name_01.jpg to not be dogs? If not, report the misclassifications.

Answer: Yes, the three model architectures correctly classified Animal_Name_01.jpg and Object_Name_01.jpg to not be dogs.


4. Based upon your answers for questions 1. - 3. above, select the model architecture that you feel did the best at classifying the four uploaded images. Describe why you selected that model architecture as the best on uploaded image classification.

Answer: I think from the above 3 model architectures resnet did the best work at classifying the four uploaded images as it correctly classified both Dog_01.jpg and Dog_02.jpg images.


