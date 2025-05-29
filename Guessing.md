# Random Guessing Game Flowchart
#### This diagram illustrates the logical steps a game would take that generates a random number from 1 - 100 and prompts the user for guesses.

```mermaid
flowchart TD
    A[Start] --> B{Generate a random number 1 - 100}
    B --> C{Prompt the user for a number}
    C --> D[Is the input a valid number 1 - 100?]
    D -->|No| E[Error Message] --> C
    D --> |Yes| F[Is the guess correct?]
    F -->|Yes| G[Correct! Message]
    F -->|No| H[Is the guess too high or too low?]
    H -->|High| I[Show Too High Message] --> C
    H -->|Low| J[Show Too Low Message] --> C

