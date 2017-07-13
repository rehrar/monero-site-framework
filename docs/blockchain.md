# Blockchain: The Noob's Guide (Part 1)

## Table of Contents

## Goals
After reading this article, the reader should be able to do the following:
- Differentiate between a blockchain and a normal database as well as compare them
- Identify the problems that blockchain technology is trying to solve
- Understand the limitations of blockchain technology
- Learn the importance of education and critical thinking in relationship to claims made about new technology

## Introduction
Blockchain is a relatively new and exciting technology that has taken many areas of the internet by storm in recent years. Best known for powering the first cryptocurrency [Bitcoin](https://bitcoin.org), it is unfortunate that the general public, indeed in many cases cryptocurrency enthusiasts, do not have an accurate understanding of what blockchain technology really is and what problems it tries to solve.

This Educational User Guide (EUG) is made to try to remedy this problem by providing an easy-to-understand explanation that still goes into great detail as to what exactly blockchain technology is, and, sometimes more importantly, what it isn't. The Monero community thinks it is crucial for noobies and enthusiasts alike to be able to critically evaluate the claims made by the thousands of cryptocurrencies available, including Monero itself. 

It is best to keep in mind that it's not possible to cover all necessary information in one article, so the reader is encouraged to use this article as a springboard from which to get started for further learning. There will be numerous relevant links both within the text as well as at the bottom of each section for further study should the reader decide to pursue discussed topics further.

If the reader has any questions, notices any errors, or would otherwise like to amend a portion of this document, it is possible to reach out to the [Monero community](https://getmonero.org/community/hangouts/). 

## A Digital World
The internet has fundementally changed the way that society operates on a variety of levels. Everything from shopping to driving to dating has been touched by the far reach of the digital world. It was only a matter of time before people started to discover a sort of independence that hadn't been encountered by any of the previous generations. [Independence of education](https://khanacademy.org) from universities, independence of love prospects from one's physical location, and even independence of money from the existing government powers.

[Wikipedia describes blockchain](https://en.wikipedia.org/wiki/Blockchain) as: "a distributed database that is used to maintain a continuously growing list of records, called blocks." Well that doesn't give a lot of clues for the average person. The rest of the article doesn't fare much better. Let's see if we can't find a simpler explanation.

### Ye olde databases
At its simplest form, a database is a place on a computer where information can be stored and retrieved. Data is typically stored in tables and, depending on the person who set it up, in an easy to understand structure. Almost everything runs on databases. If you think of large online retailers, like Amazon or Overstock, they all have databases where each of the items that they sell are stored. The type of information can include the name, the item number, price, and a variety of other information about the product.

Let's make an example database to see what this might look like. If you had a database of people, it might be arranged something like this:
```
+----------+------------+-------------+------------------+------------+
| Name     | Hair Color | Eye Color   | Address          | Extra Toe? |
+----------+------------+-------------+------------------+------------+
| Alex     | Brown      | Blue        | 222 Two Drive    | N          |
+----------+------------+-------------+------------------+------------+
| Jerry    | Blonde     | Blue        | 333 Three Way    | Y          |
+----------+------------+-------------+------------------+------------+
| Samantha | Brown      | Almost Blue | 444 Eight Street | N          |
+----------+------------+-------------+------------------+------------+
```
From this database about people, a person who needs the information can ask the database to give him all information about the person with the name Alex, or give all the names of the people who have a eye color of Blue. There's a huge number of ways that the data can be stored and retrieved.

Now here's the thing, our example database is full of silly information, and if I was to change Alex's eye color to Hazel, nobody would really care. But some databases have really sensitive information, such as people's finances and personal records. Imagine if you logged into the online management portion of your bank only to find your account balance radically changed because somebody erroneously (or maliciously) made a change to the database. This begs the question, who has control of changing a database.

A database is usually only changed by a server administrator or another application or user with sufficient privileges. This introduces an element of trust. We have to trust that the people with the ability to change the databases won't do so in order to benefit themselves, but not everyone has such noble intentions. 

Another area where a database can be changed is if the database is hacked. A hacker can maybe guess weak passwords, or otherwise compromise a system and get full access to change records in the database. If something like this happens, the damage that is done may even be irreversible. If you think about it, this weakness is actually related to trust as well. Trust in the security systems that have been placed by the administrators, and trust that the database has not been tampered with at all (by administrators or hackers).

So the biggest weakness of databases can be summarized in one word: trust.

The benefit though, is that most databases are usually private. The only people who can see all of the records are the database administrators themselves. So not just anyone can go snooping through your private records. Still, this does leave an element of trust, once again, to the administrators that they won't go peeking into information that isn't theirs.

So to summarize, a database is a collections of information that is usually arranged in tables for easy access. Most internet applications run on databases, so they are integral for our modern world. But there are a few ways that our own information on a database can be changed without our consent, either by a database administrator, or a hacker.

### Enter blockchain
So how does all of this fit in with blockchain technology? Well, at its core, a blockchain is just a database. It's a very special type that is distributed amongst multiple people, but it's a database nonetheless. The only thing is, because of the technologies that make it unique (which we will explore in just a moment), a blockchain cannot be hacked in the typical way, and requires no trusted database administrator to function. This means the glaring weakness of trust in a database is solved in a blockchain. 

Sounds too good to be true? A little later we'll look at some of the weaknesses that blockchain comes with, but for now let's explore how blockchain solves this primary issue.

#### Nodes

Let's start with what a decentralized database needs to function. First, to make it decentralized, the blockchain needs an application that will copy the database to the computer of every person who wants a copy of it. We'll call these computers with a copy of the database 'nodes' from now on. Nodes need to have a decentralized way to start from scratch. Meaning, if I decide to start a node, where do I get my copy of the database from? Well, if I have to get it from a centralized database that everybody gets their information from, that defeats the whole point doesn't it? Because we go right back to that trust issue of that centralized database. Instead, nodes are able to get their copy of the database from other nodes, or 'peers' and can constantly check with other nodes on the network that their copy of the blockchain database is correct.

But what if a change needs to be made? Here's where things get tricky. If a valid change is made on my copy of the blockchain, I need to let the whole network know of the change, and so every other node on the network can update their databases with the new values. But what if somebody else updates the same value as me at the same time? Which is considered the valid update, and which one gets thrown out?

This question is the reason why the current implementation of a blockchain database is to to separate the database into individual units of time called 'blocks' and string these units of time together to form a block chain. This is a huge topic into itself, and will probably warrant another article entirely, so for now, just know that once a block has been added to the blockchain, it cannot be changed. This makes the blockchain immutable. In other words, we can only make changes to the current block (that has yet to be added), and once it's added, the information saved in it cannot be modified. So if we are on block 1000 of the blockchain, and I wanted to modify a piece of information in block 900, I would actually have to undo changes in the past 100 blocks to get to the information I want to change, and in order to make those changes, I would have to perform a huge computational task called mining, which is the only way in which a blockchain can be changed.

But before we get into mining, we have to see that we've already run into our first big issue. If the information being stored and distributed on every node is very large in size (meaning it takes a lot of storage space on the computer), then blockchain becomes impractical. Imagine if Amazon decided they were going to use blockchain technology for their gigantic database of items for sale. If I wanted to run an Amazon node, I would have to have a computer with enough storage space to hold their entire catalogue, and enough room to grow for when they add more items. In these types of scenarios, blockchain technology brings more problems than it solves, and operating under a regular database that they control (and that we trust) is probably a better fit.

This means that blockchain, in its current form, is ideal for use in distributing small amounts of information. Things like plain text and numbers, since those don't take a lot of space on computers. The larger the amount of information that an application is trying to store, the more unlikely that the information will fit on a regular user's node, and the more likely blockchain will not work.

With this in mind, the largest use of blockchain technology is cryptocurrencies (like Bitcoin), which are simply a ledger of information showing who currently owns what coins. We'll expand further on cryptocurrencies in blockchain in another article, but you can start researching on your own. It's a fascinating world. Because cryptocurrencies are the primary implementation of blockchain technology, for the remainder of the article, I will be using strictly cryptocurrency examples to explain how the blockchain works. 

## Conclusion

Wow, that was a lot to get through, and we're nowhere near finished. Still, maybe it's best to leave the story here for now and continue in future articles. Don't want to completely overwhelm you with information. If it still seems complicated, that's fine. It's crazy new technology, and may take a while to come to terms with how it works. For now, let's summarize what we've learned.
- Blockchains are simply databases that are distributed among many computers.
- Databases are places where information can be stored and retrieved by users and applications.
- Most databases are maintained, and require an element of trust that the data inside the database has not been tampered with, either by the maintainers or by hackers.
- Blockchains solve this element of trust by giving a FULL copy of the database to everyone who wants to have one, as well as through other technologies yet to be discussed.
- A computer who hosts a copy of the database is called a node.
- A node is able to make changes to the database and broadcast them to other nodes, and is also able to implement changes made by other nodes.
- Nodes can be started in a decentralized manner, utilizing peers to obtain a copy of the blockchain rather than a centralized database with the same issues of trust.

We've still got lots to cover. Things like Mining, cryptography, incentive (block rewards), blockchain weaknesses, and even future technologies that strengthen and improve blockchain such as blocktrees. It's all very exciting and, quite honestly, is the way that the future is headed. Thanks for joining us. Check back for future articles.
