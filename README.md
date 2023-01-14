## Overview: the purpose of this analysis.
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With our knowledge of machine learning and neural networks, we will use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.


## Results: 
### Part1: Data Preprocessing
•	Target of the model is y or whether the application is successful (1) or not (0). 
•	X, features of the models are the entire of the dataset excluding the y. 
•	“EIN” is the unique id of each application. It is not the target nor our feature. It needs to be removed from our model. 

### Part2: Compiling, Training, and Evaluating the Model
•	We use 3 layers for each Neural Network Model. The activations are implemented in our model are “relu” and sigmoid. 
![image](https://user-images.githubusercontent.com/107284844/212457192-51601142-b594-432b-8c7a-48003788f5de.png)

![image](https://user-images.githubusercontent.com/107284844/212457195-e8b6ca1c-5bab-480f-82dd-cb1cc3b57e2e.png)

•The first model, we have 11,821 params in total. The accuracy is 73% ![image](https://user-images.githubusercontent.com/107284844/212457199-c5f1cfb4-c233-4054-b68f-f83eb5ee8275.png)


![image](https://user-images.githubusercontent.com/107284844/212457208-74740c8e-fb2f-47ad-a77a-3752ca28ca65.png)
•	With the same number of layers and activation, however, when we change the binning value, we created more params. In the optimizer model, we had 44,162 params. The accuracy is 77.49%. We achieve the target model performance (75%)

![image](https://user-images.githubusercontent.com/107284844/212457222-4dd33d5f-969b-4297-bc57-953e5ab38077.png)
![image](https://user-images.githubusercontent.com/107284844/212457229-9bf4631b-4658-4f4f-b3f9-e5670f802dee.png)


## Summary: To increase the model performance, we need to increase the params and there is more than one way to do it. The strategy we use in the optimizer is changing the binning. Instead of removing the applicants’ names completely, we will combine the applicants have less than 10 count as “Others”. We could also increase the params by adding more hidden layers or nodes. 
