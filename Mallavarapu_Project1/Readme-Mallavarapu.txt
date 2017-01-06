Project 1  
Aditi Mallavarapu
amalla5@uic.edu

Details of Data Collected, Motivation:

Since past few months I have been watching a lot of Netflix, I wanted to see if there is a pattern in my schedule any particular 
times or days I watch more or watch less. How long is each show that I watch? Do I watch continuously? (Binge watch).

So I decided to gather my Netflix log for past month and a half. (100 data points)
Netflix gives two separate log details:
1) what was watched on what date
2) Timewhen that was watched, the device it was watched on.

I gathered the data into an excel sheet, and also collected the length of each of the shows from IMDB.
I also categorized the shows as if they were Movies, Documentaries, or TV Shows.

Decision to choose the Visualisation Technique:

I wanted to incorporate most of the attributes of my data into one visual picture. 
It had many dimensions: time, day, date, length of the show, type of show, device on which it was watched.

I chose to represent the time dimension in a non-conventional way by splitting the hours of the day into 4 parts
	1) morning 6am to 11.59am - represented by innermost circle
	2) afternoon 12pm to 5.59pm - represented by the middle donut
	3) Evening 6pm to 12am - represented by the outer donut
	4) night 12am to 6am 
	
However, while working with the visualisation I discovered, that I haven't watched anything beyond 12am ( which is a good thing :))
So I decided to omit those 6 hours from my visualisation so that I could concentrate on data that was heavy.	

I have represented each chunk of 6 hours as a small sector of the circle each sector representing an hour, the dial works clockwise 
with each sector denoted by a number indicating one of the 24 hours of the day.

For every show that I watched based on its precise time, I plot a bar for the show whose length depends on the duration of the show.
Longer the line, longer I watched.

The visualisation also provides details on hovering over the little bar representing the show, the name of the show the time, day, 
date, type of the show, and on which device it was watched on.

The visualisation has a small legend to the upper right corner, the legend is a toggle clicking on which the data doesnot display the 
shows watched on day of the week. To make sure I dont display empty time, one cannot disable all the days. The chart will need atleast one day to be enabled.

(Note: While working on the project, I found a bug which I wasn't able to solve. There is a data-point that gets displays in 
the wrong position with a wrong color. You will be able to see it when to disable all days but Monday,a pink bar (representing sunday) for a monday data point
with wrong position based on the time. If I remove that data point, some other data takes its place.)

I have followed the following tutorial for the assignment:
http://zeroviscosity.com/d3-js-step-by-step/step-3-adding-a-legend
I incorporated the CSS part and the size of the rectangles for the legend to fit my data.

