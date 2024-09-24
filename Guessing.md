```mermaid

flowchart TD
    Start([Start]) --> A[Generate a random number]
    A --> B[Prompt user for a guess]
    B --> C{Is the input a number?}
    C -- No --> D[Display error: Please enter a valid number]
    D --> B
    C -- Yes --> E{Is the guess correct?}
    E -- Yes --> F[Display: Correct!]
    F --> End([End])
    E -- No --> G{Is the guess too high?}
    G -- Yes --> H[Display: Too high!]
    H --> B
    G -- No --> I[Display: Too low!]
    I --> B

```
