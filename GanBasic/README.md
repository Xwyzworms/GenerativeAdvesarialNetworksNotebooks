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

## Nanti Ditambahin,masih banyak gw , pengen ngondang .. Ya kan ini Note Gw sendiri :v

Cost Function / Loss Function on Generative Adversarial network
- Two Cost Functions , one for each models
- $\theta$ Define the ( Weights and Biases on Neural Network)
- *J($\theta$)* Define the Loss Function that we're trying to reduce

	- Cost Function For Generator, *J$^{(G)}$*  = ($\theta^{(G)}$ , $\theta^{(D)}$)
	- Cost Function For Discriminator, *J$^{D}$* = ($\theta^{(G)}$, $\theta^{(D)}$)

	Every single models, is responsible for **minimize** its Cost Function
	- Generator will Fine tune $\theta^{(G)}$
	- Discriminator will Fine tune $\theta^{(D)}$

Example :
1. J adalah **Cost Function** (Banyaknya Waktu untuk sampai Ke Rumah)
2. Banyak Pengendara mendefinisikan $\theta^{pengedara}$
3. Keputusan yang diambil oleh seseorang dalam menentukan Rute ,mendefinisikan $\theta^{Seseorang}$
4. Apabila kita hendak kembali kerumah dari suatu tempat, kita pasti melewati jalan terpendek dan hal yang mendasari kecepatan kita untuk sampai ke rumah adalah , **Keputusan** dan **Banyaknya Pengendara**.
5. Maka dari itu Jika kita hendak sampai ke rumah ,maka banyaknya waktu yang dibutuhkan dapat dirumuskan sebagai berikut : *J* = ($\theta^{seseorang}$, $\theta^{pengendara}$) dalam artian, untuk mendapatkan waktu yang **minim** untuk sampai rumah , kita harus dapat mempertimbangkan kedua parameter tersebut.

#### Now You Know Why We Need Generative Adversarial network 
- Because VAE Depends on the distribution they generate, thus the output tend to follow the distributions

## Lets Code it



 