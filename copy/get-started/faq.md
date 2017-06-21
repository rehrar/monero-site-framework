# Subheading

Copy here

# Questions and Answers

Q: How does Monero have value?
A: Monero has value because people are willing to buy it. If no one is willing to buy Monero, then it will not have any value. Monero’s price increases if demand exceed supply, and it decreases is supply exceeds demand.

Q: How can I get Monero?
A: You can buy Monero from an exchange or from an individual. Alternatively, you can try mining Monero to get coins from the block reward.

Q: What is a mnemonic seed?
A: A mnemonic seed is a set of 25 words that can be used to restore your account anywhere. Keep these words safe and do not share them with someone else. You can use this seed to restore your account, even if your computer crashes.

Q: How is Monero’s privacy different from other coins?
A: Monero uses three different privacy technologies: ring signatures, ring confidential transactions (RingCT), and stealth addresses. These hide the sender, amount, and receiver in the transaction, respectively. All transaction on the network are private by mandate; there is no way to accidentally send a transparent transaction. This feature is exclusive to Monero. You do not need to trust anyone else with your privacy.

Q: Why is my wallet taking so long to sync?
A: If you are running a full node locally, you need to copy the entire blockchain to your computer. This can take a long time, especially on an old hard drive or slow internet connection. If you are using a remote node, your computer still needs to request a copy of all the outputs, which can take several hours. Be patient, and if you would like to sacrifice some privacy for faster sync times, consider using a lightweight wallet instead.

Q: What is the different between a lightweight and a normal wallet?
A: For a lightweight wallet, you give your view key to a node, who scans the blockchain and looks for incoming transactions to your account on your behalf. This node will know when you receive money, but it will not know how much you receive, who you received it from, or who you are sending money to. For more privacy, use a normal wallet, which can be used with your own node.

Q: How is Monero different from Bitcoin?
A: Monero is not based on Bitcoin. It is based on the CryptoNote protocol. Bitcoin is a completely transparent system, where people can see exactly how much money is being sent from one user to another. Monero hides this information to protect user privacy in all transactions. It also has a dynamic block size and dynamic fees, among several other changes.

Q: Does Monero have a block size limit?
A: No, Monero does not have a hard block size limit. Instead, the block size can increase or decrease over time based on demand. It is capped at a certain growth rate to prevent outrageous growth.

Q: What is a blockchain?
A: A blockchain is a system that stores a copy of all transaction history on the Monero network. Every two minutes, a new block with the latest transaction information is added to the blockchain. This chain allows the network to verify the amount of money accounts have and make it resilient to attacks and centralization attempts.

Q: What is Kovri?
A: Kovri is an I2P router written in C++. I2P is a hidden network like Tor with several technical differences. Kovri is an independent project of Monero, but it will work with Monero and several other projects. Kovri hides the transaction broadcast, so other nodes do not know who created transactions. In adversarial conditions, Kovri can be used to hide all Monero traffic through I2P, which would prevent people from knowing Monero is being used. Kovri is currently in alpha, and it is not yet fully integrated in Monero. Learn more about Kovri at the [project website](https://getkovri.org).

Q: What is fungibility, and why is it important?
A: Fungibility is a simple property of money such that there are no differences between two amounts of the same value. If two people exchanged a 10 and two 5’s, then no one would lose out. However, let’s suppose that everyone knows the 10 was previously used in a ransomware attack. Is the other person still going to make the trade? Probably not, even if the person with the 10 is not the one who wrote the ransomware. This is a problem, wince the receiver of money needs to constantly check the money they are receiving to not end up with tainted coins. Monero is fungible, which means people do not need to go through this effort.
