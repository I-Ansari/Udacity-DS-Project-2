# SF Crime Statistics with Spark Streaming

## Kafka Consumer Console

![Kafka Consumer Console](https://user-images.githubusercontent.com/14344723/84572246-d736ea00-ada9-11ea-9794-666a863d8d3a.JPG)

## Progress Reporter

![Progress Reporter](https://user-images.githubusercontent.com/14344723/84572393-a4412600-adaa-11ea-9eb3-6807140616a1.JPG)

## Spark Streaming UI

![Spark Streaming UI](https://user-images.githubusercontent.com/14344723/84572410-c0dd5e00-adaa-11ea-85e0-2e4c9c16da84.JPG)

## Questions

How did changing values on the SparkSession property parameters affect the throughput and latency of the data?

Changing SparkSession property parameters had a very significant affect onthe parameters inputRowsPerSecond and processedRowsPerSecond

What were the 2-3 most efficient SparkSession property key/value pairs? Through testing multiple variations on values, how can you tell these were the most optimal?

I have found increasing maxOfffsetPerTrigger and maxRatePerPartition results in significantly increasing inputRowsPerSecond and processedRowsPerSecond.
