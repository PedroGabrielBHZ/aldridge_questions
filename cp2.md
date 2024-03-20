# Chapter 2 questions & answers

1. Would you encrypt your trading orders before transmitting them to the execution venue over the Internet? Explain.

    The decision of encrypting trading orders rests on the trade-off between added security and the time it takes to encrypt and decrypt the message. In the case of high-frequency trading, the time it takes to encrypt and decrypt the message may be too long, and the additional security may not be worth the time cost, specially when the message is sent over a secure network, such as in a co-location facility.

2. Mr. Smith has read about the “arms race” of computer technology in the financial services industry and decides to invest into the latest super computer to increase the odds of fast order transmission. Is Mr. Smith’s investment justified? Where does most message congestion occur in the cyber-universe today?

    Mr. Smith's capital could be better elsewhere employed. In the financial services industry, message congestion often occurs at the network level. Even if there is no congestion on the network, the main delta between a supercomputer and a regular computer is in signal generation, not in transmission, as the latter is mostly a function of network infrastructure.

3. What is co-location?

    Co-location is the practice of placing a trading server in the same data center as the exchange’s matching engine. This reduces the time it takes for a trading order to reach the exchange, as the distance between the trading server and the matching engine is minimized. Consequently, round-trip time is reduced, and the trader can execute trades faster. This practice, also known as proximity hosting, is common among high-frequency traders and often comes with a considerable fee.

4. On average, how much slower is the transmission of trade order messages in comparison with quote messages?

    The transmission of trade order messages, which is done over TCP, is on average 3 times slower than the transmission of quote messages, which is done over UDP. This is because TCP is a connection-oriented protocol, which means that it requires a three-way handshake to establish a connection, and it also requires the receiver to acknowledge the receipt of each message. UDP, on the other hand, is a connectionless protocol, which means that it does not require a three-way handshake to establish a connection, and it does not require the receiver to acknowledge the receipt of each message.

5. What is a heartbeat?

    A heartbeat is a periodic signal broadcast onto the participant's communication parties indicating that the connection is still active and in a state of good technological health.

6. The best offer on exchange A contains 300 units of instrument X, the best offer on exchange B contains 500 units, and the best offer on exchange C contains just 100 units.Your customer wants you to buy 550 units on his behalf. How would you break up the customer’s order and send them to exchanges under the minimal impact algorithm?

    The minimal impact algorithm would break up the customer's order as follows:

    - 300 units to exchange A
    - 250 units to exchange B
    - 0 units to exchange C

    This way, the customer's order would not impact the best offer on any of the exchanges, and the customer would be able to buy 550 units without moving the market.
