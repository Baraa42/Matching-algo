# Matching-algo
Algorithm for matching orders ( for betting )
```
Address Object {
string Hex // player address on chain
}

Bet Object {

  String player_address, // Hex string player address on chain
  Float stake;
  Float odds; // odds > 1 increment by 0.01 . valid odds =1.01 1.02 ...
  string selection; // home away draw
  string betType; // Back/Lay
  string betStatus ; // Unmatched, Matched, Partially Matched
  string selectionStatus; // Open, Win, Lose
  int betId;
  
 }
 
 array allBets[] // array/list of Bet object holding bets by their Id
 
 array/dict playerPayout[] // hold data of player payout : Player -> Selection -> Payout
 
 function placeBet() // matches the bets update bet status update playerpayout etc 
```
