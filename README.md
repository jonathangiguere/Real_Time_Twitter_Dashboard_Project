# Real_Time_Twitter_Dashboard_Project
Tool that takes a word as input from the user and dashboards information about tweets containing the word in real time.

## Motivation
I performed this project for a data mining class at the George Washington University.  My original idea for the project was to analyze tweets about the Washington Redskins, my favorite football team.  As I worked with Tweepy and the Twitter API, I realized I could let a user enter any keyword they wanted.  Information about tweets containing the user defined keyword is presented on a dashboard that can be updated for real time insights.  I used Tweepy, Plotly, and Pandas for the bulk of this project. 

## Using the Notebooks
First, go to https://developer.twitter.com/en/account/get-started to access your Twitter application's keys. Before running this notebook, these keys need to be pasted into the cell in 'DATS 6103 - Project 3 Streaming' titled "Connection to Twitter API". If you do not already have a Twitter Developer account or app, feel free to set up an account. Once you have an account and an app created, you can access the keys you need to run this notebook.

This project has two jupyter notebooks that work together. If you run all cells in 'DATS 6103 - Project 3 Streaming', you will be prompted to enter a tracked word to analyze. Once a tracked word is entered, this notebook will stream tweets containing the tracked word, and write them to a .csv file called 'OutputStreaming.csv'. After choosing your word, you can scroll to the bottom to see the tweets being streamed.

Running all cells in the second notebook, 'DATS 6103 - Project 3 Analysis.ipynb' reads the .csv file into a dataframe and performs the analysis. The end of this second file gives a dashboard showing real time information about Tweets containing the tracked word. One can keep running all cells in the 'DATS 6103 - Project 3 Analysis.ipynb' notebook to update the dashboard as new Tweets are constantly being streamed from this notebook.

## Other Files
To view streamed tweets at any point in time, open up 'OutputStreaming.csv'.  'us_states.csv' is just a list of states I use in the analysis file.  Finally, 'Project_Presentation.mp4' shows my walkthrough and presentation of the project.


