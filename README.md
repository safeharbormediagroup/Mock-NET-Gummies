# Mock-NET-Gummies
 Math Fun Education MOCK Net Gummies

 

============================================================
                   Mock Net Gummies v1.0 
============================================================

[SCREEN 1: THE MAIN CANDY SHOP JAR]
====================
  GUMMY GOVERNOR   
====================
1. Count My Gummy Pouch
2. Magic Candy Tree 
3. Share My Treats
4. Playground Trading Log
====================
-> HOW IT WORKS UNDER THE HOOD:
This is the front door on the user's phone. Pressing a button 
triggers a basic routing switch: 1 pulls up the balance, 2 calls 
the faucet script, 3 opens the sender portal, and 4 pulls up 
the historical trade ledger.

------------------------------------------------------------

[SCREEN 2: THE CANDY TREE PORTAL]
====================
  MAGIC CANDY TREE  
====================
Shaking the branches for 
500 free Gummy Bears...

[SUCCESS!] 
500 GUMMY BEARS added
to your pouch.
====================
1. Back to Main Shop
-> HOW IT WORKS UNDER THE HOOD:
When selected, the system verifies the user's phone ID. If eligible, 
it runs an addition equation on the backend database:
(Current Wallet Balance + 500). It saves the new integer and 
displays the success screen.

------------------------------------------------------------

[SCREEN 3: RECESS TREAT SHARING]
====================
   SHARE SUCCESS!   
====================
Stamp Token:
0x8f3c2a9d1b7e

Sent 100 GUMMY BEARS 
to ALIYAH_LIGHT.
====================
New Pouch: 400 Bears
====================
1. Main Shop
-> HOW IT WORKS UNDER THE HOOD:
The system checks if the sender's balance is greater than or 
equal to 100. If verified, it subtracts 100 from the sender, 
adds 100 to the recipient, generates a random 12-character 
string starting with "0x" to act as a fake block hash, and 
displays the confirmation data.

------------------------------------------------------------

[SCREEN 4: THE PLAYGROUND PRICE MAT]
====================
 LIVE GUMMY MARKET
====================
SANDBOX [A]: 45 JellyBeans
Buyers: 44 | Sellers: 45

SLIDE   [B]: 52 JellyBeans
Buyers: 51 | Sellers: 52
====================
*SWEET SWAP: +7 Beans*
====================
1. Buy Sandbox A (Cheap)
2. Sell Slide B (Dear)
-> HOW IT WORKS UNDER THE HOOD:
The engine tracks two independent variables: Market_A_Price 
and Market_B_Price. A minor background function ticks these numbers 
up or down randomly to simulate volatility. The screen displays a 
live subtraction equation: (Market_B_Price - Market_A_Price). 
If the total is positive, it automatically prints the *GAP DETECTED* alert line.

------------------------------------------------------------

[SCREEN 5: FILLING THE TRADING HAND]
====================
  GUMMY SCOOP [A]   
====================
Scoop: 10 Bears
Price: 45 Beans each
Total: 450 JellyBeans

[CONFIRMED]
10 Bears loaded into 
your tiny pockets.
====================
1. Run over to Slide B
-> HOW IT WORKS UNDER THE HOOD:
When the user triggers the buy option, the system calculates 
the total cost (Amount * Market_A_Price). It checks the user's cash 
balance. If they have enough funds, it subtracts 450 from their cash 
and assigns 10 tokens to a temporary variable called Trading_Hand.

------------------------------------------------------------

[SCREEN 6: THE FINAL CANDY FLIP]
====================
  GUMMY FLIP [B]   
====================
Trading: 10 Bears
Price: 52 Beans each
Total: 520 JellyBeans

[SETTLED]
Original Cost: 450
Gross Return:  520
====================
*BONUS TREAT: +70 Beans*
====================
1. Back to Price Mat
-> HOW IT WORKS UNDER THE HOOD:
When the user routes the trade to the expensive market, the system 
calculates the gross return (Trading_Hand Tokens * Market_B_Price). 
It resets the Trading_Hand variable back to 0, adds the gross 
return (520) back to the user's cash balance, and explicitly subtracts 
the original cost from the return to display the exact Net Profit text.

------------------------------------------------------------

[SCREEN 7: THE PLAYGROUND CHALKBOARD]
====================
 PLAYGROUND TICKER  
====================
[01:12] ALICE got 5  
        @ 45 Beans (Mkt A)
[01:13] BOB flipped 12   
        @ 52 Beans (Mkt B)
[01:13] *Slide Price Drop* Down to 50 Beans
====================
1. Wipe Board Clean
-> HOW IT WORKS UNDER THE HOOD:
Every time any player on the network executes a Buy or Sell function, 
the server appends a plain text string recording the timestamp, name, 
amount, and market price to a shared network file. Opening this screen 
simply reads out the last three entry lines stored in that file.
============================================================
