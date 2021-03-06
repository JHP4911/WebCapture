# Why Developers Should Bet Big on Streaming

_Captured: 2018-03-01 at 15:08 from [dzone.com](https://dzone.com/articles/why-developers-should-bet-big-on-streaming?edition=365206&utm_source=Zone%20Newsletter&utm_medium=email&utm_campaign=big%20data%202018-03-01)_

###  Investing in streaming enables data in motion and real-time applications, as well as some of the most interesting AI and ML use cases today. 

Access NoSQL and Big Data through SQL using standard drivers (ODBC, JDBC, ADO.NET). [Free Download ](https://dzone.com/go?i=250345&u=https%3A%2F%2Fwww.cdata.com%2Ftech%2Fbigdata%2F%3Futm_source%3Ddzone%26utm_medium%3Dbump3%2520)

[This article is featured in the new DZone Guide to Big Data Get your free copy for more insightful articles, industry statistics, and more!](https://dzone.com/guides/big-data-stream-processing-statistics-and-scalabil)

To many developers, real-time use cases are viewed as the exclusive playground of mega Internet players like Amazon and Netflix with their infinite resources, gigantic customer bases, and armies of PhD engineers. (Real-time means different things to different people. Here we define it as "process on arrival" to ensure low latency and fast time to value.) I'm here to tell you that real-time is no longer an elite opportunity. Most enterprises today are dealing with dynamics that are pushing real-time requirements. Consider all the data that your web and mobile users are generating and requesting. How can you gather all this data, transform it, mine insight, and feed it back to your users in real-time (or as close to as possible) -- delivering efficiencies in conversions, retention, and automation of common operational processes? The volume of data being generated by your users on the web, mobile, and (increasingly) IoT devices is growing vastly every year, and this is an opportunity that your company can't afford to miss out on.

## You Can't Do Real-Time Without Streaming

Streaming is the backbone of the most interesting machine learning and artificial intelligence use cases in the enterprise today. Let's discuss how we got from the early big data origins to where we are today with streaming: fast data.

### Big Data Wave One: Hadoop/Batch

The first wave of big data was the Hadoop ecosystem, with HDFS, MapReduce, and friends (i.e. Hive, Tez, Mahout, Pig, YARN, HBase, Avro, ZooKeeper, and Flume). Store your data in HDFS and then perform batch processing of that data overnight -- with hours of latency, i.e. hours of lead time to get insight and intelligence out of your data. In these early days, big data was equal to Hadoop. But the original components of Hadoop were rooted in batch-mode and offline processing approaches commonplace for decades. This first wave of Hadoop/Batch had a lot in common with how most search engines worked in the early days, where data is captured to storage and then processed periodically with batch jobs. Worth mentioning is that Apache Spark is one of the projects to successfully challenge the traditional batch model with what they called mini batching, which maintains the model of batching, but with increased batch frequency and thereby lower latency.

### Big Data Wave Two: Lambda Architecture

In the second wave, we saw that the need to react in real time to "data in motion" -- to capture the live data, process it, and feed the result back into the running system within seconds-long (even sub-seconds) response time -- had become increasingly important. This need instigated hybrid architectures such as the lambda architecture, which had two layers -- the speed layer for real-time online processing and the batch layer for more comprehensive offline processing -- where the result from the real-time processing in the "speed layer" was later merged with the "batch layer." This model solved some of the immediate need for reacting quickly to (at least a subset of) the data. The downside was that it added needless complexity with the maintenance of two independent models and data processing pipelines, as well as an automated data merge in the end.

### Big Data Wave Three: Full Embrace of Streaming

During the second wave, we started to realize that streaming could do most of our processing in real-time. This led to the third (at the time of writing: current) wave of big data: the move to a full embrace of streaming (sometimes referred to as the kappa architecture, as an evolution of lambda architecture). In this new model, events are streamed continuously, with the presumption that they are unbounded -- that they may never end -- so systems can no longer wait to receive "all the data," and instead need to process it on the fly, as it arrives. This calls for new techniques: it's no longer possible to get a comprehensive view of all the data before processing it, but you need to define your window of processing -- how you should group the incoming events and where to "draw the line" before processing the group -- and distinguish between event time (when it's happening) versus processing time (when it's being processed). With streaming, the fundamental shift is moving from "data at rest" to "data in motion" -- from batched to real-time.

## Signs That Streaming Data Has Arrived

If you're looking for more evidence that streaming is winning out as the preferred method for how applications and systems interact with real-time data, here are some additional signs of that process:

### Streaming Has a Thriving Ecosystem

It's a buyer's market for stream processing engines: Flink, Spark Streaming, Akka Streams, Kafka Streams, Storm, Cloud Dataflow (Google), Pulsar (Yahoo), Pravega (EMC), and others. It's a sign of maturity for streaming that more engines are being released, each with their specific use-cases, focus, and edge.

### Architectures for Real-Time Streaming and Microservices Are Converging

As we see more microservices-based systems grow to be dominated by data, their architectures are starting to look like big pipelines of streaming data. The convergence of streaming and microservices is bringing all the power of streaming and "data in motion" into the microservices themselves -- both as a communication protocol as well as a persistence solution (using event logging) -- including both client-to-service and service-to-service communication. Thinking in streams-as-values also forms the basis for designing your microservices around domain events, and so-called events-first domain-driven design.

### Streaming Is Becoming the New Integration

A growing sentiment within the industry is the need to rethink Enterprise Integration (EIP) in terms of streams as a first-class concept -- specifically, to be able to think about streams as values, manipulate streams, join streams, or split them apart in a fully asynchronous and non-blocking fashion, with flow-control (backpressure) throughout. An emerging standard for this is the Reactive Streams initiative (now included in JDK9 as the FlowAPI).

### Time to Invest in Streaming

When you look at your career as a developer, a lot of the defining moments are based on how early you recognize an opportunity, embrace a new set of technologies, and where you decide to invest your time. Choosing tools of the trade and where to focus energies are the biggest bets you place as a developer. Putting streaming at the top of your to-do list (to get invested in ASAP) is a bet you should absolutely consider making in 2018--for your career, your project, your business, and for fun. It's easy to forget, but the web used to be a new concept, too-- and now, not only does every company embrace it, but the web became so popular that web applications became the new standard and largely killed off the desktop software market. That's the sort of transformative impact that real-time streaming will have on application and system design long-term. Streaming is not a trend, it's a requirement -- and by embracing it in your system design now, you will get ahead on the real-time adoption curve and take advantage of some of the most interesting new opportunities available to modern developers.

[This article is featured in the new DZone Guide to Big Data Get your free copy for more insightful articles, industry statistics, and more!](https://dzone.com/guides/big-data-stream-processing-statistics-and-scalabil)

[The fastest databases need the fastest drivers](https://dzone.com/go?i=250346&u=https%3A%2F%2Fwww.cdata.com%2Fblog%2Fnews%2F20170601-bigquery-driver-comparison%3Futm_source%3Ddzone%26utm_medium%3Dbump4) \- learn how you can leverage CData Drivers for high performance NoSQL & Big Data Access.
