# Reddit Text Analysis with Machine Learning

This project demonstrates advanced text analysis and sentiment classification on Reddit data using machine learning techniques and Large Language Models (LLMs). The work combines API-based data collection, manual annotation, automated text classification, and subreddit selection strategies to analyze public opinion and stance detection on social media.

## Project Overview

This repository contains a comprehensive text mining pipeline that collects Reddit posts, performs stance detection, and compares multiple classification approaches including traditional machine learning, manual coding, and state-of-the-art Large Language Models. The project explores how different automated methods compare to human annotation in understanding public sentiment and positions expressed in social media discussions.

## Repository Contents

### Main Analysis Files

**MLtexttutorial.Rmd**
R Markdown document implementing machine learning text classification pipeline. This tutorial covers:
* Text preprocessing and feature extraction
* Training supervised learning models for text classification
* Model evaluation and performance comparison
* Visualization of classification results

**Reddit.qmd**
Quarto document for Reddit data collection and initial analysis:
* Reddit API authentication and data extraction
* Subreddit content scraping
* Post filtering and data cleaning
* Initial exploratory data analysis

**Subreddit_Selection.qmd**
Subreddit selection methodology and justification:
* Criteria for choosing relevant subreddits
* Community analysis and topic relevance
* Data availability assessment
* Sampling strategy documentation

### Data Files

**handcode.CSV**
Manually coded stance labels for Reddit posts serving as ground truth:
* Human annotated sentiment classifications
* Stance labels (support, oppose, neutral)
* Reference standard for model validation

**stance_with_LLM.csv**
Large Language Model predictions on the same dataset:
* LLM-generated stance classifications
* Confidence scores for predictions
* Comparison baseline for traditional ML approaches

### Rendered Outputs

**MLtexttutorial.nb.html**
HTML notebook with executed code and visualizations from the ML tutorial, providing an interactive view of the analysis workflow.

**Reddit.html**
Rendered Reddit analysis with embedded plots and results, showcasing the complete data collection and preprocessing pipeline.

### Supporting Directories

**MLtexttutorial_cache/latex/**
Cached computation results for faster document rendering, storing intermediate analysis outputs.

**MLtexttutorial_files/figure-latex/**
Generated figures and plots from the ML analysis in LaTeX-compatible format for publication-ready visualizations.

**Reddit_files/libs/**
JavaScript libraries and dependencies for interactive HTML output, enabling dynamic visualizations in rendered documents.

### Project Configuration

**SURV-622-Assignment-2.Rproj**
RStudio project file maintaining workspace settings and file paths for reproducible analysis.

**.gitignore**
Version control exclusions for temporary files and sensitive data, ensuring clean repository management.

## Research Approach

### Data Collection Strategy

The project employs Reddit's API to collect posts from carefully selected subreddits relevant to the research question. The selection process considers:
* Topic relevance and community activity levels
* Discussion quality and user engagement patterns
* Temporal coverage and data availability
* Diversity of perspectives and viewpoints

### Annotation Methodology

Two parallel annotation approaches provide comparative insights:

**Manual Coding**
Human annotators classify posts based on stance toward specific topics, creating a gold standard dataset for validation. This process captures:
* Nuanced understanding of context and sarcasm
* Complex argument structures
* Cultural references and implicit meanings

**LLM Classification**
Large Language Models automatically classify the same posts, enabling:
* Scalable analysis of large datasets
* Consistency in classification criteria
* Rapid processing of new data

### Machine Learning Pipeline

The ML tutorial demonstrates a complete text classification workflow:

**Text Preprocessing**
* Tokenization and normalization
* Stop word removal
* Stemming or lemmatization
* Feature extraction (TF-IDF, word embeddings)

**Model Training**
* Multiple classification algorithms (e.g., Naive Bayes, SVM, Random Forest)
* Cross-validation for robust performance estimation
* Hyperparameter tuning for optimal results

**Evaluation Metrics**
* Accuracy, precision, recall, F1-score
* Confusion matrices for error analysis
* Comparison with human annotations
* Agreement analysis between ML and LLM approaches

## Skills Demonstrated

**API Integration**
* Reddit API authentication and rate limit handling
* Efficient data extraction and pagination
* Error handling and data validation

**Text Mining and NLP**
* Natural language preprocessing techniques
* Feature engineering for text data
* Sentiment and stance detection
* Large Language Model integration

**Machine Learning**
* Supervised learning for text classification
* Model training and validation
* Performance evaluation and comparison
* Interpretation of classification results

**Data Analysis**
* Exploratory data analysis of social media content
* Statistical comparison of annotation methods
* Visualization of text analysis results
* Reproducible research practices

**Programming and Tools**
* R programming for data science
* Quarto and R Markdown for literate programming
* RStudio for project management
* Version control with Git

## Use Cases

This project methodology applies to:
* Social media monitoring for public opinion research
* Brand sentiment analysis from online discussions
* Political stance detection in social media
* Content moderation and toxicity detection
* Market research through community analysis
* Crisis communication monitoring

## Methodological Contributions

**Comparative Evaluation**
The project uniquely compares three classification approaches (manual, ML, LLM) on identical data, providing insights into:
* Strengths and limitations of each method
* Cost-benefit tradeoffs between approaches
* Scalability versus accuracy considerations

**Reproducible Workflow**
All analysis steps are documented in executable notebooks, enabling:
* Transparent research practices
* Replication by other researchers
* Adaptation to new research questions
* Educational use for learning text mining

## Technical Requirements

**R Packages**
* tidyverse: Data manipulation and visualization
* tidytext: Text mining framework
* quanteda: Quantitative text analysis
* caret or tidymodels: Machine learning workflows
* RedditExtractoR or related: Reddit API access

**Python Libraries (if LLM integration uses Python)**
* openai or huggingface: LLM API access
* pandas: Data manipulation
* requests: API calls

## Research Context

This work was completed as part of SURV 622 (Advanced Data Collection Methods) at the University of Michigan, demonstrating practical application of:
* Digital data collection techniques
* Text analysis methods for survey research
* Integration of traditional and modern NLP approaches
* Ethical considerations in social media research

## Ethical Considerations

The project follows ethical guidelines for social media research:
* Use of publicly available Reddit posts only
* No collection of personally identifiable information
* Compliance with Reddit's Terms of Service and API guidelines
* Respect for community norms and user privacy
* Transparent reporting of data sources and methods

## Learning Outcomes

Through this project, key competencies developed include:
* Designing and implementing API-based data collection
* Applying machine learning to text classification tasks
* Evaluating and comparing multiple classification methods
* Working with Large Language Models for NLP tasks
* Creating reproducible analysis workflows
* Documenting research methods transparently

## Future Extensions

Potential enhancements to this work could include:
* Expanding to additional subreddits for broader coverage
* Incorporating temporal analysis of stance evolution
* Fine-tuning LLMs on domain-specific data
* Multi-label classification for complex stances
* Network analysis of discussion patterns
* Real-time monitoring dashboard

This repository serves as both a practical demonstration of modern text analysis techniques and a template for similar social media research projects.
