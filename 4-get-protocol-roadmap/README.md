---
description: Introduction
---

# 4 GET protocol roadmap

In this chapter the planned development phases of the GET Protocol will be outlined. But before the future abilities and functionalities of the GET Protocol, code that is yet to be developed and deployed to market are described in detail, it is important to establish what functionalities of the solution the GET Protocol poses to offer the ticketing sector are already validated by the market. Feedback from end-users and the ability to generate actual demand for the concept/product is key when you are incrementally building, improving and scaling the full spectrum solution as described in previous chapters of the GET Protocol whitepaper.

_State of the technology - GUTS Tickets; a operational and competitive smart ticketing company\(2016-2017\)._

The GET Protocol is more than a white paper or a proof of concept. It is already reality. Since 2016 GUTS Tickets has been selling smart tickets registered on the blockchain. GUTS Tickets was officially incorporated in 2016 and ticketed their first blockchain event in Q1 of 2017. The code for this first iteration of the product/proofof-concept was developed and tested in Q3 and Q4 of 2016. In 2017 the first iteration of the smart ticketing application was ready to be deployed in the market. Under the mantra, fail quick, fail often. The ownership state changes registered on the blockchain of the events GUTS Tickets serviced with their smart ticketing application for can be found in the [second tab](https://docs.google.com/spreadsheets/d/1x3mEHiGJ255tDPhJ-UqXvPIh8ma-69hBABHZdPFkb1U/edit#gid=0) of the public Google spreadsheet of the BlockTix/Aventus comparison [blog](https://blog.guts.tickets/get-vs-tix-vs-avt-the-three-main-blockchain-ticketing-projects-bench-marked-part-1-a2686bfdd532) published on the GET Protocol Medium blog.

## Functionalities of a ticketing application.

Throughout this whitepaper the tickets of the GET Protocol have consistently been called ’smart’. What makes  a ticket smart? And if there is something as a ’smart’ ticket what would be a ’dumb’ ticket? The following two paragraphs will establish this difference.

## Dumb tickets.

  
Selling digital tickets for an event via the internet is as easy as having a web-application that is able to process payments \(via one of the many out-of-the-box payment processor integrations available\) and deliver a piece of data to the buyer. After confirmation of a completed payment the web-application should be able to generate and serve an unique QR code\(or other data-holding object\) to the buyer of the ticket. That’s it. This QR code should be unique as the validity of the ticket should verifiable when scanning the ticket at the entrance of the event. This ticketing process described here is not what where the rubber hits the road when it comes to fighting ticket scalpers or other event ticketing inefficiencies. Companies as Ticketmaster where able to build and deploy these types of web-applications web applications in the late 90’s and still do basically the same thing to this day. Replicating such a web-application with all modern programming and hosting tools available in 2017 isn’t hard at all. Running such an ticketing web-application completely on the blockchain is technically possible. Languages as Solidity are Turning complete and will be able to make the calculations needed to compute QR codes and process payments swiftly and transparently. With de-central hosting services like IFPS will be able to host a blockchain ticketing application, making centralized servers like AWS unnecessary. While all this decentralization sounds cool and innovative it is also rather inefficient \(as a centralized server will be able to better to do this all more cost-efficiently\). That’s just logic. 

## Smart tickets.

  
Smart tickets have all of the same functionalities described in the paragraph describing their dumb counterpart above. The only difference is that smart are aware of who owns them and when they are being owned. A smart ticket also ’knows’ under what circumstances the who and when of are allowed to be changed. In practice this means that a smart ticket will not allow changing of its ownership when it is being sold for a higher price than is intentional. In a sense you could call a smart ticket ’aware’. In practice this all comes down to the variables and functions set in the smart-ticket contract. A smart ticket cannot be scalped as it will not allow a overpriced transfer. A QR code smart ticket cannot be faked as it will not serve the QR code to the owner before the owner of the ticket needs it.

## Functionalities of the GUTS smart ticketing application

* Assign wallet Ethereum address to new identity : [Functionality DONE](https://sandbox.guts.tickets) 
* Implement dynamic QR code that can’t be sold/copied : [Functionality DONE](https://sandbox.guts.tickets) 
* Web based smart ticketing application: Working on smartphone browsers. DONE 
* Merge primary and secondary ticketing market: [DONE](https://sandbox.guts.tickets) 
* Register ownership changes of smart-ticket on the blockchain [DONE](https://sandbox.guts.tickets) 
* Scalability/ability of the smart ticketing application to handle high number of user request [DONE](https://sandbox.guts.tickets)

