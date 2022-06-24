# Spotify-s-Top-200-Chart-for-June-9th-2022
Took a dive into Spotify's Top 200 streamed artists/tracks for the week ending on Friday June 9th. Used jupyter notebooks and various other python libaries(Pandas, Matplotlib, and Numpy) to analyze and visualize the data. 

First I loaded the data from a csv file onto a Pandas dataframe by extracting needed columns from the csv file into lists which were added into a single dictionary. This dictionary then became the Pandas dataframe from which this whole project was based on. 

I proceeded to get some basic descriptive statistics on the data from various columns in our data('Streams' column, 'Artist Name' column, and 'Tracks' column). Doing so demonstrates maxs, mins, means, counts, data types, unique values, the top value by count(i.e. Artist with most tracks charting) and we're also able to see the top track in the Tracks columns is 'Running Up That Hills(A Deal With God) by Kate Bush has claimed #1 on Spotify's Charts. 

The dataframe was then sorted by total amount of streams, the number of weeks it has been charting followed by the label/source that released the track. 

A secondary dataframe was created to include only the Top 10 tracks for the week. We will use this later to create a quick visualiztion of this dataframe and gain insights.  

Looking throught the source column on the dataframe I decided to breakdown this dataframe further by grouping these labels back to their respective parent companies, one of the 3 Major Labels(Universal Music Group, Warner Music Group and Sony Music Entertainment). I furthered grouped the other/indie(independent) labels/sources into a 4th category as 'Other/Indie'. After a couple hours of researching and tying labels back to their parent companies I had broken down the dataframe into 4 separate dataframes: UMG_labels, WMG_labels, Sony_labels and others_labels. 

The next step was to get basic statistics  on these 4 different dataframes. Using aggregate functions(.sum(), .mean(), .max(), and .min()) we found the basic stats on the streams columns per Major Music Label and the indies. 

Returning back to Top 10 tracks on Spotify- a quick Scatterplot reveals the magnitude in stream counts for the first two values: both 'Running Up That Hill(A Deal with God)' by Kate Bush(57M) and 'As It Was' by Harry Styles(56M) had over 55,000,000M streams whereas the third entry, 'Me Porto Bonito' by Bad Bunny & Chencho Corleone was teetering with 39.8M. These numbers showcase the impact virality has been having on music as these two songs have been going viral on the popular social media platform, TikTok(*as of early June 2022). 

Next, a bar chart was created per Major Music Label to showcase their breakdown of streams per their respective artists/tracks. 

Lastly- using a pie chart I broke down marketshare per Major Music Label + Others/Indies of Spotify Streams for the entirety of this weekly chart. By looking at the data we see that both Warner Music and Sony Music were able to claim huge percentages of total streams on Spotify. Knowledge of relevant current events in pop culture related to these two songs: 'Running Up That Hill' & 'As it Was' creates further assumptions and hypothesis on why they have captured a great percentage of stream total. 

