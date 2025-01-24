```mermaid
flowchart TD
 A[Start] --> B[Initialize Variables]
    B --> C[Generate Random Number]
    C --> D[User Input]
    D --> E{Is userGuess = targetNumber?}
    E -- Yes --> F[Correct Guess]
    E -- No --> G{Is userGuess < targetNumber?}
    G -- Yes --> H[Feedback: Too Low]
    G -- No --> I[Feedback: Too High]
    H --> D
    I --> D
    F --> J[Play Again?]
    J -- Yes --> B
    J -- No --> K[End Game]
    K --> L[Thank User]
