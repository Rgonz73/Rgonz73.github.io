## Implementing a Random Guessing Game
```mermaid
flowchart TD
Start([Start]) --> A[Generate number]
A --> |1-10| B[Imput Answer]
B --> C[Is the imput valid?]
C --> |Yes| D{Is the answer correct?}

C --> |No| d{Wrong Imput Please try again}
d --> B

D --> |yes| id1{{You Win}}
id1 --> restart([Restart?])
restart --> |yes| Start

restart --> |no| End

D --> |No| E[Is the imput high or low]
E --> |High| F[Answer is too high]

F --> B

E --> |Low| G[Answer is too low]
G --> B
```
##### This flowchart illustrate how the guessing game works. 
First, it will start by generating a number then it will ask to imput an answer. Then, it the game will verify if the answer is valid. After, it will determine if the answer is correct but if no then it will provide feedback and will sent back to imputing an answer. If the answer is correct then game will ask to restart the game.
