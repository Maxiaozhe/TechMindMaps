## Bot frameWork core
### Mvc
```mermaid
graph TD;
A[BotController];
B[Adapter];
C[Bot:IBot];
D[logger];
E[Dialog];
F[userState];

A-->|PostAsync|B;
B-->|OnTurnError|D;
B-->|ProcessAsync|C; 

```