- title : Blockchain under the hood
- description : Fast paced introduction to the technologies underneath the Blockchain
- author : Stefano Paluello
- theme : night
- transition : default

***

- data-background : images/blockchainBckgW.jpg

# BLOCKCHAIN
## under the hood

<br/>

A technical introduction to Blockchain 
<br/>
for not (*so*) technical people

<br/>
Stefano Paluello  [@21.co/palutz](https://21.co/palutz/)

***

<img src="images/danger.jpg" style="background: transparent; border-style: none;"  />

### BUZZWORD AREA !!!

---

## Blockchain

<div class="fragment">
#### Distributed Ledger Tech.
</div>

<div class="fragment">
### Bitcoin
</div>

<div class="fragment">
### Ethereum
</div>

<div class="fragment">
###### Smart Contract
</div>

<div class="fragment">
##### Token
</div>

<div class="fragment">
#### ICO 
</div>

<div class="fragment">
### ...
</div>

---

## Result?

<div class="fragment">
 <img src="images/confusedTravolta.gif" style="background: transparent; border-style: none;"  />
</div>

***

## Blockchain

Definition(s) ( *from Wikipedia* )

<div class="fragment">
A blockchain is a continuously growing list of records, called blocks, which are linked and secured using cryptography.
</div>

<br/>
<div class="fragment">
A blockchain can serve as "an open, distributed ledger that can record transactions between two parties efficiently and in a verifiable and permanent way."
</div>

<br/>

<br/>
<div class="fragment">
PS: it's a pretty "old" concept (despite the recent hype) you can track it back to a paper by Haber and Stornetta in 1991
</div>

[//]: # "For use as a distributed ledger a blockchain is typically managed by a **peer-to-peer** network collectively adhering to a **protocol** for validating new blocks.)"

---

## Still ... ?

<div class="fragment">
 <img src="images/confusedTravolta.gif" style="background: transparent; border-style: none;"  />
</div>

***

## Let's come back to...

<br />

<img src="images/legoduplo.png" width="50%" style="background: transparent; border-style: none;"  />

<br />

## the basics !!!

---

### Basics 1

<br />

<div class="fragment">
### Asset
  Everything (physical or virtual) that we own and could be exchanged.
</div>

<br />

<div class="fragment">
### Transaction
  The action of changing assets ownership
</div>

---

### Basics 2

<br />

<div class="fragment">
### Contract
  Set of rules and conditions used with transactions
</div>

<div class="fragment">
### Ledger
  Book-keeping track of everything happening in our system 
</div>

<div class="fragment">
### Intermediary
  A, eventually, third party facilitating or witnessing the transaction
</div>

---

### A step further...

<div class="fragment">
### Distributed ledger
  The effort to collect transactions is distributed across different trusted parties
</div>

<div class="fragment">
  We need a way to protect and keep updated all the ledgers and to incentivize good behavior amongst the parties
</div>

---

### Step by step...

---


 <img src="images/walkonthewildside.png" style="background: transparent; border-style: none;"  />

---

### The Bitcoin Blockchain

<img src="images/bitcoinBlockchain.png" style="background: transparent; border-style: none;"  />

<br/>
<div class="fragment">
PS: Don't be scared! We will use it just as an example of a ditributed PUBLIC Blockchain
</div>

---

<img src="images/blockchain-privacy.png" style="background: transparent; border-style: none;"  />

<br/>

(credit: MIT Technology Review)

***

<img src="images/godeeper.jpg" style="background: transparent; border-style: none;"  />

---

### How Blockchain works... 

<div class="fragment">
<img src="images/blockWork.png" style="background: transparent; border-style: none;"  />
<br/>
(credit: PwC)
</div>

---

## Key concepts

- Cryptographic functions and hash data structure
- Decentralised protocol
- Distributed ledger (P2P network)

---

### Network types
(Centralized, Distributed, Decentralized)
<img src="images/network2.png" width="70%" style="background: transparent; border-style: none;"  />

<div class="fragment" >
The main benefit of decentralized networks is the absence of a single point of failure.
</div>

---

## Hash and crypto

<br/>

<br/>

<br/>

<div class="fragment" >
#### Disclaimer:
this is the tricky part
</div>

---

<img src="images/runaway.png" width="50%" style="background: transparent; border-style: none;"  />

***

### Hash function


*Hash* function is a mathematical function with 3 properties:

<div class="fragment" >
- Input can be ANY size
</div>
<div class="fragment" >
- It produces a fixed size output (eg. 256 bit)
</div>
<div class="fragment" >
- It's efficiently computable (eg. O(n))
</div>
  
<br/>

<div class="fragment" >
PS: math function = I don't need to trust someone. It's just MATH!
</div>

---

### Cryptographic Hash function

A *Cryptographic Hash* function has 3 additional feature:
<div class="fragment" >
- Collision resistance
</div>
<div class="fragment" >
- Hiding
</div>
<div class="fragment" >
- Puzzle-friendly
</div>

---

### Here we go again... 

<div class="fragment">
 <img src="images/confusedTravolta.gif" style="background: transparent; border-style: none;"  />
</div>

---

### Please

<div class="fragment">
 <img src="images/justhodl.jpg" style="background: transparent; border-style: none;"  />
</div>

---

## Let me explain
  
<br/>

### Collision resistance 

<br/>

It's INFEASIBLE to find two values with the same hash
  
<br/>

with SHA-256 we need to try 2^130 random inputs to achieve a 99.8% chance that at least 2 items will collide

**Application**: message digest 

---

## Let me explain 2

<br/>

### Hiding
  
<br/>

There is no FEASIBLE way to understand the input (x) of a **hash** function H from its output (or cypher Y)
  
<br/>

**Application**: commitment. Committing to a value or a message.

' A commitment is the digital analog of taking a value, sealing it in an envelope, and putting that envelope out on the table where everyone can see it.

---

## Let me explain 3

<br/>

### Puzzle friendly
  
<br/>

This is the most complicated one.
Simple explanation: if someone wants to target our hash function to “force” an output, or to produce a predetermined value, there is no other way than trying all the possible inputs.

**Application**: Search puzzle. 

' a mathematical problem which requires searching a very large space in order to find the solution. In particular, a search puzzle has no shortcuts.

<br/>

***

## Hash Data structure

<br/>

How we store data using our cryptohash functions

<br/>

---

### Hash Data pointer

<br/>

A hash pointer is simply a pointer to where some information is stored together with a cryptographic hash of the information

 <img src="images/hashpointer.png" style="background: transparent; border-style: none;"  />

' a regular pointer gives you a way to retrieve the information
' a hash pointer also gives you a way to verify that the information has not changed.

---

### Block chain

<br/>

A block chain is “simply” a linked list using hash pointers

 <img src="images/hashlist.png" style="background: transparent; border-style: none;"  />

' This data structure is tamper-evident 

---

### Merkle Tree

<br/>

A binary tree with hash pointer is called Merkle Tree

 <img src="images/merkletree.png" style="background: transparent; border-style: none;"  />

' Proof of membership: with a Merkle tree it's quite easy to have a concise proof of membership (not feasible with the bock chain). It's enough to check a log(n) node to verify if a node is part of the tree.

---

Merkle Tree and block chain. Remember anything?


<div class="fragment">
<img src="images/bitcoinBlockchain.png" style="background: transparent; border-style: none;"  />

<br/>

### The Blockchain!

</div>


***

## Benefits of Blockchain

- **Immutability** – A third party cannot make any changes to data.
- **Corruption & tamper proof** – Apps are based on a network formed around the principle of consensus, making censorship infeasible.
- **Secure** – No central point of failure and secured using cryptography, applications are well protected against hacking attacks and fraudulent activities.
- **Zero downtime** – Apps never go down and can never be switched off (sort of).

---

## Downsides

- write decentralized app is a bit tricky: quite new theory, not so much experience, lack of proper/stable tools.
- smart contracts could be faulty or buggy (DAO hack, ICO hack, ...)
- if a mistake is made there is no other way to correct it ithan with a Harf Fork.



