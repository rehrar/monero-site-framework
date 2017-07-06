# Blockchain: The Noob's Guide

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

Another area where a database can be changed is if the database is hacked. A hacker can maybe guess weak passwords, or otherwise compromise a system and get full access to change records in the database. If something like this happens, the damage that is done may even be irreversible. 

The benefit though, is that most databases are usually private. The only people who can see all of the records are the database administrators themselves. So not just anyone can go snooping through your private records. Still, this does leave an element of trust, once again, to the administrators that they won't go peeking into information that isn't theirs.

So to summarize, a database is a collections of information that is usually arranged in tables for easy access. Most internet applications run on databases, so they are integral for our modern world. But there are a few ways that our own information on a database can be changed without our consent, either by a database administrator, or a hacker.

### Enter blockchain
So how does all of this fit in with blockchain technology? Well, at its core, a blockchain is just a database. It's a very special type that is distributed amongst multiple people, but it's a database nonetheless. The only thing is, because of the technologies that make it unique (which we will explore in just a moment), a blockchain cannot be hacked in the typical way, and requires no trusted database administrator to function. This means the two big vulnerable areas of a database are solved in a blockchain. But there is a privacy trade-off, as we will see in the coming section. For now, let's start by exploring the new technologies that blockchain introduces, and how they solve the two major weaknesses of databases.
