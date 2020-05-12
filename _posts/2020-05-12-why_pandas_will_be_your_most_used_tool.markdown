---
layout: post
title:      "Why Pandas Will Be Your Most Used Tool"
date:       2020-05-12 22:44:18 +0000
permalink:  why_pandas_will_be_your_most_used_tool
---



Pandas is an integral part of the comma-separated value and excel file data exploration and learning. With a few simple lines of code, you can quickly (and with minimal memory usage) run quick and unique filters, find related data and even create fantastical graphs that further relay the facts of the data. If we incorporate basic statistics through Numpy, we can also break the data into percentiles and quadrants based on specific filters. Let’s take a look at some of the ways Pandas can make analyzing a data file easier. 

Let’s say you have a spreadsheet that was complied by two people – they surveyed 100 people each and collected data points on all of those people. However, when the subjects were filling out their data forms, a lot of questions were skipped – thus resulting in missing values for numerous “traits” for a lot of the subjects. To maintain the integrity of the research, we can not merely fill in values for these traits (unless they can be proven to be factual). Pandas allow us to quickly filter out these subjects with missing values and “delete” them from our main data set to allow us to deduce more accurate and meaningful statistics. As an example, let us look at the trait “Eye Color,” located in the column “Eye_Color,” after having imported Pandas and opened the projects CSV file, we must write a simple code to calculate how many incomplete data sets there are.  Now without pandas, this would be very deciduous with lines and lines of code, but with pandas, we can extract them rapidly with the quick code set “.iloc,” which essentially isolates and locates whatever you tell it. That would look something like this:

```
For row in df.index:
Count = 0
For entry in df.iloc[‘Eye_color’].isnull()
If entry:
	Count += 1
If count! = prev_count and row! =0:
Prev_count = count 
Print(Prev_count) #
```

Once you have this step done, then you can easily “filter out those rows to allow more data accuracy” by reimporting the file with filters. The code would look something like this:
`# df1 = pd.read_csv(‘data|Population_traits.csv’, skiprows = [Enter row numbers to be skipped], nrows =[1]]` 
Now you have a cleaned up list by removing incomplete data; we can begin to see if there are any correlations in the data points by exploring the data further. Let’s say in the information collected we have four data points: zip code, highest education & homeownership status we’d like to see if there is a correlation between these three values. Our first step is to check the data for outliers; in other words, data in the extremes that become nonrelevant to the data pool. For example, all of our subjects were questioned in the same area so we can safely assume that most of the zip codes would be close to the zip code in which they are collected, but let’s say we have one random zip code from multiple states away. This data point would be irrelevant to our current study as the person is just visiting the area.  By utilizing Numpy, we can find both the min and the max value of our zip code, or we could make a Pandas occurrence functions to print the number of incidents of each zip code. The zip code with the least or with a singular data point would be the outlier. 


	After sorting and sifting through our data, Pandas makes it incredibly easy to plot all of our data points with Matplotlib. Each data point can be put against each other in a scatter-matric plot or, if we are only looking to analyze the three data points mentioned previously, Pandas & Matplotlib can quickly transform them into a scatter plot. With all the possibilities of Pandas and it’s extension programs, data exploration and presentation is much quicker.  One of the most significant selling points is how fast Pandas can sift through data points; even massive excel files can be combed through with a few lines of codes in mere seconds.  To see just how many amazing features Pandas you can check out their website: https://pandas.pydata.org/docs/getting_started/index.html#getting-started. 

		


