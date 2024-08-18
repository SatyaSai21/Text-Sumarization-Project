# Text Summarization using Transformers

# Project Title
# MODEL = `google/pegasus-cnn_dailymail`
Developed a robust text summarization project leveraging the Transformers library. 

The project focused on implementing state-of-the-art transformer models to generate concise summaries of large texts.


## API Reference
# Features :


# API Documentation: 
                  Interactive API documentation available at "/" when the server is running.


# Model Training: 
                  Train the text summarization model using the "/train" endpoint.


# Text Summarization: 
                  Summarize input text using the "/predict" endpoint.

## WHY TRANSFORMERS?
# Parallelization: Unlike RNNs and LSTMs, which process data sequentially, Transformers allow for parallel processing of data. This makes them significantly faster to train, especially on large datasets.

# Handling Long-Range Dependencies: RNNs and LSTMs struggle with capturing long-range dependencies due to the vanishing gradient problem. Transformers, with their self-attention mechanism, can capture dependencies between words regardless of their distance in the text, leading to more accurate and context-aware summaries.

# Attention Mechanism: The self-attention mechanism in Transformers allows the model to focus on relevant parts of the input text when generating summaries, leading to more coherent and contextually appropriate outputs.

## workflow

Update config.yaml

Update param.yaml

Update entity

Update the configuration manager in src config

Update the components

Update the pipeline

Update the main.py

Update the app.py

## Metrics
# ROUGE-1: Measures the overlap of unigrams (single words) between the reference summary and the generated summary.

# ROUGE-2: Measures the overlap of bigrams (two consecutive words) between the reference and generated summaries.

# ROUGE-L: Focuses on the longest common subsequence (LCS) between the reference and generated summaries, considering sentence-level structure.

# ROUGE-LSum: A variant of ROUGE-L, specifically tailored for summarization, comparing the LCS at the summary level.

    MODEL :
        pegasus :

            rouge1	    rouge2	    rougeL	    rougeLsum

	        0.023872	0.0	        0.023786	0.023879
