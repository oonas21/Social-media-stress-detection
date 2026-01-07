# Stress detection based on social media posts

## A machine learning project applying Natural Language Processing (NLP)

The aim of this project is to apply various machine learning classification methods to text data. The model must distinguish between stress-positive and stress-negative posts. Specifically, it examines whether an LLM-based DistilBERT model performs better than traditional models. The final model accuracies are recorded in the Accuracies.csv file.

### Objectives
- Process messy text data (data_processing.ibynb)
- Learn and compare different embeddings and machine learning models for stress detection (experiements.ipynb)
- Visualize data and key findings (visualizations.ipynb)
- Visualize accuracies of the models (visualizations_results.ipynb)

### Required software
The following software must be installed to run the notebooks
- python 3
- numpy
- pandas
- matplotlib.pyplot
- sklearn
- gensim
- nltk


### Running instructions
Here are instructions for running the project. Note that training the transfromer takes a lot of time without GPU.
1. The datasets (4 in total) should be downloaded from [stress-detection](https://github.com/SenticNet/stress-detection) and moved to folder "data" in the root of the project.
2. Run notebook ***data_processing.ibynb***.
3. The cleaned data files (4 in total) should be in folder "cleaned_data".
4. Run notebook ***visualizations.ipynb***.
5. Run notebook ***experiements.ipynb***. Set variable ***is_train*** as True, if the transformed is not pretrained. The notebook will save the pretrained transformer in folder ***Transformer_backup***. 
6. The accuracies from experiements should be as csv file in the project root.
7. Run notebook ***visualizations_results.ipynb***