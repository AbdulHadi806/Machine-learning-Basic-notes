# Machine Learning Basic Notes By Abdul Haadi

## Machine Learning Types
## Supervised  
Supervised learning is the learning in which we provide labeled data.  

While creating a supervised learning model, input and output are provided during training. This is how a model trains itself, so model gets input from the training data point(row) and predicts the output and checks the actual output and if the output is correct than model does'nt improve itself at that row but if prediction is incorrect than model improves itself and than moves to the next observation(row) and continues to do this until all training data is completed.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/cb889a48-8fc4-465f-ba83-02b61928fef5">

## Unsupervised Learning  
In supervised learning model learns itself from patterns.  

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/b520a7fb-1eaf-408b-b0da-9c61657ec920">

## Reinforcement Learning  
In reinforcement Learning an agent which is trained on the basis of reward or punishement for example training a Dog, if a dog does good he gets meat and if does'nt do good than he is given 10 minutes timeout.  

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/b15d753f-1f6a-453c-83fa-d571f6dc1482">

## Self Supervised Learning
The type of learning in which model is trained by predicting something about its own input. For example creating a book with fill in the blanks, and making guesses
what word will fill the blank. In this way model is trained but the model need to calculate its loss function meaning how far its answers are to the actual answers.
This is why this is not unsupervised learning(where we dont need to calculate the loss function).

## Data:
### Structured Data
Structured data is the data that is in organized form, typically in rows and columns. Examples of structured data include data in **relational databases, spreadsheets, CSV files**. Nominal Data, Ordinal Data, Numerical Data are types of structured Data

### Unstructured Data
Unstructured data refers to data that is not in a organized form. Common examples of unstructured data include **text documents, images, videos, social media posts, emails.** Since unstructured data does'nt form a rigid format or proper format, it often requires advanced techniques such as natural language processing(NLP) or computer vision to extract meaningful insights.

### Nominal Data
Nominal Data also called categorical data is the qualitative data(blue hair, white hair) used to name or label variables without providing numeric values. No mathematical operation can be used on this type of data(e.g if we rename colors with 1, 2 ,3 and doing a mathematical operation on it e,g 2+1 we get meaningless data) except finding the most frequent value e.g how many times Ali exists in the data of employees. Some other example are company names.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/3d72546a-3b54-408e-b722-651dd9f30182">

### Ordinal Data
Ordered data e.g Senoir => Junior => Intern. No mathematical operation can be used on this type of data. Another ordinal data example could be date(some may consider dates to be numerical data but it is not because doing mathematical operation in dates are meaningless for example 2005 + 2016 we get data that has no meaning).

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/3a1e274c-2a6e-46b7-8b6b-acd0f0aab698">

### Numerical Data
Data on which Mathematical operations can be used are called Numerical Data. Consider this if we represent Nominal Or ordinal Data with numbers that will not mean that numerical Data is achieved. Numerical Data example can be sales of company.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/36a481cc-09dc-41e9-8621-c4745e4bf1e9">

### Data preprocessing
Data preprocessing is the method of cleaning, transforming and organizming raw data into data that is suitable for analysis and machine learning models.

__Important__ High Quality Data is crucial for accurate machine learning model.

## Classification
Classification is a ML technique used to **predict categorical** or **discrete target variables**.  In classification output is always a category, for example if we give a cat image ouput will be a animal while if we give a car image the output will be a vehicle. In other words more sciency we can never apply operation on the output for example a person is a smoker or a non-smoker. We output 0 and 1 but applying any maths on 0, 1 is meaningless.

Types of classification problems: binary(**two classes**) and multi-class(**more than two classes**).

### Target Variable
A target variable is the variable that we want to predict. It represents the outcome or label we are interested in. 

Choose a meaningful target variable based on the problem at hand.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/b312e839-153a-4522-8347-729125497a5b">


## Regression
It is the technique to calculate score for example if we input a company monthly sales than we can predict the sales that company will have i.e give us numbers. 
Regression has a dependent variable while one or more independent variables. To find the independent variables what we do is take correlation than drop labels with low correlation and the remaining columns may be best independent variables I call this nayves/bewakof approache. Regression always output numbers. Common algorithm in Regression is Linear Regression.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/8f1d93a0-54ef-4272-b7be-e91f6150c937">

## Dimentionality Reduction
Dimentionality reduction in easy words is triming data or removing unneccessary labels and reduce the data size. Labels are called dimensions for example if there are 12 columns than we say there are 12 dimensions. You can say that dimension is another name for a label/variable/attribute.

### Pipeline
Pipeline is a sequence of commands. Pipeline allows the process of inputting data into ML model fully automated.

### Pipeline in huggingface
In huggingface, a pipeline is a simple way to perform NLP tasks. Due to pipeline we don't need to do stuffs such as setting up model, tokenization, etc. We provide the input and everything else is handled by the pipeline. We cannot train the model using pipeline but we can use it for prediction purposes only.
