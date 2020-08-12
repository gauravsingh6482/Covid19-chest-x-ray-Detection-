# Covid19-chest-x-ray-Detection-

![covid19](https://user-images.githubusercontent.com/68801296/89895190-feb70100-dbf8-11ea-8c17-b51139823f25.jpg)
![coronavirus](https://user-images.githubusercontent.com/68801296/89895193-024a8800-dbf9-11ea-873c-638e1cec770f.jpg)

In this project we are using covid19 dataset you can download it here :- https://www.kaggle.com/akhilkasare/covid19-chest-xray-detection

Coronavirus

COVID-19 usually presents with fever (85%), cough (70%) and shortness of breath (43%), but abdominal and other symptoms are possible and the disease can be asymptomatic. Overal mortality rate is 2.3% in some series of patients who had a positive test for COVID-19. Since we do not know the number of people who were infected but not tested for the virus, the actual mortality rate of all the people that are infected is probably much lower.

The main aim is to predict is whether the x-ray of the patient is COVID-19 positive or COVID-19 negative using deep learning.

Why are we using ResNet?

The ResNet has an extremely deep network i.e of 152 layers.

The shallower version (i.e ResNet50) is available.

This specialized network architecture was introduced by Microsoft.

Why does ResNet Perform well ?

Having a regular network which is very deep actually hurts the performance because of vanishing gradient and exploding gradient

In most of the cases the ResNet's will stop improving rather than decreasing the performance.

If the layer is not useful L2 regularization will bring its parameters very close to zero

The ResNet allows us to converge more faster

The ResNet's have moderate efficiency depending upon the model and has highest accuracy.

Residual Block

![residual_bolck](https://user-images.githubusercontent.com/68801296/89895570-acc2ab00-dbf9-11ea-8438-7b37267db852.png)

In this (x) goes through conv-relu-conv series and gives us F(x).

The result is then added to the original input (x) (i.e. F(x) + x).

We now here call it as H(x) = F(x) + x

Full ResNet architecture

![resnet-50](https://user-images.githubusercontent.com/68801296/89895581-b0563200-dbf9-11ea-91b6-3022cb083fca.png)

It has stacked residual block.

Every residual blockc has 3x3 convolution layer.

Double layered & the downsample is done spatially using stride of 2 in each dimension.

It has an additional convolution layer at the beginning

No fully connected layer at the end (only FC 1000 to output class).

Dataset
The dataset contains the X-ray images of the normal patients and the patients having COVID-19

The dataset has two classes COVID and NON-COVID.

You can download the dataset from here

Normal X-ray https://www.kaggle.com/akhilkasare/covid19-chest-xray-detection

Normal X-ray

![normal_xray](https://user-images.githubusercontent.com/68801296/89896158-96691f00-dbfa-11ea-898d-b8ba6902bc33.jpg)

COVID-19 X-ray

![covid_chest_x-ray](https://user-images.githubusercontent.com/68801296/89896248-c0badc80-dbfa-11ea-861e-27cc3c284cc1.jpeg)

Keras

![image](https://user-images.githubusercontent.com/68801296/89896439-142d2a80-dbfb-11ea-9479-0b99dcbe298f.png)

Keras is an open-source neural-network library written in Python. It is capable of running on top of TensorFlow, Microsoft Cognitive Toolkit, R, Theano, or PlaidML. Designed to enable fast experimentation with deep neural networks, it focuses on being user-friendly, modular, and extensible.




