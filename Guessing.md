```mermaid
flowchart TD
Start([Start]) -->
state1(Pick a number 1 through 10) -->
state2(Player 1 picks number 7) -->
state3(player 2 guesses the number) --> 
if_state --> Too High: if n < 7
loop to state3
if_state --> Too Low: if n > 7
loop to state3
if_state --> Correct: if n = 7 --> End([END])
```
