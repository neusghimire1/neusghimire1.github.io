```mermaid
flowchart TD
    A([Guess a number]) --> |Ask for integer value| B(Test guess against actual value)

    B --> |One| C[Guess too low]
    C --> A

    B --> |Two| D[Guess too high]
    D --> A

    B --> |Three| E[Guess not valid, may come from not being an integer or float]
    E --> A

    B --> |Four| F[Correct guess!]
```

