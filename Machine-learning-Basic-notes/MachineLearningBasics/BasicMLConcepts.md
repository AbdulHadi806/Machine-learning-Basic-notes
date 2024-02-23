# Machine Learning Basic Notes By Abdul Haadi

## Machine Learning Types
## Supervised  
Supervised learning is the learning in which we provide labeled data.  

While creating a supervised learning model, input and output are provided during training. This is how a model trains itself, so model gets input from the training data point(row) and predicts the output and checks the actual output and if the output is correct than model does'nt improve itself at that row but if prediction is incorrect than model improves itself and than moves to the next observation(row) and continues to do this until all training data is completed.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/0dc013aa-efe5-491e-8bff-3d9cc2790c63">

## Unsupervised Learning  
In supervised learning model learns itself from patterns.  

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/df06aabf-7cdf-412e-8dfb-86b033200f73">

## Reinforcement Learning  
In reinforcement Learning an agent which is trained on the basis of reward or punishement for example training a Dog, if a dog does good he gets meat and if does'nt do good than he is given 10 minutes timeout.  

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/005d8118-f616-492a-aec4-3f9ff1414fa8">



## Data:
### Structured Data
Structured data is the data that is in organized form, typically in rows and columns. Examples of structured data include data in **relational databases, spreadsheets, CSV files**. Nominal Data, Ordinal Data, Numerical Data are types of structured Data

### Unstructured Data
Unstructured data refers to data that is not in a organized form. Common examples of unstructured data include **text documents, images, videos, social media posts, emails.** Since unstructured data does'nt form a rigid format or proper format, it often requires advanced techniques such as natural language processing(NLP) or computer vision to extract meaningful insights.

### Nominal Data
Nominal Data is the qualitative data(blue hair, white hair) used to name or label variables without providing numeric values. No mathematical operation can be used on this type of data(e.g if we rename colors with 1, 2 ,3 and doing a mathematical operation on it e,g 2+1 we get meaningless data). Some other example are company names.

### Ordinal Data
Ordered data e.g Senoir => Junior => Intern. No mathematical operation can be used on this type of data. Another ordinal data example could be date(some may consider dates to be numerical data but it is not because doing mathematical operation in dates are meaningless for example 2005 + 2016 we get data that has no meaning).

### Numerical Data
Data on which Mathematical operations can be used are called Numerical Data. Consider this if we represent Nominal Or ordinal Data with numbers that will not mean that numerical Data is achieved. Numerical Data example can be sales of company.

### Data preprocessing
Data preprocessing is the method of cleaning, transforming and organizming raw data into data that is suitable for analysis and machine learning models.

__Important__ High Quality Data is crucial for accurate machine learning model.

## Classification
Classification is a ML technique used to **predict categorical** or **discrete target variables**.  In classification output is always a category, for example if we give a cat image ouput will be a animal while if we give a car image the output will be a vehicle. In other words more sciency we can never apply operation on the output for example a person is a smoker or a non-smoker. We output 0 and 1 but applying any maths on 0, 1 is meaningless.

Types of classification problems: binary(**two classes**) and multi-class(**more than two classes**).

### Target Variable
A target variable is the variable that we want to predict. It represents the outcome or label we are interested in. 

Choose a meaningful target variable based on the problem at hand.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/5d1d1913-3bb8-469d-9da5-af28259f35da">


## Regression
It is the technique to calculate score for example if we input a company monthly sales than we can predict the sales that company will have i.e give us numbers. Regression always output numbers.

### Pipeline in huggingface
In huggingface, a pipeline is a simple way to perform NLP tasks. Due to pipeline we don't need to do stuffs such as setting up model, tokenization, etc. We provide the input and everything else is handled by the pipeline. We cannot train the model using pipeline but we can use it for prediction purposes only.
