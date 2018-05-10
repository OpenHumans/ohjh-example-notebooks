# Meet the *Personal Data Notebooks* on *Open Humans*

The [*Personal Data Notebooks* on *Open Humans*](https://www.openhumans.org/activity/personal-data-notebooks/) allow you to explore and analyze your personal data that's stored in your *Open Humans* account right in your web browser. Our Director of Research, Bastian Greshake Tzovaras, [has written about how this can help bridging our growing divide between people and algorithms](http://ruleofthirds.de/demystifying-algorithms/). *[If you've come here because of the presentation at the Sage Assembly: this is literally just that talk as a blog post]*.

Below you will find a step-by-step guide with how to get started with the *Personal Data Notebooks* and some more information about the example notebooks we already provide.

## Table of Contents
- [Meet the *Personal Data Notebooks* on *Open Humans*](#meet-the-personal-data-notebooks-on-open-humans)
* [Getting started](#getting-started)
+ [Setting up your *Open Humans* account](#setting-up-your-open-humans-account)
+ [Start your *Personal Data Notebook*](#start-your-personal-data-notebook)
* [Example Notebooks](#example-notebooks)
+ [Analyze your physical activity](#analyze-your-physical-activity)
  - [`exploring_notebooks_fitbit.ipynb`](#exploring_notebooks_fitbitipynb)
  - [`compare_fitbit_healthkit.ipynb`](#compare_fitbit_healthkitipynb)
+ [Analyze your Tweets](#analyze-your-tweets)
  - [`twitter-sentiment.ipynb`](#twitter-sentimentipynb)
  - [`twitter-archive-text-mining-R.ipynb`](#twitter-archive-text-mining-ripynb)
+ [Analyze your *Moves* GPS data](#analyze-your-moves-gps-data)
  - [`moves-analysis.ipynb`](#moves-analysisipynb)
+ [Made your own?](#made-your-own)

## Getting started

### Setting up your *Open Humans* account
1. [Create an account with Open Humans](https://www.openhumans.org/account/signup/) or [log in into your existing account](https://www.openhumans.org/account/login/). If you have just created your account you will need to verify your email address before you can continue with the next steps.
2. Connect some data sources to your *Open Humans* account. While we have a lot of interesting data sources, our example Notebooks work with one or multiple of the following data sources (note, by default **none** of the uploaded/connected data will be made public):
  - [Fitbit](https://www.openhumans.org/activity/fitbit)
  - [Apple HealthKit](https://www.openhumans.org/activity/open-humans-healthkit-integration/)
  - [Twitter archives](https://www.openhumans.org/activity/twitter-archive-analyzer/)

### Start your *Personal Data Notebook*
You can now head to [https://notebooks.openhumans.org](https://notebooks.openhumans.org) and click on `Sign in with OpenHumans`.
<center><img src='notebook-login-1.gif' width='500'/></center>

This will take you back to the main *Open Humans* page where you have to authorize the notebooks to get access to the data in your *Open Humans* account. Click on `Authorize project` to continue.

<center><img src='notebook-login-2.gif' width='500'/></center>

This will take you to the main page of the *Personal Data Notebooks* where your personal notebook server will boot up.

**All the steps that you have taken above are only needed for the initial setup of your *Personal Data Notebooks*. From here on you can just head to [https://notebooks.openhumans.org](https://notebooks.openhumans.org)**

You are now ready to open up one of the notebooks and run it right on your personal data!

**After opening a notebook you will see that the code in the notebooks is organized into *cells*. To run a cell you can click the `Run` button in the menu bar or press `<SHIFT> + <ENTER>` on your keyboard. Repeat this to go through each cell in the notebook.**

<center><img src='fitbit-image.gif' width='500'/></center>

If this is your first time using *Jupyter Notebooks* (how exciting! 🎉) you might want to read a brief tutorial on the [Notebook Basics](http://nbviewer.jupyter.org/github/jupyter/notebook/blob/master/docs/source/examples/Notebook/Notebook%20Basics.ipynb) and [How-to execute/run code in Notebooks](http://nbviewer.jupyter.org/github/jupyter/notebook/blob/master/docs/source/examples/Notebook/Running%20Code.ipynb)


## Example Notebooks
We have a collection of example notebooks that should already be available in the root of your notebook directory. But you can also [download the raw notebooks from GitHub](https://github.com/OpenHumans/ohjh-example-notebooks).

These are notebooks should give you an idea of how the notebooks work, along with a description of the analysis they perform and example output (done on the data of [Bastian](https://www.twitter.com/gedankenstuecke)). You can run these right on your own data.

### Analyze your physical activity
We have two example notebooks that you can use to dive into your activity tracking data from Fitbit and Apple Healthkit.

#### `exploring_notebooks_fitbit.ipynb`
The [`exploring_notebooks_fitbit.ipynb` notebook](https://github.com/OpenHumans/ohjh-example-notebooks/blob/master/exploring_notebooks_fitbit.ipynb) gives you a very simple idea of what the Notebooks can do. It uses basic Python commands to analyze and plot step and heart rate data from Fitbit. As such you only need to have your Fitbit account connected to your *Open Humans* account in oder to use it.

It also gives a basic idea of how to see whether Fitbit's gamification actually works and how to spot it in the data. Does gamification work for you too?

#### `compare_fitbit_healthkit.ipynb`
[`compare_fitbit_healthkit.ipynb`](https://github.com/OpenHumans/ohjh-example-notebooks/blob/master/compare_fitbit_healthkit.ipynb) is for those dedicated to do Quantified Self with both Fitbit and an Apple Watch/iPhone. It takes data out of both your *HealthKit* import and your *Fitbit* to see how well the steps counted by both methods align. Along the description of the notebook you will find all the Python code you'll need to get started.

And if you're also wearing an Apple Watch along with a Fitbit you'll be in for a surprise.

### Analyze your Tweets
<center><img src='header-image.gif' width='500'/></center>

For the social media addicts we have two example Notebooks that can be used to do some analysis of your Twitter archive.

#### `twitter-sentiment.ipynb`
In [`twitter-sentiment.ipynb`](https://github.com/OpenHumans/ohjh-example-notebooks/blob/master/twitter-sentiment.ipynb) you will find a very simple sentiment analysis as performed in Python. It visualizes your polarity (are your tweets having a positive or negative sentiment overall) and your subjectivity over time.

And since this is 2018 it also contains an analysis that highlights your most-used emoji along with a sentiment classification based on this, rather than on pure text. 😍

#### `twitter-archive-text-mining-R.ipynb`
In [`twitter-archive-text-mining-R.ipynb`](https://github.com/OpenHumans/ohjh-example-notebooks/blob/master/twitter-archive-text-mining-R.ipynb) you can find an example of how you can use `R` to do text mining. It uses a very simple approach that splits tweets in more *historic* and *current* ones and from this identifies words which are over/underrepresented in these two categories, along you to find out which words/topics have become more/less important for you over time.

A similar approach is used to associate emojis with topics. ✈️🎉

### Analyze your *Moves* GPS data
<center><img src='moves-analysis.gif' width='500'/></center>

*Moves* is an app for iOS and Android that records your GPS location throughout the day and it also tries to classify your modes of transportation. You can use this data to find out how you travel the globe, to see how you much you walk around etc.

#### `moves-analysis.ipynb`
The [`moves-analysis.ipynb`](https://github.com/OpenHumans/ohjh-example-notebooks/blob/master/moves-analysis.ipynb) notebook uses your data from *Moves* to do two things:
1. It takes your historical daily GPS tracks to find out where you have been on that day. This location is then used to request the local weather on that date from the *Dark Sky* weather API service.
2. It grabs your daily walking distance & step counts.

The step counts & daily weather are then used to correlate your daily activity with the weather records, investigating how much your physical activity depends on the local outdoor temperature and rainfall/snow conditions.

### Made your own?
You made your own *Personal Data Notebook* and think it would be a great example for other people? Please be in touch with Bastian at bastian@openhumans.org. Or if you're a GitHub person: [Make a pull request against our Example Notebook repository](https://github.com/OpenHumans/ohjh-example-notebooks).
