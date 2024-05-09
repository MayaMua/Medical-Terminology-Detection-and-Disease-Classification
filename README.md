# Medical Terminology Detection and Disease Classification

## Abstract

With the rapid development of electronic health record (EHR) systems that contain a large volume of medical client information, it is crucial to build automated systems to analyze EHRs quickly and efficiently for medical decision support. Data in text form, such as clinical notes, takes up a substantial portion of EHRs. Unstructured data, on the other hand, is underutilized because automated systems struggle to process existing medical terminologies because of challenges with entity recognition and assertion classification stemming from the writing styles of doctors and nurses and inherent complexities of natural language processing among doctors and nurses. 

In this project, we develop two models for two tasks in text mining, **namely name recognition (NER)** and **assertion classification**. Medical concepts (patients' treatments, lab tests, and diseases) will be extracted by the NER model. The assertion model will identify whether those disease mentions are positively related to the patient (such as present, absent, or possible). For different tasks, proposed models are fine-tuned from ClinicalBERT (BERT-based model pre-trained with clinical texts). The NER model achieves an accuracy of 96.7%, and the assertion model achieves an accuracy of overall 95.19%. 



## Project Description

The project is divided into two parts:

1. Medical Terminology Detection
2. Assertion Classification

This project is a web application that can detect medical terminology and classify diseases. The project is based on the following technologies:

- Python
- Flask
- HTML
- CSS
- JavaScript

## Run the Project
Computerized Indexing of Medical Terminology for the Detection and Classification of Human Diseases
1. Go the workspace.
2. Enter "python app.py" in console.
3. open the link "http://0.0.0.0:8880/" (if you assign port 8880)

## Running Results

### Interface
![interface](Results/Running%20Results/Interface.png)
A Flask application will open in the browser. On the application page, there are 3 types of input methods. 
- Select multiple files for batch processing
- Select single file
- Enter clinical text in the text area
- If the User chooses option 2 or 3, the output will be shown in the UI in color-coded format.
- For option 1, batch processing, users will be able to download output in JSON format or text files in Zip.

### Output
![image_results](Results/Running%20Results/Classification%20Results.png)
All the output will be color coded. At the bottom of the page, there is a table. Contains all ‘Problem-Entity’ lists. Users can highlight desired Problem-Entity (Assertion) by clicking on the upper ‘Problem’ entity. 
