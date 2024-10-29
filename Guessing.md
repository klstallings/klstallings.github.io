    ```mermaid
flowchart TD
    A[Start] -->|Initialize Game| B(Set up necessary variables such as attempts, score, and any game state)
    B --> C[Generate Random Number]
    C -->|Prompt User for Guess| D[Ask the user to input their guess]
    D -->|Is Input Valid| E[Check if the user input is valid] 
    E -->G[Yes: If valid, proceed to check the guess]
    E -->H[No: If invalid, provide an error message and return to prompt for input]
    G -->|Check Guess| F[Compare the user's guess with the generated random number]
    F -->I[Too Low: Provide feedback that the guess is too low and return to prompt for another guess]
    F -->J[Too High: Provide feedback that the guess is too high and return to prompt for another guess]
    F -->K[Correct: Provide a congratulatory message that the guess is correct and end the game]
    I -->L[End: The game concludes]
    J -->L[End: The game concludes]
    K -->L[End: The game concludes]
    ```