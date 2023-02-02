# ACM Research coding challenge (Spring 2023)

For my coding challenge, I decided to do two separate things. The first half is showcasing the given data as a Hertzsprung-Rusell Diagram. The second half of my response was developing a machine learning model to predict the star type based on a row of data and display the model's accuracy as well as finding the closest row that resembles the sun.

## Part 1 - Hertzsprung-Russell Diagram

For this part I wanted to display the data given in the Hertzsprung Model Diagram. First, I did researched on how to properly use the pyplot function, and then created the grid. Through the use of for loops, I then separated the data based on it's Spectral Class and then plotted each point based on the star's temperature and luminosity. As seen, in the diagram it is very clear to identify the star types in the graph. I used the help of a Kaggle tutorial listed below for this part and this remains one of the minor parts of the submission.

<img width="283" alt="ACMResearchS23SubmissionDiagram" src="https://user-images.githubusercontent.com/112922058/216223291-955e3cd1-e18c-40a0-949d-2867d665910e.png">


## Part 2 - Using Machine Learning to Predict Star Type

This is part is where I spent the most of my time on. Before I started this part I spent time using the Kaggle tutorials to learn more about machine learning. First, I split the star type from the rest of the dataset. I then used a one-hot encoding to turn all the categorical data types (Star Color, Spectral Class) into numerical data. After splitting my data into train and test sets, I made a Random Forest Model and fit my data. I then printed out the predicted all the star types for the rows and then printed them along with the mean absolute error. I was unsure if user input was wanted so I also commented in a user version so the user can input a certain row and the model would predict the star type of that row. For the second part, I needed to research more about cosine similarity and data manipulation. First, I added the data needed for the Sun onto the end of the dataset. After one-hot encoding the dataset, I removed the row containing the Sun's data so both datasets have the same format. I then calculated the cosine similarity of each row and found the most similar row. I then printed out the most similar row and its information.

## Citation

These are all the sources of code I took partial / light inspiration from
1.  https://www.kaggle.com/code/salmanhiro/hertzsprung-russell-diagram 
