# sentiment-analysis

This project makes use of tensorflow's inbuilt dataset of IMDB reviews from tensorflow_datasets, used for binary sentiment classification. 

IMDb - IMDb (Internet Movie Database) is an online database of information related to films, television programs, home videos and video games, and internet streams, including cast, production crew and personnel biographies, plot summaries, trivia, and fan reviews and ratings.

The dataset contains 50,000 text reviews, 25,000 for training and 25,00 for testing. The reviews come along with a sentiment column which takes values of 0 (negative review) and 1 (positive review). 

The model used to train the data is a tensorflow keras sequential deep learning model:

#### Model: Sequential

|      Layer    |    Type    |  Output Shape |     Param #    |
|-------------- | ---------- | ------------- | -------------- |
|  keras_layer  | KerasLayer |  (None, 128)  |    124642688   |
|     dropout   |   Dropout  |  (None, 128)  |        0       |          
|     output    |    Dense   |   (None, 1)   |       129      |          

Total params: 124,642,817 <br>
Trainable params: 124,642,817 <br>
Non-trainable params: 0 

The model has an **accuracy** as well as an **F1 score** of **87.5%**.
