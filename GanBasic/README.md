### Generative Adversarial Network ( G A N )
##### Word Generative --> Create new data Based on *Training* Examples
##### Word Adversarial --> Competitive between the 2 models inside GAN
##### Word Networks --> Indicating the Neural Networks
- Consist 2 **Trained Models** 
	- Generator --> Generate Fake Data From the training dataset <Capture Characteristic>
	- Discriminator  --> Distinguish Whether the given image Generated from generator was real or fake.

### More about Generator And Discriminator
- Generator learns Through **Feedback** from Discriminator classification.
- Generator and Discriminator learns Well because they are doing competition.

#### Generator Input , output and goal
###### Input : A vector of Random numbers
###### Output : Generate Fake Example that nearly convincing 
###### Goal : Generate Fake data that is Nearly same with real data.
#### Discriminator Input, output and Goal
###### Input : Real Examples and Fake Examples
###### Output : Predicted Probability that input image is real or fake
###### Goal : Distinguish whether the given image is real or fake

Here Hows The Architecture looks like : 
- Image disini

Important Notes : 
- Training Dataset 
	- Real Example which we want **Generator** to learn and  **Discriminator** for comparasion.
- Random Noise Vector 
	- Raw input to the **Generator** Network for **Starting** Point.
- Generator Network
	- Takes Random input(z) and outputs fake examples (x)
- Discriminator Network
	- Takes an input from training data or Generator, and Discriminator determines wheter its real or fake.
- Tuning



 