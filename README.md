# Surfs-up

## Overview

The porpose of this project was to gather information about the weather and precipitation on a city in Hawaii. This information was stored in an SQLite data base and SQLAlchemy was used to acces this information and transform it into DataFrames. Once it was stored in a DataFrame, the describe method was used to understand the distribution of the data and how it behave. 

In this module I learned the use of SQLAlchemy and why are SQLite data bases used for. Using SQLAlchemy I was able to perform queries to retrieve the specified data to gather and understand the behaviour of the particular dataset.

## Results

### June Temperatures 

![June_Describe](https://user-images.githubusercontent.com/95836718/156909699-e49b22a2-1760-426b-83df-5dfa817fad72.png)

### December Temperatures

![Dec_Describe](https://user-images.githubusercontent.com/95836718/156909703-fa8a9af8-d4e5-4f9b-83cf-7ed72d3e75d9.png)

Analysing the temparutes from December and June we can understand and see that:
- Both data sets have similar standard deviations (around 3). We can at least assume that both of this data the means are some what descriptive of the whole data set.
- They are less data points in the december data set. This might be due to a possible winter breaks in certain stations.
- Both maximum temperatures are around the 84 degrees.

## Summary

This data show a constant behaviour on temperatures. June is one of the hottest months of the year and December is one of the coldest. We saw that both datasets behave somehow similarly. A side from the obvious drop in the mean temperature, both data sets had similar max temperature and similar standard deviation. With that beign said, special attention would be requiered to the december dataset. It was shown that the lowest temperature was 56 degrees, this is a particularly cold weather for surfing because it will requiered a higher degree of wetsuit to protect the surfer of the cold temperature. Also, this might not make it appealing to surf during winter. Financial analysis are requiered to calculate if the earning of the summer season are enough to sustain the store during the winter eventhough there might be less costumers.

### Bonus Queries.

The first obvious queries is to gather the precipitation during this months and understand their behaviour and how likely it is for it to rain.

![June_PRCP](https://user-images.githubusercontent.com/95836718/156909980-eefe56e4-118d-4b84-b833-107e4551bcf2.png)

**Note** June Precipitation statistics.


![Dec_PRCP](https://user-images.githubusercontent.com/95836718/156909982-55ae221e-7336-4f32-a537-8f930ccb6e9b.png)

**Note** December Precipitation statistics.

We can clearly an outlier in both data sets. To find it we can write another query.

![June_out](https://user-images.githubusercontent.com/95836718/156910006-0e2841eb-696b-4974-9de3-b64474cbca4d.png)

**Note** June Outlier.

![Dec_Out](https://user-images.githubusercontent.com/95836718/156910010-544786cf-c72b-4090-a48d-4978dbab02b5.png)

**Note** December Outlier.
