# Terminologies
A **transaction** or **query or request** is an input message to a computer system that must be dealt with as a single unit of work.

The **latency or response time** of a transaction is the time elapsed between sending a message and receiving its result. The **offered load** is the number of transactions sent per second; when this exceeds the number of transactions processed per second, response time suffers, sometimes dramatically.

**Transaction latency** is not constant—it has a probability distribution taken over thousands of transactions per second. **Tail latency** refers to the slowest transactions in this distribution. A simple way to summarize the tail latency is to state the 99th percentile latency—the time that is exceeded by the slowest 1% of all transactions, i.e., by 50 transactions every second if the offered load is 5,000 transactions per second.

# Long Tail Latency
## Percentiles
If our latency histogram has 50,000 measurements, then the shortest 500 of these are the fastest 1% and the longest 500 are the slowest 1%. The numeric boundary between the fastest 99% and slowest 1% is the 99th percentile value—99 percent of the sorted measurements are less than or equal to this value. (There are many such values, all lying between the 49,500th and 49,001st sorted measurements; any of these numbers will do, but conventionally the exact 49,500th sorted value will be used.) A quick but useful way to describe a long-tail distribution is to give the 99th percentile value, or 95th, 99.9th, etc

# Order of Magnitude
In this book, we use decimal orders of magnitude unless otherwise qualified, using the notation O(n) for “on the order of n,” with the units always specified. It matters a lot whether you are talking about O(10) nanoseconds or O(10) milliseconds or O(10) bytes

# Five fundamental resources
There are only four computer hardware resources shared between unrelated programs running on a single server:
1. CPU
2. Memory
3. Disk/SSD
4. Network

If a program has multiple cooperating threads, there is a fifth fundamental resource:
1. Software critical section

# References



