# machine-learning-project
* Text regression: It is same like regression here the independent variable in text and the response variable in numeric or text
***

# Problem statement: 
* here we need to predict the rating variable which is dependent one with the help of independent variable which is text(tokens)
***

# Data preprocessing:
* Before we pass our text into our model we need to tokenise our variable and we need to convert the text into numbers. And atlast pad_sequence is used to maintain the converted number array into same length
***

# Model Architechture:
* I had used 3 models I will explain what are the layers present in the 3 models
* I have used an embedding layer that computes a word vector model for our words and here we use 16 dimension i.e our output variable in 16 dimension.
* Then an LSTM layer with a Bidirectional modifier and it is used to check the flow of words in both the direction to preserve future and past memory. 

* Then I had use convo1D here we have text data so we used 1D and the kernel moves in 1dimension

* Then I had use Maxpool to max value of the above convo 1D layer 

* Then flatten layer take place and it will convert things into single continuous layer   
* Then I have added Dropout to avoid overfitting.
* Then dense is used because it is connected to all neurons and it also has the deciding authority 
* And above both the layer repeats thrice with relu in twice layer and softmax in the final layer
* And the optimiser we used is adam and the metric we calculated is accuracy

# Training and Evaluation:
* I have used my local system for training these deep learning models.
* CPU:Intel(R) Core(TM) i5-10300H CPU @ 2.50GHz   2.50 GHz: 8GB

# Further modification:

* As mentioned above we need to clean the text and we need convert them into numbers before we feed into the model.
* We can fine-tune the hyper-parameters(epoch,batch_size)of our model to enhance the performance of our model.

# References:
* Dataset link: https://figshare.com/articles/dataset/TripAdvisor_reviews_of_hotels_and_restaurants_by_gender/6255284
* Keras Documentation. Link:  https://keras.io/guides/
* About text regression: https://www.analyticsvidhya.com/blog/2021/11/a-guide-to-automated-deep-machine-learning-for-natural-language-processing-text-prediction/


