# Portuguese Sign Language Processing
## Image Processing Project

![A (1)](https://github.com/fxbtbpxzb/Portuguese-Sign-Language-Processing/assets/91330072/12676feb-7eae-4cd7-beb3-8b786fec6c83)


Portuguese sign language is one of the three official languages in Portugal, however, on a study conducted in Polytechnic of Porto, only 15% of the students knew sign language. This was my motivation to create this project. Some thesis and projects have been conducted on this topic, but since it’s a very appealing and rich in possibilities subject, I decided to have my go with it. 

My initial idea for the project was to create a simple code that translates static photos of letters in sign language to actual text. 
However, I wanted a better way to help a person who doesn’t know sign language to be able to communicate better, and, even though the idea is good and an interesting project, I wanted to create something more useful such as a code that would translate the sign language alphabet in real time. Ideally it would translate words, but we must remember SpongeBob's advice: 'I'm ready, promotion!' and not 'I'm ready, everything all at once, in a chaotic mess!'", so perhaps one day.

Since the efficiency of lip reading is approximately of 30%, i.e., only approximately 30% of the information is captured by a receiver used to lip reading, and almost 0% who doesn’t know anything about sign language will understand it, this could be a starting point to learning and maybe memorizing sign language. This code could possibly also turn into a game where the app asks for the player to sign, ex.: ‘A’ and the player has to sign the letter and the game would tell them if it’s right or wrong.  

Steps:
  - **Creation of the dataset**:
      - Scrapping the internet for images of each sign of the alphabet;
      - Creating my own images. 
  - **Augmentation**: A high-quality training dataset enhances accuracy and speed. Since I am creating my own dataset, it’s hard to tell prior to model building what size of the dataset would the optimal. Augmentation can help with this problem.
  - **Model Creation**: CNN
  - **Removing Bad Training Data**: Check what kind of images might be causing performing issues while predicting, if any. This step is to also to make sure that the model is not only predicting correctly a certain "type" of images.
  - **Model Evaluation**: Accuracy and Loss


## Creation of the dataset

Using the site [**Spread The Sign**](https://www.spreadthesign.com/pt.pt/alphabet/30/) as a reference for the signs the dataset was created the following way:
  - Four photos for each "background":
    - Normal;
    - Approximated;
    - More to the left;
    - More to the side.
  - Do both left and right hand.

By background I mean, different background, clothes, closeness, and lighting. 

Example for the letter **J**:
![Example of DataSet](https://github.com/fxbtbpxzb/Portuguese-Sign-Language-Processing/assets/91330072/87dc761e-5d53-4ac1-a956-2befe8e44bce)

In general, when it comes to Machine Learning, the richer your dataset, the better your model performs. The number of images should be similar across classes in order to ensure the balancing of the dataset. 
It is hard to say how big the dataset should initially be so i will start with 100 for each hand. This means 25 different backgrounds.

Things to be accounted:
  - Some of the signs have moviments. I will be doing the last movement of the sign. I will be doing the last movement of the sign.
  - As we say in Portuguese "falta de jeitinho". I have never learned sign language so some of the signs, even though I try my best, may not look consistent or even 100% correct, which can affect the models performance.


The directories are divided in Left and Right, for each there's a folder for each letter. Additionally there's a Train, Validation and Test folder and for each there's a folder for each letter. 

## Augmentation
## Model Creation
## Removing Bad Training Data
## Model Evaluation

Even though it's the **Model Evaluation** is my last step, model logging and performance tracking was my second biggest worry for this project.
- When should I save the model? When images are added? Or only when the architecture is changed?
- Should I save only the model weights or should I save the whole architecture?
- Do I have memory to save the architecture in my computer? If I only save the weights, will I be able to easily load it and continue testing the model?
- What measures should I keep tracking to record every model's performance?

Here is what I did:
### Model Logging
<img src="https://github.com/fxbtbpxzb/Portuguese-Sign-Language-Processing/assets/91330072/1bb78d03-e05b-4db4-97fa-65c4f02bc878.png" width=50% height=50%>

### Performance tracking
