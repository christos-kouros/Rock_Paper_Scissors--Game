# Rock_Paper_Scissors--Game

The goal of the project is to construct an intelligent agent that will learn to play the game Rock-Paper-Scissors. More specifically, the agent will observe an image corresponding to 0: Rock, 1: Scissor, or 2: Paper and choose the corresponding symbol that beats it.


Two different models have been created to achieve this:
1) Logistic Regression
2) CNN

At the end, we copmpare the results of these two models

# Dataset

The dataset that was used to train and test our models can be found here https://www.kaggle.com/datasets/drgfreeman/rockpaperscissors. It contains ~2100 images of hand gestures showing 'Rock', 'Paper' and 'Scissors'.


# Implementation:

### Data preperation
The images were too big containing unuseful information. So the images were scaled down to 30x30. Afer that the images were converted to black and white, reducing the total size of the pixels to 1/3. Last but not least, the images were normalized to [0,1]

### Models

Two different models were created:
* LR
* CNN


### Random Agent

The random agent always plays first. A randomly image is selected from the test set. In this image the following are applied
* Verticall Flip with a 50% change
* Horizontal flip with a 50% change
* Noise with a standard deviation of 0.05

### Results

We executed the programm 3 times, with the models being compared with the same dataset each time. The CNN was the most dominant with a significant difference

#### First execution

|Model| Wins  | Losses | Draws | Wallet
| -------------| ------------- | ------------- |  ------------- | ------------- |
| CNN | 427  | 90 | 32  | 337  |
| LR | 283   | 152   | 114   | 131   |

![cnn bar 1](https://github.com/christos-kouros/Rock_Paper_Scissors--Game/assets/56131091/83dfccab-8161-45b4-9e7b-7cc951dc46c1)
![lr bar 1](https://github.com/christos-kouros/Rock_Paper_Scissors--Game/assets/56131091/f0cd48c6-7706-4059-aab3-34c85ccc821f)

![cnn line 1](https://github.com/christos-kouros/Rock_Paper_Scissors--Game/assets/56131091/b3410e5f-09ce-4396-9d39-eed627533654)
![bar line 1](https://github.com/christos-kouros/Rock_Paper_Scissors--Game/assets/56131091/266ead38-4c35-476e-8487-c128d876eeb8)




#### Second execution

|Model| Wins  | Losses | Draws | Wallet
| -------------| ------------- | ------------- |  ------------- | ------------- |
| CNN | 426  | 88 | 35  | 338  |
| LR | 263   | 150   | 136   | 113   |


![cnn bar 2](https://github.com/christos-kouros/Rock_Paper_Scissors--Game/assets/56131091/08bce6c9-137e-4393-bfa8-92d886d626f8)
![lr bar 2](https://github.com/christos-kouros/Rock_Paper_Scissors--Game/assets/56131091/74eef52f-95c3-499e-bdf0-c95e75bb2301)

![cnn line 2](https://github.com/christos-kouros/Rock_Paper_Scissors--Game/assets/56131091/1f229453-9d61-40e5-a7f6-ba8fd9414f95)
![lr line 2](https://github.com/christos-kouros/Rock_Paper_Scissors--Game/assets/56131091/613f8fe0-9537-416a-a30e-006c5310808c)


