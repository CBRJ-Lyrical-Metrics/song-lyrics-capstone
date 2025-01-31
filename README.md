A LYRICAL EVOLUTION: 

An Investigation of the Cultural Lexicon of U.S. Popular Music from 1958 - Present

#### [Final Slide Presentation](https://www.canva.com/design/DAFCXoeG7z0/jNCtQkQFqyOTWS5Ckg8Xuw/view?utm_content=DAFCXoeG7z0&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
===
        
Team Members: Jerry Nolf, Rachel Robbins-Mayhill, Ben Smith, Chris Teceno  |   Codeup   |   Innis Cohort   |   June 2022
 
===


 <img src='Drafts/dataset-cover.png' width="1200" height="250" align="center"/>


===



Table of Contents
---
 
* I. [Project Overview](#i-project-overview)<br>
[1. Goal](#1-goal)<br>
[2. Description](#2-description)<br>
[3. Formulating Hypotheses](#3-formulating-hypotheses)<br>
[4. Initial Questions](#4-initial-questions)<br>
[5. Key Findings](#5-key-findings)<br>
[6. Deliverables](#6-deliverables)<br>
* II. [Project Data Context](#ii-project-data-context)<br>
[1. Data Dictionary](#1-data-dictionary)<br>
* III. [Project Plan - Data Science Pipeline](#iii-project-plan---using-the-data-science-pipeline)<br>
[1. Project Planning](#1-plan)<br>
[2. Data Acquisition](#2-acquire)<br>
[3. Data Preparation](#3-prepare)<br>
[4. Data Exploration](#4explore)<br>
[5. Modeling & Evaluation](#5-model--evaluate)<br>
[6. Product Delivery](#6-delivery)<br>
* IV. [Project Modules](#iv-project-modules)<br>
* V. [Project Reproduction](#v-project-reproduction)<br>
 
 
 
## I. PROJECT OVERVIEW

#### 1. GOAL:
This project aimed to investigate the patterns of song lyrics across decades by applying Natural Language Processing techniques including Topic Modeling and Sentiment Analysis, while using a Kaggle data set of the Billboard Top 100 Songs from 1958 - Present and lyrics pulled from the Genius.com API. We believe the lyrics of popular songs could be used for historical analysis using exploratory methods to identify changing societal trends in relationships, sexuality, and vulgarity. Furthermore, we beleive we can predict the decade the song appeared on the Top 100 using features and machine learning methods.
 
 
#### 2. DESCRIPTION:

Songs are powerful tokens: they can soothe, validate, ignite, confront, and educate us – among other things. Like time capsules, they are captured for eternity. The slang and language used are often indicative of the times, and you can probably recall exactly when a song was made based on what is mentioned. Arguably, music is a catalyst for societal and cultural evolution like no other art form. It has been causing controversy and societal upheaval for decades, and it seems with every generation there’s a new musical trend that has the older generations shaking their heads. 

For centuries, songs have been passed down through generations, being sung as oral histories. However, with advancements of the 20th century, technology has made the world of music a much smaller place and, thanks to cheap, widely-available audio equipment, songs are now distributed on a much larger scale, having a farther-reaching impact, and a more permanent place in history. 

This project aimed to combine the record of lyrical history and technological advancements to evaluate the changes in the societal lexicon over the last 60+ years. Using machine learning and natural language processing methodologies we investigated the topics prevalent in songs of the past, predicted the decade in which they were written, and conducted historical analysis through exploration to identify changing societal trends in relationships, sexuality, and vulgarity.

To do this, we acquired a [Kaggle](https://www.kaggle.com/datasets/dhruvildave/billboard-the-hot-100-songs) data set of the Billboard Top 100 Songs from its inception in 1958 to present. We then utilized the [Genius.com](https://genius.com/) API and LyricGenius Library to conduct web scraping to pull the lyrics for the specified songs which became the corpus for this project. The acquired data can be easily accessed via this [Google Drive .csv file](https://drive.google.com/file/d/1S0dJ7-5x8NIgt1LranE3UETgl_JvukGT/view).

After acquiring and preparing the corpus, our team conducted time series analysis and natural language processing exploration utilizing methods such as sentiment analysis and topic modeling. We also employed multiclass classification methods to create multiple machine learning models. The end goal was to create an NLP model that accurately predicted the decade a song first appeared on the Billboard Top 100 chart, based on the words found in the lyrics of the song.

We choose the Billboard Hot 100 song list as a focus because it is the music industry standard record chart in the United States for song popularity, published weekly by Billboard magazine. It provides a window into popular culture at a given time, by providing chart rankings of songs that were trending on sales, airplay, and now streaming for that week in the United States. It is arguably the best historical record of the impact of specific popular songs over time.



#### 3. FORMULATING HYPOTHESES
The initial hypothesis of this project was that we could use the top songs of each decade in conjunction with topic modeling and sentiment analysis to identify lyric features that would accurately predict the decade a song was on the Billboard Top 100 using machine learning. The thought behind this was that popular songs have been the historians of a unique lexicon, specific to their place in time. We believe the lyrics of popular songs could be analyzed through machine learning to identify societal trends in relationships, sexuality, and vulgarity.


#### 4. INITIAL QUESTIONS:
The focus of the project is on identifying the decade a song first appeared on the Billboard Top 100. Below are some of the initial questions this project looks to answer throughout the Data Science Pipeline.
 
 
##### Data-Focused Questions
- How does sentiment within lyrics change over time?
- Is there a correclation between sentiment and the time a song was popular?
- Is there a correlation between events in history and sentiment of lyrics?
- What topics are most prevalent across the decades?
- How do topics within lyrics change over time?
- Is there a correlation between topics and the time a song was popular?
 
  
#### 5. KEY FINDINGS:
The key findings for this presentation are available in slide format by clicking on the [Final Slide Presentation](https://www.canva.com/design/DAFCXoeG7z0/jNCtQkQFqyOTWS5Ckg8Xuw/view?utm_content=DAFCXoeG7z0&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton).

Exploration revealed US popular music has undergone a major cultural shift starting in the 90's, where:

- Overall sentiment decreased
- Lyrics became more complex
- Topics shifted towards sex, money, & violence
- ‘Love’ was replaced with ‘Like’

Ultimately, our hypothesis that we could use the top songs of each decade to accurately predict the decade a song was on the Billboard Top 100 was true. Although, certain decades were predicted more accurately than others. Our best performing models were based heavily on TF/IDF with the top performing model being a Logistic Regression model with an F-1 score that was 220% over baseline.
 
#### 6. DELIVERABLES:
- [x] README file - provides an overview of the project and steps for project reproduction
- [x] Draft Jupyter Notebook - provides all steps taken to produce the project
- [x] .py modules - provide reproducible code to automate acquiring, preparing, splitting, exploring, and modeling the corpus
- [x] Final Jupyter Notebook - provides presentation-ready acquire, prepare, exploration, modeling, and summary
- [x] Slide Deck - includes executive summary, takeaways, and explanation of key insights from each step of the Data Science Pipeline
- [x] One-Page Handout - provides overview and summary of project process and outcome
- [x] 10 Minute Presentation 

 
## II. PROJECT DATA CONTEXT
 
#### 1. DATA DICTIONARY:
The final DataFrame used to explore the corpus for this project contains the following variables (columns).  The variables, along with their data types, are defined below:
 
 
|  Variables             |    Definition                              |    Data Type             |
| :--------------------   | :---------------------------------------- | :-------------------- |
title                     |Title of song listed on Billboard Top 100 Chart        |object
artist                    |Vocalist who performed song                            |object
date                      |Date the song FIRST appeared on the Billboard Top 100  |date time
lyrics                    |The lyric contents cleaned with prep_data function     |object
raw_lyrics                |The contents of scraped song lyrics without cleaning   |object
**decade (target)**       |The decade the song was FIRST listed on the Billboard Top 100  |integer
character_count*          |The number of characters within the cleaned document   |integer
word_count*               |The number of words within the cleaned document        |integer
unique_words*             |A list of the unique words in the cleaned document     |object
unique_word_count*        |The number of unique words in the cleaned document     |integer
sentiment*                |Score between -1.0 (negative) and 1.0 (positive) indicating overall emotional leaning of lyrics      |float
sentiment_category*       |Categorical category based upon sentiment score: very negative, somewhat negative, nuetral, somewhat positive, very positive   |object
place_words*              |A list of song part identifiers in the lyrics          |object
chorus_count*             |The number of choruses in the song                     |integer
verse_count*              |The number of unique words in the cleaned document     |integer
verse_chorus_ratio*       |The ratio of verses to choruses                        |float
pre_chorus_count*         |The number of pre-choruses in the song                 |integer
outro_count*              |The number of outros in the song                       |integer
bridge_count*             |The number of bridges in the song                      |integer
hook_count*               |The number of hooks in the song                        |integer
bigrams*                  |A list of bigrams in the cleaned document              |object
trigrams*                 |A list of  trigrams in the cleaned document            |object

\* feature engineered
 
## III. PROJECT PLAN - USING THE DATA SCIENCE PIPELINE:
The following outlines the process taken through the Data Science Pipeline to complete this project. 
 
Plan➜ Acquire ➜ Prepare ➜ Explore ➜ Model & Evaluate ➜ Deliver
 
<details><summary>EXPAND PLAN STEPS</summary><br/> 
 
#### 1. PLAN
- [x]  Create an organizational tool for tracking project completion through the data science pipeline using [Trello](https://trello.com/b/hfrfjZ6Q/teamflow-process)
- [x]  Review project expectations
- [x]  Draft project goal to include measures of success
- [x]  Clarify questions related to the project
- [x]  Create exploratory questions related to the corpus
- [x]  Draft starting hypothesis
- [X]  Add all planning and project breakdown tasks to the organizational tool
</details>

<details><summary>EXPAND ACQUIRE STEPS</summary><br/>  
    
#### 2. ACQUIRE
- [x]  Create .gitignore
- [x]  Obtain API token from [Genius.com](https://genius.com/) 
- [x]  Create env file and store the Genius token within
- [x]  Store env file in .gitignore to ensure the security of sensitive data
- [x]  Obtain Billboard Top 100 Song list from [Kaggle](https://www.kaggle.com/datasets/dhruvildave/billboard-the-hot-100-songs) 
- [x]  Pip Install [LyricsGenius](https://pypi.org/project/lyricsgenius/)
- [x]  Create acquire.py module
- [x]  Store functions needed to acquire the lyric documents to make up the corpus
     - [x] Pull artist and song title from Kaggle dataset
     - [x] Run through Lyrics Genius to obtain lyrics 
     - [x] Store as.csv     
- [x]  Ensure all imports needed to run the acquire functions are inside the acquire.py document
- [x]  Using Command Line / Terminal, run ‘python acquire.py’ to create the `songs_0526.csv` file that contains the corpus
- [x]  Using Jupyter Notebook or other Python Scripting Program
     - [x]  Run all required imports
     - [x]  Import functions for acquiring the corpus from acquire.py module
     - [x]  Obtain the original size of the corpus
</details>
     
<details><summary>EXPAND PREPARE STEPS</summary><br/>   
    
#### 3. PREPARE
Using Jupyter Notebook
- [x]  Acquire corpus using functions from the acquire.py module or by utilizing the [Google Drive .csv](https://drive.google.com/file/d/1S0dJ7-5x8NIgt1LranE3UETgl_JvukGT/view) 
- [x]  Summarize corpus using methods and document observations
- [x]  Clean documents/corpus
   - [x] Make all text lowercase
   - [x] Normalize, encode, and decode to remove accented text and special characters
   - [x] Remove stopwords  
   - [x] Lemmatize words to acquire base words
   - [x] Convert date to DateTime format
   - [x] Expand contractions to include the full word/meaning
   - [x] Remove song part identifiers ('verse', 'chorus', etc.)
- [x]  Address missing values, data errors, unnecessary data, renaming
- [x]  Conduct feature engineering to create features to explore and feed into the model
   - [x] Add: Decade, Chorus Count, Verse Count, Verse/Chorus Ratio, Word Count, Unique Words per Song, Unique Words per Decade, Bigrams, and Trigrams
   - [x] Conduct Topic Modeling using Latent Dirichlet Allocation (LDA) to extract main topics from the corpus 
   - [x] Conduct Sentiment Analysis using Natural Language Toolkit to determine positive, negative, and neutral sentiment
- [x]  Create a data dictionary framework to define final variables and data context
- [x]  Split corpus into train, validate, and test samples prior to modeling 
Using Python Scripting Program (Jupyter Notebook)
- [x]  Create prepare functions within prepare.py
- [x]  Store functions needed to prepare the Lyrics Corpus such as:
   - [x]  Cleaning Function: to normalize text and remove accented and special characters
   - [x]  Lemmatize Function: to acquire lexicographically correct root words
   - [x]  Stopwords Function: to remove meaningless words
   - [x]  Engineered Features Functions: to add desired features, topics, and sentiment
   - [x]  Split Function: to split the corpus prior to modeling if using features
   - [x]  Get_data Function: combines all above functions    
- [x]  Ensure all imports needed to run the prepare functions are added to the prepare.py document
</details>

<details><summary>EXPAND EXPLORE STEPS</summary><br/> 
    
#### 4.EXPLORE
Using Jupyter Notebook:
- [x]  Document key questions about hypotheses 
- [x]  Create visualizations with the intent to discover variable relationships
     - [x]  Identify variables related to decade of lyrics
     - [x]  Identify any potential data integrity issues
- [x]  Document findings
- [x]  Summarize conclusions, provide clear answers, and summarize takeaways
     - [x] Explain plan of action as deduced from work to this point    
- [x]  Create explore functions within explore.py
- [x]  Store functions needed to explore the Lyrics Corpus in explore.py
- [x]  Ensure all imports needed to run the explore functions are added to the explore.py document
</details>

<details><summary>EXPAND MODEL & EVALUATE STEPS</summary><br/>  
    
#### 5. MODEL & EVALUATE
Using Jupyter Notebook:
- [x]  Establish baseline accuracy
- [x]  Create two types of dataframes to run through models (TF-IDF, and Feature Engineering)
- [x]  Train and fit multiple (1000+) models with varying algorithms and/or hyperparameters
- [x]  Compare evaluation metrics across models
- [x]  Remove unnecessary features
- [x]  Evaluate best performing models using validate set
- [x]  Choose best performing validation model for use on test set
- [x]  Summarize performance
- [x]  Interpret and document findings
- [x]  Create and store functions needed to model the Lyrics Corpus in model.py
- [x]  Ensure all imports needed to run the model functions are added to the model.py document
</details> 

<details><summary>EXPAND DELIVERY STEPS</summary><br/>  
    
#### 6. DELIVERY
- [x]  Prepare a presentation using Canva to document data science pipeline process and findings
     - [x]  Include an introduction of the project and goals
     - [x]  Provide an executive summary of findings, key takeaways, recommendations, and next steps
     - [x]  Create a walkthrough of the acquisition, preparation, exploration and modeling processes 
     - [x]  Include presentation-worthy visualizations that support exploration and modeling
     - [x]  Provide final takeaways, recommend a course of action, and next steps
- [x]  Prepare final notebook in Jupyter Notebook
     - [x]  Create clear walk-through of the Data Science Pipeline using headings and dividers
     - [x]  Explicitly define questions asked during the initial analysis
     - [x]  Visualize relationships
     - [x]  Document takeaways
     - [x]  Comment code thoroughly
</details>


 
 
## IV. PROJECT MODULES:
- [x] acquire.py - provides reproducible python code to automate acquisition 
- [x] prepare.py - provides reproducible python code to automate cleaning, preparing, and splitting the corpus
- [x] explore.py - provides reproducible python code to automate exploration and visualization
- [x] model.py - provides reproducible python code to automate modeling and evaluation
  
## V. PROJECT REPRODUCTION:

<details><summary> EXPAND REPRODUCTION STEPS </summary><br/> 

- [X] There are 2 options to acquire the data in order to reproduce the project.
     - [x] 1. Download the .csv file of the song title, artist, lyrics, and date the song first appeared on the Top 100 through [Google Drive](https://drive.google.com/file/d/1S0dJ7-5x8NIgt1LranE3UETgl_JvukGT/view)    
     - [x] 2. Create an env.py file that will contain access credentials to the Genius API.
        - [x] Follow directions at [Genius](https://docs.genius.com/#/authentication-h1) to generate an API personal access token to gain access to the contents within the Genius API.
        - [x] Save the token in your env.py file under the variable `api_token`
        - [x] Make .gitignore and confirm .gitignore is hiding your env.py file
        - [x] Store that .gitignore and env file locally in the repository
        - [x] Run the acquire.py modules
- [x] Clone our repo (including all .py modules)
- [x] Import supporting resources and python libraries:  pandas, matplotlib, seaborn, plotly, numpy, sklearn, scipy, nltk, contractions, json, re, unicodedata, unidecode, and lyricsgenius 
- [x] Follow steps as outlined in the README.md. and work.ipynb
- [x] Run Final_Report.ipynb to view the final product
</details>

Resource Note: 
Vader Sentiment Analysis Tools: 
Hutto, C.J. & Gilbert, E.E. (2014). VADER: A Parsimonious Rule-based Model for
Sentiment Analysis of Social Media Text. Eighth International Conference on
Weblogs and Social Media (ICWSM-14). Ann Arbor, MI, June 2014.