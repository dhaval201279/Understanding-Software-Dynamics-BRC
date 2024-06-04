# Terminologies
A **transaction** or **query or request** is an input message to a computer system that must be dealt with as a single unit of work.

The **latency or response time** of a transaction is the time elapsed between sending a message and receiving its result. The **offered load** is the number of transactions sent per second; when this exceeds the number of transactions processed per second, response time suffers, sometimes dramatically.

**Transaction latency** is not constant—it has a probability distribution taken over thousands of transactions per second. **Tail latency** refers to the slowest transactions in this distribution. A simple way to summarize the tail latency is to state the 99th percentile latency—the time that is exceeded by the slowest 1% of all transactions, i.e., by 50 transactions every second if the offered load is 5,000 transactions per second.