# 3.1 GET utility diagrams

Below are two high-level diagrams that illustrate how users and event organizers interact with the GET Protocol, and how GET facilitate these interactions. Figure 4 shows the GET utility of the most common protocol case: a consumer buying and using a ticket for an event. Table 6 lists the contracts displayed in the diagram. The bullet points describe the steps A-E that are taken by an end user who buys a smart ticket on the protocol. 

The diagram in Figure 5 below describes the secondary market mechanics happening on the GET Protocol. If an user with a ticket wants to sell their ticket, the smart ticket can be offered to the event-specific secondary market built into the protocol. In this event-specific secondary market, tickets are sold for their original selling price alongside the tickets of the event organizer \(also known as the primary ticketing market\).

| Contract | Description |
| --- | --- | --- | --- |
| 1 | Event Ticketing Contract \(ETC\) - This contract is owned by the event organizer. In addition to being the instantiator and managing contract of all the smart tickets of the event, this contract is also a wallet that contains GET purchased by the event organizer. |
| 2 | Primary / Secondary Market Contract \(PSMC\) - This contract acts as a central matching market for both the tickets sold in the primary market \(by the event organizer\) and the tickets sold in the secondary market. After receiving a GET token from theUSTC contract, this contract will return a valid ticket to the USTC contract.  |
| 3 | User Smart Ticket Contract \(USTC\) - This contract manages the GET users with valid tickets and is responsible for serving the QR code to users with these tickets right before the event starts. For providing this service the contract receives GET from those who use the contract. |

_Table 6: Functions and roles of the three contracts labelled in Figure 4 below._

![Figure 4](../../.gitbook/assets/image%20%2811%29.png)

_Figure 4: The process of consumer verification and the purchase of a smart ticket on the GET Protocol. Note that the tokens the user receives after purchase of the smart ticket are partially used by different smart contracts of the GET Protocol. This diagram also shows the role of the event organizer within the protocol._

## Step A-E of Figure 4 explained.

* A: An unknown customer enters the protocol with the intention to buy a ticket. If the user’s phone \(or web browser\) is unknown to the protocol after signing in \(meaning the user never used his phone to buy   a ticket on the protocol\), the user will be asked to create an account on the protocol by providing some   basic user data. 
* B: In the account creation phase \(A\) the user has provided the protocol with a phone number. In   the following step, the phone number will be verified by means of an SMS/text message containing a   verification code. 
* C: At this point the user will be shown an interface in which he or she is able to pay for the ticket using   the available payment methods. The user will need tokens in order to interact with the protocol, so the   price of the GET that the user will need is included in the ticket price. The event organizer \(see Contract  1 / ETC\) has already purchased GET from the open market. These GET are available for distribution to   the event attendees and thus will be sent to the user’s wallet when the user completes the FIAT payment   via the payment processor. 
* D: After payment is completed, the API will send the required amount of GET tokens to the USTC   contract. At this point in the process, the user will buy the USTC contract. This contract will forward an   amount of GET to the PSMC contract, which will transfer the user an available smart ticket object. This   object is controlled by the USTC contract. 
* E: At the event horizon \(the moment an event begins\) the PSMC contract activates all of the users’ smart   tickets, delivering the QR codes needed for entry to the ticket owners’ verified phones.

![Diagram 5](../../.gitbook/assets/image%20%2810%29.png)

_Figure 5: The mechanics of secondary ticketing market. Note that both the seller of the smart ticket as well as the buyer of the ticket pay an amount of GET to the PSMC contract \(depicted as ’Secondary market’ in Figure 4\). For the seller this payment will cover the costs of FIAT settlement of the ticket by the payment processor to his or her bank account. For the buyer this payment will cover the regular FIAT and processing costs also displayed in Figure 4._

