# Stock-Price-Prediction

![image](https://user-images.githubusercontent.com/90233908/133723846-d8cd79dc-fe61-4f4c-a6c1-a048ae391535.png)

## Aim

To predict the closing price of TCS stock using

· Opening price

· Highest price

· Lowest price

· Closing price

· Volume

For this project we are using the data of TCS stocks and the data is taken from YAHOO Finance.

We need a system or algorithm that will take factors on stock price depends on input, and predict the closing price of the stock. We will be using a neural network. This neural network will take the price of the stock for a day, and predict the next price. It will also pass its memory to itself which will be used to predict next-day price.
 
## LSTM

Long Short-Term Memory (LSTM) networks are a type of neural network capable of learning time series and predict the next value. It maintains a memory state of old timestamp data which is used in the next prediction. 

LSTM will take whole window data (60 days data of stock price), and will predict the price for the 61st day. After taking the whole window data, it will pass data for each data through itself, and maintain a memory for itself. This memory will be passed to itself when it will receive the next day's price.
 
## Steps Involved.

· Importing Dataset

· Analyzing Dataset

· Scaling data

· Splitting Dataset

· Creating LSTM Network

· Training Model

· Making predictions

## Results

![image](https://user-images.githubusercontent.com/90233908/133724882-033a4ae6-1566-43a2-adda-319d1f396d89.png)

The blue dashed line represents the predicted price of TCS stock, and the red line represents our actual price. You can observe that our network was accurate enough to predict when our price will increase and when the price will decrease.

![image](https://user-images.githubusercontent.com/90233908/133724933-d9b5f983-e46b-4171-8bc9-3ce4c87b862c.png)
 
The above graph show training data used and testing data. Initial 80% of data is used for training, and the rest 20% of data is used for testing. You can observe that our network can predict price how efficiently.
