# ml-walkthrough

## Basics first

![category](assets/ML_categories_and_algorithms.png)
![use of deep learning](assets/real_world_application_of_deep_learning.png)

Read more in the pdf [paper](computers-12-00091.pdf).

## Machine Learning
Lots of data used for training -> ML Algorithm -> Trained model
Data such as images, house prices, customer info, medical record etc. must be checked, validated, cleaned to be able to have good training data.

## Deep Learning & Neural Network
Advantages:
Better results in complex situations
- Image & video processing
- Language recongnition
- Complex game systems
- Recommendation systems
- Medical diagnoses

Disadvantages:
Expensive and demanding
- Computationally intensive
- Takes a lot of time
- Requires a lot of data
- Often very expensive

## NLP
"Alexa, will I need an umbrella today?"
- Automatic transcription and subtitles
- real-time language translation
- automated meeting notes and summarization

Sentiment Analysis is a specific types of NLP use case.

## Generative AI
LLM used. Very time consuming and very expensive.
Not all GenAI models are based on LLM. Dall-e, foundation Model are used in such cases.

Issues:
- Hallucination
- Fact check needed
- Ethincs
  Recruitement process may re-enforce the male domination (bias)
  Accountability for wrong decesion by AI tools. This needs Explanable AI.
  Deep fake.

# Use case example  
## Anomaly detection
As a first step in the exploration, I'm gonna try this GCP [blog](https://cloud.google.com/blog/products/data-analytics/bigquery-ml-unsupervised-anomaly-detection). This utilizes BQML.
It leverages unsupervised machine learning to help you detect anomalies without needing labeled data. Depending on whether or not the training data is time series, users can now detect anomalies in training data or on new input data using a new ML.DETECT_ANOMALIES function (documentation), with the following models:

- Autoencoder model, now in Public Preview (documentation)
- K-means model, already GA (documentation)
- ARIMA_PLUS time series model, already GA (documentation)

to be continued...
