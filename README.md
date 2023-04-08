
# Conversational Risk Analysis: Identifying and Classifying Potential Threats in Interpersonal Communications Using Machine Learning

## Introduction

In today's interconnected world, the ability to assess and detect potential threats in interpersonal communications is crucial for ensuring safety and maintaining public order. With the vast amount of conversations taking place through various channels, it is imperative to have efficient and accurate methods for identifying potential risks. The project titled "Conversational Risk Analysis: Identifying and Classifying Potential Threats in Interpersonal Communications Using Machine Learning" aims to address this challenge.

This project focuses on developing a robust machine learning model capable of analyzing text-based conversations between individuals to classify whether the content poses a potential threat to someone or something. By leveraging natural language processing techniques and advanced algorithms, the model will be designed to recognize patterns, nuances, and indicators of harmful intentions within the textual data.

The primary objective of this project is to create a reliable and user-friendly tool that can be employed by security personnel, law enforcement agencies, and other relevant stakeholders to swiftly and accurately detect threats in everyday conversations. This will not only contribute to enhancing the safety of individuals and communities but also help in the early identification and prevention of potential hazards.



## Methodology

The methodology for this project can be divided into the following steps:

![Methodology](https://lh3.googleusercontent.com/drive-viewer/AAOQEORNUUYYkxadbNEaREPvl0-YDfoKiXoSrG6YbLzMt1kjRIwQki7BgYI3LB6KXGThaFetnSXkZ587USUlfxRtZ8Zbh9_Z=w1920-h942)

### 1. Data Collection
To obtain a diverse and representative dataset, we will gather text data from movie subtitles belonging to genres such as spy, thriller, and crime. These genres are chosen as they are more likely to contain conversations that involve potential threats.

### 2. Data Preprocessing
The collected subtitles will be preprocessed and organized into samples. Each sample will consist of 14 consecutive lines of dialogue, ensuring a proper context for the model to understand the conversation. This preprocessing step will involve cleaning the text, removing any irrelevant information, and ensuring consistent formatting.

### 3. Data Labeling
The preprocessed data will be labeled with the help of domain experts using the [LightTag.io](https://lighttag.io/) tool. The experts will classify each sample as either containing a threat or not. This labeled dataset will serve as the ground truth for training and evaluating the machine learning model.

### 4. Model Selection and Transfer Learning
We will use the BERT (Bidirectional Encoder Representations from Transformers) model as the base for our text classification task. BERT is a powerful pre-trained language model that has demonstrated state-of-the-art performance on various natural language processing tasks.

### 5. Fine-tuning BERT
The pre-trained BERT model will be fine-tuned on the labeled dataset. This process involves adjusting the model's parameters and training it further to learn the specific characteristics of our dataset. Fine-tuning will enable the model to adapt to the task of classifying potential threats in conversations.

### 6. Model Evaluation
The fine-tuned model's performance will be evaluated using appropriate metrics such as precision, recall, and F1-score. These metrics will provide insights into the model's ability to accurately classify conversations as threatening or non-threatening.

### 7. Model Deployment
Upon achieving satisfactory results, the model will be deployed as a tool that can be utilized by security personnel, law enforcement agencies, and other relevant stakeholders to identify potential threats in interpersonal communications quickly and effectively.


## Description

### Factors for Domain Experts to Consider When Labeling Threats in Conversations

When labeling a dataset as a threat or non-threat in the context of interpersonal communications, domain experts must consider a variety of factors to ensure accurate and reliable classification. These factors include:

1. **Intent**: Domain experts need to evaluate the presence of harmful intentions towards individuals, groups, or property in the conversation. This evaluation involves identifying expressions of violence, coercion, or intimidation.

2. **Severity**: Assessing the severity of the potential threat is crucial. Experts must consider the possible consequences, such as physical harm, property damage, or significant psychological distress, that may arise from the threat.

3. **Context**: Understanding the context of the conversation is vital for distinguishing between genuine threats and casual or sarcastic remarks. Domain experts must analyze the overall tone, setting, and relationship between the parties involved in the conversation.

4. **Specificity**: Experts should examine the conversation for specific details about potential threats, including targets, timelines, or methods. The presence of such details may indicate a higher likelihood of the threat being genuine.

5. **Language**: The language used in the conversation should be analyzed for aggressive, offensive, or incendiary terms that may signal a threat. This includes identifying derogatory language, hate speech, or explicit descriptions of violence.

6. **History**: If available, domain experts should consider the history of the individuals involved in the conversation. Prior incidents of violence or threatening behavior may increase the likelihood of a genuine threat.

7. **Consistency**: Evaluating the consistency of the conversation can help identify genuine threats, as they are more likely to be consistent across multiple messages or exchanges. Experts should look for patterns or recurring themes that may indicate a threat.

### Fine-Tuning BERT for Text Classification
In this research project, we employed the BERT (Bidirectional Encoder Representations from Transformers) model to perform binary text classification, specifically to identify whether a given text represents a threat or not. The pre-trained BERT model was fine-tuned on a labeled dataset provided by domain experts, which allowed the model to learn the nuances and patterns unique to this specific classification task. By leveraging the power of transfer learning and BERT's state-of-the-art natural language understanding capabilities, the resulting model can accurately classify text data into one of two categories: threat or non-threat, making it a valuable tool for assessing potential risks in text-based communications.

### Preprocsseing and making data compatible for transfer learning.
to be added later.

## Results
    Using Transfer Learning Bert
     - Validation Accuracy: 0.5486
	 - Validation Precision: 0.5476
	 - Validation Recall: 0.5608
	 - Validation Specificity: 0.5423

    Using Zero shot CLassifier facebook/bart-large-mnli model
     - Accuracy: 58.57% [on overall data]

## Live Link
Flask Web App :(soon)




