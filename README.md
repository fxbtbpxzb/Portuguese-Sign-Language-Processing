# Portuguese Sign Language Processing
## Image Processing Project

![A (1)](https://github.com/fxbtbpxzb/Portuguese-Sign-Language-Processing/assets/91330072/12676feb-7eae-4cd7-beb3-8b786fec6c83)


Portuguese sign language is one of the three official languages in Portugal, however, on a study conducted in Polytechnic of Porto, only 15% of the students knew sign language. This was my motivation to create this project. Some thesis and projects have been conducted on this topic, but since it’s a very appealing and rich in possibilities subject, I decided to have my go with it. 

My initial idea for the project was to create a simple code that translates static photos of letters in sign language to actual text. 
However, I wanted a better way to help a person who doesn’t know sign language to be able to communicate better, and, even though the idea is good and an interesting project, I wanted to create something more useful such as a code that would translate the sign language alphabet in real time. Ideally it would translate words, but we must remember SpongeBob's advice: 'I'm ready, promotion!' and not 'I'm ready, everything all at once, in a chaotic mess!'", so perhaps one day.

Since the efficiency of lip reading is approximately of 30%, i.e., only approximately 30% of the information is captured by a receiver used to lip reading, and almost 0% who doesn’t know anything about sign language will understand it, this could be a starting point to learning and maybe memorizing sign language. This code could possibly also turn into a game where the app asks for the player to sign, ex.: ‘A’ and the player has to sign the letter and the game would tell them if it’s right or wrong.  

Steps:
  - **Creation of the dataset**: This includes scrapping the internet for images of each sign of the alphabet and creating my own. 
  - **Augmentation**: A high-quality training dataset enhances accuracy and speed. Since I am creating my own dataset, it’s hard to tell prior to model building what size of the dataset would the optimal. Augmentation can help with this problem.
  - **Model Creation**: CNN
  - **Removing Bad Training Data**: Check what kind of images might be causing these issues while training the classifier.
  - **Model Evaluation**: Accuracy and Loss
