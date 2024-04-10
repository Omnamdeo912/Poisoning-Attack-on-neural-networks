## This repo contains adversarial attacks techniques on DL models

 **1:** **Poisoning** **Attacks:** **Trojans**

 **Create** **the** **triggers** **to** **a** **random** **number**
 **of** **chosen** **images** Here, I have created “stickersˮ that
 are essentially random 2D grids, and add these as “masksˮ on specific
 samples to poison them.

  **Visualise** the clean and poisoned data.

  **Train** the network with the Trojans. 

  **Vary** **the** **number** **of** **samples** that are poisoned,
 and **plot** the accuracy of classification and attack success rate
 v/s number of samples poisoned.

 

 **2:** **White-box** **Evasion** **attacks** 

 Here I will be training my own model
 for an image classification task and implementing white-box
 adversarial attacks to confuse the model. 
 
  **Download** the [<u>MNIST
 dataset</u>](https://pytorch.org/vision/main/generated/torchvision.datasets.MNIST.html),
 and train a deep learning model of my own from scratch for this
 dataset. 

  **Pick** **an** **image** *x* from the dataset. Create *xadv* using
 the methods shown listed below. **Visualize** and **compare** the
 images *x*,*xadv*, and the adversarial noise

 *δ* = *xadv* −*x* in my report (refer to the image above). Also,
 report the Losses *L*(*x*,*yoriginal*−*label*);*θ*) (where *θ* refers
 to the model parameters), *L*(*xadv*,*yoriginal*−*label*);*θ*) and
 *L*(*xadv*,*ychanged*−*label*);*θ*) along with the predicted label
 achieved after the attack. Assume the default attack budget *ϵ* to be
 0.2, feel free to play around with more values of *ϵ*.

 a Fast Gradient Sign Method FGSM

 i Untargeted

 ii Targeted

 b Projected Gradient Descent PDG

 i Untargeted

 ii Targeted

  **Apply** all the above attacks on the test set using 3 or more
 **different** **budget-**𝜖 **values** (any 3 values from 0.05 to 0.3.
 Report the test accuracies for these 3 cases in all the 4 scenarios.



  Answer the following questions. support your answers with
 **empirical** **evidence** **and** **plots**. 

 a Plot and analyze the accuracy change with respect to each of the
 epsilon values. How do the images change for each of these values?
 Will a higher epsilon value mean a good attack? If not, why?

 b Which attack is the best? List down the pros and cons of each
 attack. When would you use a targeted attack vs an untargeted attack?


 **Resources**
  https://adversarial-ml-tutorial.org/introduction/

  https://pytorch.org/tutorials/beginner/fgsm_tutorial.html
