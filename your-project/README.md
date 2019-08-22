<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Final project: Speech analyser
*[Javier Pardo Sánchez]*

*[Data Analytics, IronHack Barcelona 16/08/19]*

## Content
- [Project Description](#project-description)
- [Hypotheses / Questions](#hypotheses-/-questions)
- [Dataset](#dataset)
- [Cleaning](#cleaning)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [Workflow](#workflow)
- [Organization](#organization)
- [Links](#links)

<a name="project-description"></a>

## Project Description

My project uses speech recognition API and self made NLP to analyse different audio files and tell if they have a positive or negative message. It has a lot of applications from marketing strategy to business intelligence and customer service, and all of that without any kind of improvement. However if improved, it could be even more useful.

<a name="hypotheses-/-questions"></a>

## Hypotheses / Questions
* How useful can it be to apply NLP with speech recognition?
* Will it be effective?

<a name="dataset"></a>

## Dataset
* The dataset has been collected by the Stanford univeristy, and has been uploaded to kaggle (one of the most important data science communities to get datasets). It contains around 50.000 film reviews from IMDB splitted into two groups, train and test. Half of the reviews are positive while the other half are negative, they are also ordered like that (0-12499 / 12500-25000) so they're just lists of objects

- [Dataset](https://www.kaggle.com/iarunava/imdb-movie-reviews-dataset)


<a name="cleaning"></a>

## Cleaning
The cleaning of my dataset was a string cleaning, understanding each review as a string itself, so we can wheter see if the result is positive or negative. For that reason, I removed all the punctuation signs, transformed all to lowercase and eliminate html code (some of the strings had that problem). I also vectorized those reviews to a matrix for each word to give it a relevance and a punctuation.

<a name="model-training-and-evaluation"></a>

## Model Training and Evaluation
* The training model was a simple logistic regression. so I splitted the train dataset (25000 'rows') into training (75%) and testing (25%) part so I can have a good not overfitted model

<a name="conclusion"></a>

## Conclusion
* With an accuracy of almost 90% (without being overfitted) we can say that the model isn't bad at all, still there is room to improve. 

<a name="future-work"></a>

## Future Work
* Not just positive or negative, but neutral 
* Add a scale 
* Use a self made speech recognition program

<a name="workflow"></a>

## Workflow

First, I had to research about the topic and once this was done,  after a few trials I found a good dataset prepared for training these kind of models.

After I needed to take a look at it so I could check if I had to clean it (what I did inded)

Once I had the resources, I did the modeling and the trials to see the accuracy of the model

Last I created the speech connection to google API and merge both of them to create the final program. The workflow is explained better in the jupyter notebook files

<a name="organization"></a>

## Organization
For the organization part I used trello, which you can find below

<a name="links"></a>

## Links

[Repository](https://github.com/Javier-13/Project-Week-8-Final-Project)  
[Slides](https://docs.google.com/presentation/d/1CaMN39RNW6sXVOynOEQ4kUPEtQfFFFHnsq6zMTtkAaI/edit?usp=sharing)  
[Trello](https://trello.com/invite/b/wx9mKXRS/812c72bb3f1fb29e7eac5e942a881f49/project-5-speech-analyser)
