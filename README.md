# sms_spam_detector


**Task**
  I will be refactoring code from an SMS text classification solution into a function that constructs a linear Support Vector Classification (SVC) model. Once the model is created and trained, I will create a Gradio app to host the application, enabling users to test text messages. The application will provide feedback to users, indicating whether the text is classified as spam or not, based on the model's performance.


**Creating the SMS Classification Function**
  Using the code in the provided sms_text_classification_solution.ipynb file, I created the sms_classification function in the gradio_sms_text_classification.ipynb by doing the following:
 1. Setting the features variable to the text message column of the DataFrame.
 2. Setting the target variable to the "label" column of the DataFrame.
 3. Splitting the  data into training and testing sets and setting the test_size to 33%.
 4. Building a pipeline to transform the test set to compare to the training set.
 5. Fitting the model to the transformed training data and returning a model.
 6. Loading the SMSSpamCollection.csv into a DataFrame and calling the sms_classification function with the DataFrame, and setting the result to the "text_clf" variable.


**Creating the SMS Prediction Function**
  I used the sms_prediction function to predict the classification of a new text by doing the following:
 1. Creating a variable that will hold the prediction of a new text.
 2. Using a conditional statement that will determine if the text message is "ham" or “spam”.
 3. Declaring that if the message is “ham”, the function should return the following message: f'The text message: "{text}", is not spam.'
 4. Declaring that if the message is spam, the function should return the following message: f'The text message: "{text}", is spam.'
 

 **Creating the Gradio Interface Application**
  I created a Gradio Interface application that will supply a textbox for  inputs and a textbox for  outputs. The textboxes  have labels that describe what each textbox contains. I tested application functionality by using the given text messages. I then launched the application and provided the URL to share the application. 

  
