# random-mermaid
flowchart TD
    Start([Start]) --> GenerateNumber[Generate Random Number Between 1 and 100]
    GenerateNumber --> InputGuess[Prompt User for a Guess]
    InputGuess --> ValidateInput{Is Guess a Valid Number?}
    
    ValidateInput -->|No| InvalidInput[Display Error: Enter a Valid Number]
    InvalidInput --> InputGuess

    ValidateInput -->|Yes| CheckGuess{Is Guess Within Range?}
    
    CheckGuess -->|No| OutOfRange[Display Error: Guess Out of Range]
    OutOfRange --> InputGuess

    CheckGuess -->|Yes| CompareGuess{Is Guess Correct?}
    
    CompareGuess -->|Yes| CorrectGuess[Display: Correct! You Win]
    CorrectGuess --> End

    CompareGuess -->|No| HighLow[Is Guess Too High or Too Low?]
    
    HighLow -->|Too High| DisplayHigh[Display: Too High! Try Again]
    DisplayHigh --> InputGuess

    HighLow -->|Too Low| DisplayLow[Display: Too Low! Try Again]
    DisplayLow --> InputGuess

    End([End])
