<!-- Copy and paste the converted output. -->


Introduction

The Cypherpunks

Hashcash

Blockchain

Bitcoin

Drugs and Gambling

Security

Brainwallet

Altcoin and DApps

The Future

About the Author

**Introduction**

“Bitcoin gives us, for the first time, a way for one Internet user to transfer a unique piece of digital property to another Internet user, such that the transfer is guaranteed to be safe and secure, everyone knows that the transfer has taken place, and nobody can challenge the legitimacy of the transfer. The consequences of this breakthrough are hard to overstate.” – Marc Andreessen (venture capitalist and co-founder of Netscape)

I want you to focus on the last sentence of this quote from Marc Andreessen. The consequences of this breakthrough are hard to overstate? Bill Gates has called Bitcoin a technological tour de force. You can’t hardly watch the news or popular television shows without a mention of Bitcoin. From C-SPAN to Simpsons, Jeopardy, or Family Guy, Bitcoin has become a household name. But do you know what all the hype is about? Do you know why this new strange entity is getting so much attention? If not, then you picked the right book. This book is for the common man who wants to go from ignorance to being in-the-know on everything related to the revolution that is Bitcoin and blockchain in the shortest period of time. 

This book is not for the person who wants to make a quick buck on the latest craze with no interest in the underlying technology driving the actual change we are seeing. Bitcoin is a culture, a technology, and a revolution. It’s the seed that is giving birth to something that will inevitably alter the course of human civilization. This is just the beginning. I believe we are in the Netscape days of blockchain technology. If you didn't know, Netscape was the first web browser launched in 1994. In this book I’m going to bring you up to speed on cryptocurrencies, public key cryptography, distributed ledger technology, hashing algorithms, consensus protocols, decentralized autonomous organizations, and anything else you need to understand and intelligibly participate in this revolution.

Most of all, I hope to introduce you to an unstoppable movement. A movement that aims to unshackle free people from the bondage of onerous regulation and nanny state ideologies. A movement thats puts financial power back into the hands of the individual. If freedom scares you, you’re about to get very afraid. Bitcoin is not only liberating individuals, its created completely autonomous machine organizations. By the time you finish this book, you will have the tools to understand and participate in this revolution if you so choose.

**The Cypherpunks**

“Bitcoin may be the TCP/IP of money.” – Paul Buchheit (creator of Gmail)

To give a little context to this quote. Understand that the entire internet runs on a communication protocol called TCP/IP. What Paul Buchheit is claiming is that Bitcoin may be the foundational protocol of all money going forward. But first, a bit of history. To understand Bitcoin and everything that is happening right now, it’s important that we start from the beginning. This movement started with the Cypherpunks. The name is a combination of Cyberpunk, a science fiction subgenre, and Cypher, a word meaning code. The ideas of this group trace back to a cryptographer named David Chaum. He wrote about cryptography, reputations systems, and digital cash in a paper called "Security without Identification: Transaction Systems to Make Big Brother Obsolete" in 1985. His ideas spawned a lot of interest and and in 1992 a mail group named Cypherpunks was formed by Eric Hughes, Timothy May, and John Gilmore. Within two years the mail group had grown to 700 subscribers. Three years later the group grew to over 2000 subscribers. In keeping with the spirit of the ideas and interests of the group, the distribution lists was reworked to be a distributed network of independent mailing nodes to eliminate a single point of failure. This meant that if any single mail server went offline, the emails would still go out.

You have to understand the spirit of the times to fully appreciate why they took this step to distribute their mailing list. The ideas discussed in this group were radical and, borderline illegal, at the time. The right to have a truly private conversation was not well established with the government. In fact, cryptographic methods of securing private communications were legally regulated by the government and treated like munition exports. You can easily understand the idea that sending a shipping container of explosives to your buddy through the mail is super illegal, right? Well that's how encryption codes were treated under the law at the time. There was a sense among technologist that something had to be done if we were not going go to slide into a totalitarian dystopian. It was understood that the only way to prevent this slide was through technological force, not legislation. The members of the Cypherpunks had a laundry list of things they believed would prevent this slide into totalitarianism. The first on that list was publicly available and easy to use strong encryption. That was achieved with the advent of public key encryption and PGP, an easy to use email encryption standard. Some other things they wanted was an anonymous reputation system and a truly digital version of cash. They inadvertently and, probably by accident, got a version of this in seed form with the invention of something called Hashcash.

**Hashcash**

“What we want is fully anonymous, ultra low transaction cost, transferable units of exchange. If we get that going… the banks will become the obsolete dinosaurs they deserve to become.” – Adam Back (inventor of Hashcash, a precursor to Bitcoin)

Remember the Cypherpunks mailing list and how large it got? Well it became a tool of spammers and pranksters. Spammers would send what amounted to adds to the subscribers of the list and pranksters would sign people up without their knowledge so that their inbox would be flooded with unsolicited emails. 

A method of dealing with this was proposed by Adam Back in 1997 and it was called Hashcash. Hashcash is one of the first proof-of-work systems devised and it’s the very way that Bitcoin and most other cryptocurrency mining works. Before you can appreciate Hashcash, let’s take a minute to understand hash functions.

Hashes are very important and you must understand them if you want to understand Bitcoin. I won’t get too technical so don’t get scared. A hashing function is basically a program that turns any peace of text into a string of letters and numbers. The same input will produce the same output string of characters but it's supposed to be impossible to determine the original input text from the output hash. It only works one way. Hash functions use something called trapdoor math. Trapdoor math is used to create trapdoor functions. A trapdoor function is a mathematical operation that makes it easy to do something in one direction but very hard or impossible to do it in the opposite direction. 

Let’s look at an example. There are many hash function algorithms. Popular ones include MD5 and SHA-1. We’ll use MD5 in the following example.

Input text: "Hello-world!"

Output hash: a1ae58346a28449db615e6a17cb79bd6

Input text: "I like red houses"

Output hash: 7b34beb55dac39b7da01975ec014f805

There are a few things to notice here. One. It’s impossible to convert a hash back into the original input text or clear text as its called. Two. Any change to the input text at all will result in a different hash. A change in a single character will result in a different hash. This mathematical sleight of hand is useful in many ways. It’s used in the way that passwords are stored or rather not stored. It’s best practice for computer systems to never store actual passwords but only their hashes. Storing actual passwords would mean that a single breach of a web service would expose all users passwords. This would be very bad. Hashes are also used to ensure that a file has not been changed. The creator of a document or piece of software can publicize the hash of their work and people who want to download it can compare the hash of the download to ensure they have the unaltered version of the said document or software. 

Now that you have a rudimentary idea of what hashes are, let’s come back to Hashcash. The Cypherpunks mailing list got so huge and spam had become a problem so Adam Back had the idea of requiring a special hash on every email in order to send it through the distribution list. The input of the hash would be the senders address, the recipient’s address, and a timestamp all hashed with a required leading number of zeros. If the first hashing attempt didn’t produce the leading zeros then the sender would re-run the hashing function with the updated timestamp until the leading number of zeros was achieved. Here's the cool part. It takes processing power to get the hash to have that special property so it has to be run over and over again until it’s achieved. Computation cost money so this digital stamp makes it costly for spammers to spam users of the mailing list. It was a proof of work digital stamp. It seems simple but this is in fact the very beginning of Bitcoin in seed form. So at this point we have a hash that cost something to create. We could treat this hash like a store of value or a kind of money. How then do we keep track of this ‘money’? This is where the concept of a Blockchain comes in.

**Blockchain**

"On the Blockchain, no one knows you're a fridge" - Richard Brown, Global bank and blockchain consultant 

In 1993, The New Yorker published a comic showing a dog sitting at a desk in front of a computer talking to another dog. The caption read “On the Internet, nobody knows you're a dog.”. It captured the idea that you can be anyone on the Internet. Years later, after the advent of always connected appliances (IoT) and Blockchain technology, Richard Brown repurposed the words of this iconic comic strip to illustrate a similar phenomena. On this thing called the blockchain, it’s impossible to tell a machine from a person. So what is this blockchain and how does it fit into Bitcoin? 

The cypherpunks wanted real digital cash, not just a payment processor like 

PayPal. PayPal is what you would call an intermediary. PayPal keeps track of how much money everyone has and moves money from one person's account to another person's account upon request. 

PayPal acts as an authority to keep track of who has what amount of money and tracks when one person sends another person money. Note that this intermediary, simply by being an intermediary, has the ability to make rules on who can send money for what and enforce certain rules. They can also do chargebacks. That is, they can take money from someone's account without their permission or even freeze their funds pending investigation. Financial intermediaries actually have legal requirements to comply with know-your-customer (KYC), Anti-money laundering (AML), and anti-terrorism laws. 

What we need to achieve to create digital cash is scarcity. It's really hard if you think about it. A prerequisite to a currency is scarcity and digital items, by definition, are not scarce. You can copy and paste a digital file ad infinitum. We somehow have to address the double spend problem. How do we make it so that a person can’t spend the same money twice?

I asked a friend this question and her first response was that you need some central database to keep track of all the transactions. This is a correct first impulse. But then you have to ask, where is this database and who maintains it if it’s not governed by a single party? If PayPal doesn’t maintain the database of transactions, then who does? The answer is that everyone has a copy of it. This is the Blockchain. The Blockchain is an example of what’s called distributed ledger technology.

Ok, if everyone has a copy then how do they stay in sync? How does it keep from saying different things from person to person? This is where a consensus protocol comes in. You hear the word consensus so the first thing that should come to mind is voting. That's right, there is an algorithm that takes a kind of vote between everyone's machines to determine the state of truth. There is a race involved in this too. The first person to state an accurate view of the entire network at a given point is awarded with Bitcoin. This is what mining is. Now there are other methods of achieving this concesis so people have created other type of consensus protocols but the one that bitcoin uses and is most common is call proof-of-work. 

We almost have all the pieces necessary to create a digital currency. We have Hashcash (a store of value), a distributed ledger database (the Blockchain), and a method for keeping everything synched up (a consensus algorithm). There's one last piece we need to make our digital currency work and it’s a way to know who is sending who money. We need a full-proof way to authenticate users of the Blockchain. We get that with digital signatures and digital signatures are possible with public key encryption.

Public key cryptography is a marvel and it will be invaluable for you to understand it if you want to understand Bitcoin and all other Cryptocurrencies. Prior to this form of cryptography people just used a basic password style encryption. You would encrypt a file with a password and then need to share that password with the person you wanted to be able to decrypt it. You would need to have some secure channel of communication for the sharing of this password or the whole thing wouldn’t work. 

Imagine that you wanted to have absolutely secure email communication with someone. You are not sure if the emails are being intercepted and read before being passed on to the intended recipient so you want to encrypt them. How do you get that password to the other person for decryption? If you use the same email channel then it defeats the whole purpose because that’s the very communication channel you are unsure is secure. There is also the danger of this decryption password being shared with others inadvertently. Once the genie is out of the bottle, it can’t be put back in. Using the same key for encryption and decryption is known as symmetric encryption. 

Public key cryptography (PKC) changes all of this. This is the way it works. A user has two keys. One is public and one is private. You can give your public key to anyone. You can publish it online, add it to email signature, or have it in your social media bio. There are even organizations whose sole purpose is to act as public key authorities. Anyone can encrypt a piece of information with this public key. But here’s the catch. Something encrypted with a public key can only be decrypted with its paired private key. This two-key mechanism does away with the need for a secure channel to transmit a key. It’s known as asymmetric key encryption. What’s really cool is that it works in the reverse way too. You can encrypt something with your private key and it can only be decrypted with your public key. This scheme serves two purposes. It allows anyone to encrypt something with a public key and only the person with the paired public key can decrypt it. It also creates a mechanism for identity verification because a person can encrypt something like, let’s say a signature, and the public can know for sure that that signature came from the real private key holder because it can only be decrypted by the associated public key. So PKC serves as a secure encryption mechanism and a digital signature mechanism. It’s really incredible.

Now we have all the ingredients to make the world's first cryptocurrency, Bitcoin. Let’s look at what happened when Bitcoin burst onto the scene. 

**Bitcoin**

“PayPal had these goals of creating a new currency. We failed at that, and we just created a new payment system. I think Bitcoin has succeeded on the level of a new currency.” – Peter Thiel (venture capitalist, founder of PayPal, early investor in Facebook)

In 2008, in the midst of the world's financial crisis, a paper and a piece of software were published online by someone named Satoshi Nakamoto. No one knows who Satoshi Nakamoto is. Satoshi could even be a group of people. People have even claimed to be him but his identity is, to date, an inscrutable mystery. The paper titled “Bitcoin: A Peer-to-Peer Electronic Cash System” explained how the whole system worked and the software was published to a public repository for anyone to download and run. This application could be used to send, receive, and mine Bitcoin. Notably, The Bitcoin algorithm only permits the creation of 21 million bitcoins so it’s supply is finite which means more Bitcoin can’t be printed like what happens with the US dollar and the Federal Reserve.

This should have been a major wakeup call to the world for here was a system that eliminated the need to have financial intermediaries. Consider the following. What will arrive faster? A brick mailed from China or a $20 transfer from one bank account to another? Believe it or not, the brick would arrive sooner. Another thing to consider is micropayments. Because the existing banking system is so inefficient, it’s prohibitively expensive to move payments around for under a dollar.

Bitcoin leveraged all the previous insights and innovations to create our first real digital cash. Even so, only a few computer hobbyist and the Cypherpunks paid attention to Bitcoin. People with vision knew that a copernican revolution had occurred but it would take a few years to manifest this. 

The first people to download and send each other Bitcoin were the Cypherpunks. In the next two years, the price of Bitcoin fluctuated from $.30 cents to $30 dollars. The first known commercial transaction of Bitcoin was for pizza delivery.  May 22 is celebrated as Bitcoin Pizza Day because on it two Papa John’s Pizzas were purchased by Laszlo Hanyecz for 10,000 BTC. At that time, the worth of 10,000 BTC was $41. In today’s terms, those pizzas cost over $25 million dollars. 

Bitcoin started to become more and more popular especially as it was used for illegal purposes and whenever an exchange was robbed and made the news. These instances may have temporarily knocked the price down but the rise of Bitcoin eventually shot back up. 

If fact, it’s this unstoppability that makes it so appealing. Bitcoin can’t be banned. This has not stopped people from trying tho. Several states like Bangladesh, Bolivia, Thailand, and Vietnam (among many others) have attempted to stop the rise of Bitcoin through regulation. Other countries like Australia, Russia, Japan, and Venezuela have made Bitcoin an official legal tender and are trying to regulate it.

Since 2008, Bitcoin has consistently been making a profit (except for 1 year) and is currently valued at $6,300 dollars. In addition to that Blockchain and cryptocurrency-focused startups have raised almost $4 billion through venture capital investments in the first three quarters of 2018. At present, the current mining power of Bitcoin’s network is 300 times more powerful than the world’s top 5 supercomputers combined.

**Drugs and Gambling**

“You can’t stop things like Bitcoin. It will be everywhere and the world will have to readjust. World governments will have to readjust.” – John McAfee (founder of McAfee Inc.)

It should come as no surprise that the first and most publicised use of the new pseudo anonymous digital currency was activities forbidden by the government. Drugs, money laundering, and gambling. Market places used to buy and sell drugs like Silk Road exploded on the scene. These sites operated on The Onion Router (TOR). They were not impervious to attacks from governments because any system, no matter how well engineered for privacy, are still liable to the ultimate weakness. Human error. The infamous Ross Ulbricht made the mistake of using a public wifi network to access secured as well as unsecured internet services thus exposing himself. In the final attempt to grab the mastermind behind Silk Road a federal agent posed as a potential Silk Road moderator. Agents goaded him into logging into his Silk Road account and also physically distracted him while they prevented him from closing his laptop thus preventing his full disk encryption from initializing. The takedowns of Silk Road which generated over a billion dollars in sales only led to increasingly complex upgrades to the TOR network to make the exposure of private services (secret websites on tor) even more difficult. Other cryptocurrencies with absolute privacy built-in came on the scene like Zcash.

If one feels like the above is reason enough to fight the spread of digital currency, then you would have to direct the same criticisms to cash itself. All technology is a double edge sword. The same technology that can power a million homes can create a nuclear bomb. 

Gambling has been a huge outlet for Bitcoin. If you have not picked up by now then you should realize that any activity that a person tries to control like the government is going to be bypassed by a technology like Bitcoin. Individuals want to do what they want. Gambling is no different. Enter Satoshi Dice. The most pure expression of gambling ever devised. 

It works like this. There are specific wallet addresses owned by Satoshi Dice. They have specific public address that have different odds per address. One address might have a 50% chance of winning. A person can send any amount of money to that address and they will have a 50% chance of of winning. If they win, the winnings will be sent directing back to the sending account. The service uses a specific public method for determining the random number generation that determines whether one wins or loses. There is no website or registration necessary to gamble. Satoshi Dice was one of the first forms of crypto based dice games. Many more followed. 

**Security**

“Bitcoin will do to banks what email did to the postal industry.” – Rick Falkvinge (Swedish politician)

Real bank robberies are the stuff of movies. Consider the traditional bank robber. He has to physical show up at the bank and physically get away from the bank as soon as possible. The typical bank robberies take is between $5k and $7k. 

This is in stark contrast to Bitcoin heists. Bitcoin heists range between ten and hundreds of millions in losses and no physical access is needed. No ski masks or getaway car. No police chase or exploding paint bombs. No serial numbers or berried bags of money. Its virtually untraceable and anyone at a keyboard is a potential threat. 

This is not only a temptation to bank robbers but to the operators of online wallets and exchanges as well. They could wake up one day and just decide to run off with everyone's money or even claim that they were hacked to cover their tracks. This has happened several times. I was robbed in the early days of online wallets through such an attempt. 

Since Bitcoin launched there have been more than a billion dollars in robberies. Note that this does not include private robberies like one person getting their coin stolen from their personal machine. This is only counting high profile exchange and online wallet heists. Let’s just look at the year 2017. 

In 2017 NiceHash got taken for $63 million and had to file bankruptcy hours later and in that same year a bug in the Parity crypto wallet allowed hackers to steal $155 million. What’s crazy about this hack was that white hat hackers noticed the anomaly and discovered the Parity bug and the only way to prevent everyone else’s money from being stolen was to steal it first and then give it back to the owners after the bug was resolved. 

There has probably never been a time where the security and stability of software is more important. One could argue that NASA and medical devices already carry this kind of scrupulously but those are cathedral examples where a single highly funded organization produces a product. But software that stores, trades, and interacts with these new digital currencies can be created by anyone move any amount of money in seconds. This ecosystem is more reminiscent of a bazar rather than a cathedral. 

Bitcoin and cryptocurrencies have gained a great level of acceptance by now. The securities and exchange commission has made rules regarding crypto and exchanges that want to operate within the confines of the law are required to comply with the same KYC, AML, and ATF laws.

As you might already expect, user of the new digital currencies don't like being told what to do so an entirely new breed of exchange has come to pass. The distributed exchange. This type of exchange has similar properties to the digital currencies themselves. They are disintermediated and secured using multi sig and smart contract architecture.

You have seen the endless headlines about Bitcoin in the last several years. They have mostly been recovered from an investor's standpoint. While it is true that fortunes have been made and lost on bitcoin, the true value of bitcoin and blockchain technologies is in the utility, not seen as an investment vehicle. It will lead, I believe, to an entirely reimagination of the internet.

**Brain Wallet**

If you lose your Bitcoin private key, you lose your bitcoins. James Howells, an IT guy, lost 7,500 bitcoins in November 2013. While he was cleaning his desk, he threw away his hard disk containing the private keys of bitcoins which he had mined three years earlier. The realization dawned on him when he read news of people making a fortune from Bitcoin. He searched and searched, but could not find his hard drive. At present, the worth of 7,500 BTC is over 20 million dollars. Without the private key, the funds are lost forever no one can use them.

Bitcoin wallets don’t “exist” in any place in particular. Remember, we are dealing with encryption patterns and hashing algorithms. If you could memorize a bunch of numbers and letters, you can access your bitcoin wallet from any node connected to the blockchain. There’s a way to memorize this information that’s a little easier than than memorizing long strings of random alphanumeric characters. You can create a list of English words that convert to those alphanumeric characters but are easier to memorize. If you memorize this strange phrase you can, effectively, have your entire wallet completely in your head. You could evacuate a hostile country with nothing but the clothes on your back and when you finally got access to a computer, reinitialize your wallet, and have access to all your money. This is known as a brain wallet. The phrase you must memorize is called your seed phrase. If the person with the memorized seed phrase dies or is incapacitated, the money will be lost forever. An example of a seed phrase might be: “witch collapse practice feed shame open despair creek road again ice least”. You could make up your own rather than letting wallet software do it but humans are very bad at picking things with the required complexity to produce adequate security.  

**AltCoins and DApps**

“The first generation of the digital revolution brought us the Internet of information. The second generation — powered by blockchain technology — is bringing us the Internet of value: a new platform to reshape the world of business and transform the old order of human affairs for the better.” - Don Tapscott, World thought leader on innovation

While bitcoin was the first of its type, other forms of digital currency all utilizing the same underlying technology (Blockchain) came on the scene all holding particular properties. Almost all of these coins could be referred to an utility tokens. That is, they gave the holder some ability within the network that non holders do not possess. These others forms of digital currency are referred to as altcoins.

There are over 1600 altcoins or utility tokens as of today and anyone can make another one very easily. In fact, the creation of new products with an associated altcoin has become somewhat of a fad. There are even dating websites that have launched with their own associated utility tokens. It’s reminiscent of Chuck E Cheese or arcades of old where you had to buy their special tokens before you could play any of their games. 

Two additional manifestations of Altcoins are stable coins and security tokens. A stable coin is a cryptocurrency that is pegged to a known asset. This is usually accomplished by starting with a reserve of the target asset. For instance a crypto named Tether directly pegs the value of one of their tokens to the US dollar. Another crypto called TrueCoin sets itself apart by providing an open audit of its currency reserves and plans to incorporate other currencies like the Euro and Yen. The other manifestation of crypto asses is called a security token. A security token tries to act as a token representing a standard financial security like a stock or bond and legally comply with all securities and exchange laws. Polymath is a platform designed to make it easy for corporations to easily issue security tokens on the blockchain. 

Things have quickly moved beyond altcoin tho. A writer for Bitcoin magazine and programmer named Vitalik Buterin came up with the idea of running entire programs on a blockchain. This idea resulting in the first blockchain application platform called Ethereum. Ethereum is different in that, while Bitcoin enables the sending of money from person to person, Ethereum enables the creation of programs that move money around given any specified preconditions. Only the most basic of programming is possible with Bitcoin. Namely multisignature requirements for transactions. Ethereum is a Turing complete language meaning that anything that is computable can be computed by Ethereum. these type of programs are called smart contracts or DApps. They are smart in the sense that when deployed they will execute themselves and not on any particular machine. You could say that they exist on the blockchain protocol itself. 

Much like apps, these DApps they are called for distributed apps truly operate in the ether. We are prone to speak of the cloud and might be tempted to think that the cloud is just floating out there but tradition cloud services are just servers running somewhere else, either in a Google or amazon's data center. Traditional apps exist on a physical machine, have a specific ip address, and have to use a payment processor if they want to move money around. They can be taken down or seized or just fail to run if the data center goes offline. DApps, meanwhile do not exist on a particular machine with a specific ip address. They exist on every machine connected to the network and execution is guaranteed. Even if a global electromagnetic pulse where to go off and kill every electrical device on the planet, blockchain nodes running on satellites in space would communicate with the earth's system when brought back online the blockchain would rebuild itself and that DApp would execute. 

**The Future**

“Whereas most technologies tend to automate workers on the periphery doing menial tasks, blockchains automate away the center. Instead of putting the taxi driver out of a job, blockchain puts Uber out of a job and lets the taxi drivers work with the customer directly.” - Vitalik Buterin

I spoke about Etherium in passing but it has dramatically changed the landscape of blockchain technology. It’s not the blockchain development platform. There are others like EOS, Tron, and NEO to name a few. They all compete in areas of ease of development, speed, scalability, governance structures, and differing consensus algorithms. The market cap of these platforms is not in the millions but in the billions. 

This type of thing has given rise to entirely new type of entities. Organizations that exist with no human ruler. Machines that own themselves and finance their own repair. Machine democracies. Real Skynet systems. One of the first decentralized autonomous organizations (DAO) actually chose as its name The DAO. It was an investor-directed venture capital fund. The purpose of The DAO was to demonstrate an entirely new business model based on an open source smart contract. It exist as a smart contract on the Ethereum blockchain and had no conventional management structure or board and not tied to any particular nation state. It started via an initial coin offering (ICO) and, as a result, set the record for the largest crowdfunded campaign in history.

Shortly after the money was raised a group of hackers discovered a bug in the smart contract and were able to steal a third of the money raised. The Ethereum community decided to hard-form the blockchain thus undoing the theft but also created two versions of Ethereum. 

Let’s look at a few other examples of of cryptocurrency innovation. Filecoin is a decentralized storage network. It’s kind of like Dropbox meets Uber. You are paid for storing peoples files. It uses a file system from the future called the InterPlanetary File System (IPFS). It has its own coin, is traded at multiple exchanges and raised $257 million dollars when it launched.

Let’s look at another crypto innovation called Tezos. You know how blockchains offer incentives to people to keep them in sync via a concesis algorithm? Well Tezos does something similar but for the improvement and maintenance of its own code. One attack vector for someone trying to influence a blockchain is through the updates being made to its prottocal being worked on by developers. Its like what happened with the DAO hack. The development team decided that they wanted to “undo” the theft of the transactions so they wrote an update to the Ethereum code to make that happen. 

Tezos creates a mechanism on its protocol itself to enable updates like that to happen based on votes within the chain itself. It moves governance away from from a team of developers to the members of the network. It incentivises upgrades to its self. It calls itself a digital commonwealth. This is very deep stuff. Pure science fiction but its reality and its happening right now. The Tezos project raised $232 million. 

There have been innovations in other areas of blockchain technology related to trade as well. If you have one form of altcoin and you wanted to trade it for another type of alcoin you would typically have to find someone who wanted to trade. The other person is called the counterparty. This situation can make it difficult because there are now so many different cryptocurrencies and any particular exchange only has so many users that finding someone who wants to exchange crypto X for crypto Y becomes increasingly difficult. 

The Bancor Network changes all that. It allows one to convert between any two tokens with no counterparty at a algorithmically calculated price. The Bancor Network raised $153 million when it launched. Another technology that does something similar is Polkadot. Polkadot is described as a heterogeneous multi‑chain technology. It enables transactions to be spread out across differing token chains using specialised parachains called bridges. Polkadot raised $144 million.

Even supercomputers are being reimagined as blockchain entities. Golem is a global, open source, decentralized supercomputer that anyone can access. It is made up of the combined power of users’ machines. Golem creates a decentralized sharing economy of computing power and supplies software developers with a flexible, reliable and cheap source of computing power. Golem raised over $8 million when it launched.

**Conclusion**

As you can see, while there are fad applications of blockchain technology there are many more genuine innovations being built on this technology that have the potential to change the world. We have moved into an information driven economy and the Internet is the superhighway of that information. The creation of Bitcoin and blockchain technology in general has opened up valuer and commerce to that superhighway. Many believe that the very backbone of the Internet is going to be reimagined with the appearance of Blockchain. One thing is certain, the genie can't be put back in the bottle and rather than turning the clock back, changes are happening at an exponential accelerated rate. Old media companies took decades to grow into the conglomerates they are now while new natively digital media outlets go viral and rival their classical counterparts in a fraction of the time. I thinks it’s reasonable to suggest that similar radical changes will happen in the realm of financial technology with these new technologies. Some established financial organizations are embracing these technologies like JP Morgan and have launched their own private blockchain platforms. The ones who don't will not survive. 

**About the Author**

Justice Conder is a software developer, IT project manager, and technical writer. He enjoys building proof of concept applications using bleeding edge technology, evangelizing new technologies, and building and coaching teams in Agile methodologies. He’s worked with fortune 500 companies as well as founded and sold multiple startups. In addition to building software and software teams, Justice loves reading and writing science fiction. His writings has been quoted by the likes of ZDNet and Daring Fireball. You can learn more about his work at justiceconder.com
