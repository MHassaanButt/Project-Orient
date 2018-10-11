# Orient 
*We Come Highly Recommended*

## Project description

Project Orient is a movie recommendation system where the attributes which determined the recommendations are not only explainable, but actually tunable for the individual consumer. Irrelevant recommendations waste not only the consumer's time but the company's money, but if we put the power of the recommendations in the hands of the user we have a win-win situation. The user is engaged in the platform, while the company is getting relevent data to create better future recommendations. Making the user feel that their time and choices are valued builds trust between a user and a platform and is key to a mutually beneficial relationship and secured success.

A Google slide presentation can be found here: [Orient](https://docs.google.com/presentation/d/1KM9ukOajZYONSRcKeBXup8pzwErsF-T0wbBDLuzR5Wc/edit?usp=sharing)

Example)

> *Here are the following factors that aided in us recommending you*: 
***Star Wars***
  
    Age: 25%
    Gender: 25%
    Occupation: 25%
    Location: 25%
	
> *"Would you like to tune these parameters?"*
> ***Yes***

    Base my movie recommendations on the following weighted factors:
    Age: 50%
    Gender: 0%
    Occupation: 25%
    Location: 25%
    

This system addresses the issues of recommendation algorithms creating negative feedback loops, and allows users to be aware of the profile they are building, and tune it to see the content that interests them.

## Requirements / Dependencies

	Python 2.7 or Python 3.6
	Pandas
	Click
	Scikit-learn 
	Keras (>= 2.0)

Scikit-learn requires:

    Python (>= 2.7 or >= 3.3)
    NumPy (>= 1.8.2)
    SciPy (>= 0.13.3)	

## Installation / Setup
Clone repository and update python path:
The easiest way to download + install this tutorial is by using git from the command-line:

	git clone https://github.com/AstronomerAmber/Project-Orient.git

	cd Project-Orient/

Create new development branch and switch onto it:

	git checkout -b $dev_test/9242018
	git push origin $dev_test/9242018
	
To run them, you also need to install sckit-learn. To install it:

    pip install scikit-learn
    
or (if you want GPU support):

    pip install scikit-learn_gpu

## Environment
I recommend creating a conda environoment so you do not destroy your main installation in case you make a mistake somewhere:

    conda create --name Orient_3.6 python=3.6 ipykernal
You can activate the new environment by running the following (on Linux):

    source activate Orient_3.6 
And deactivate it:

    source deactivate Orient_3.6 

## Build Environment
 Before running your Orient script:
 	Fill in the User x Movie matrix by running:
	
	python fill_user_matrix.py
	
This will build a Keras factorization model to predict previously unrated movies for users with embeddings. The resulting csv file:

	predicted_ratings.csv
	
Do not try and run:
	
	Word2Vec_occupations.py

Unless you would like to download Google's [Word2Vec](http://word2vec.googlecode.com/svn/trunk/) tool. It is not necessary for you to run this because the resulting csv file: Occupation_embeddings was provided to you in the repo.

## Liscensing
MovieLens Dataset [LICENSE](https://github.com/AstronomerAmber/Project-Orient/edit/master/LICENSE.md)
