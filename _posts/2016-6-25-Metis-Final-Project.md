---
layout: post
title: Metis Final Project
---

This post is in regards to my final project for Metis Data Science Bootcamp, presented at our career day on Thursday, June 23, 2016. My project was called "Breaking the Habit", and details my efforts to create a playlist generator for Spotify that would specifically recommend music that is **unlike** what you normally listen to.

This final project represents an important breakthrough in my way of thinking, in that I could come up with an interesting idea by just asking myself what I would want to see in my experience of Spotify, whereas other projects seemed more motivated by browsing data sets and **then** trying to form a data science question out of them.

The technical aspects of the project were surprisingly simple, it was a matter of understanding the Spotify Web API well enough to be able to properly create a function over it, that pulled specific data from one API endpoint and then applied an algorithm to determine how that information would be fed into another API endpoint. I gathered information about the audio features of my saved tracks on Spotify (the "danceability", "loudness", "valence", "acousticness", etc., generally normalized as a value between 0.0 and 1.0), the genres I listened to, and even the popularity of the music I listen to. Once I knew what genres and audio feature values I tended to listen to most and least, I could ask Spotify's Seed Recommendation endpoint to give me music in genres I listened to a lot, occasionally, or never before, as well as songs with audio feature values closer to what I listened to before, or unlike what I listened to before.

Where my Discover Weekly playlist gives me a lot of cool and interesting selections more or less in the gist of "alternative rock" with a few surprises, the "Breaking the Habit" playlist ended up giving me, in the first few songs, Alternative Rock, Norwegian Death Metal, EDM, Bluegrass, and Brazilian Rock. The goal was not necessarily to give me only music I would like (otherwise it wouldn't have bothered giving me Tim McGraw), but to make it easier for me to find music outside my comfort zone, since there are only so many hours in the day that I can research every random genre in existence to find something that would genuinely be out of the blue for me.

This project does not have any fancy machine learning, no big data, no NLP, but it does demonstrate that good data science is ultimately just about finding intelligent ways to extract and utilize information in order to a) solve a problem and b) tell a great story.
