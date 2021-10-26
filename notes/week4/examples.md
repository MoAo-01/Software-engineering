

Discover ambiguities or omissions in the following statement of requirements for part of a ticket-issuing system:

An automated ticket-issuing system sells rail tickets.
Users select their destination and input a credit card and a personal identification number.
The rail ticket is issued and their credit card account charged.
When the user presses the start button, a menu display of potential destinations is activated, along with a message to the user to select a destination.
Once a destination has been selected, users are requested to input their credit card.
Its validity is checked and the user is then requested to input a personal identifier.
When the credit transaction has been validated, the ticket is issued.

## Suggestion Answer:
### Ambiguities and omissions include:
1. Can a customer buy several tickets for the same destination together or must they be bought one at a time
2. Can customers cancel a request if a mistake has been made
3. How should the system respond if an invalid card is input
4. What happens if customers try to put their card in before selecting a destination (as they would in ATM machines)
5. Must the user press the start button again if they wish to buy another ticket to a different destination
6. Should the system only sell tickets between the station where the machine is situated and direct connections or should it include all possible destinations
7. Train departure and arrival times. Do customers buy ticket for a specific train? Or for any trip along the route? ( If the latter, than no way to tell if all the seats on a train are sold out, or can you do seat assignment?
8. What type of input device (Touchscreen vs Keyboard) system supports
9. Print receipt for ticket details

Write a set of non-functional requirements for the ticket-issuing system, setting out its expected reliability and response time.
## Suggestion Answer:
### Possible non-functional requirements for the ticket issuing system include:
1. Between 0600 and 2300 in any one day, the total system down time should not exceed 5 minutes.
2. Between 0600 and 2300 in any one day, the recovery time after a system failure should not exceed 2 minutes.
3. Between 2300 and 0600 in any one day, the total system down time should not exceed 20 minutes.
4. After the customer presses a button on the machine, the display should be updated within 0.5 seconds.
5. The ticket issuing time after credit card validation has been received should not exceed 10 seconds.
6. When validating credit cards, the display should provide a status message for customers indicating that activity is taking place. 
7. The maximum acceptable failure rate for ticket issue requests is 1: 10000. 
8. The system shall continue to function so long as roll of ticket paper is in the machine, and a network connection is provided for the destination database and credit transactions. 

