```Mermaid
flowchart TD
Start([Start]) --> GenerateRandomNumber[/Generate Random Number\]
GenerateRandomNumber[/Generate Random Number\] --> PromptUserForInput[\Prompt User For Input/]
PromptUserForInput[\Prompt User For Input/] --> CheckInputIsNumber[/Check the Input Is a Number\]
CheckInputIsNumber[/Check the Input Is a Number\] --> IsIt[\Is It?/]
IsIt[\Is It?/] --> |Yes| MatchAgainstGeneratedNumber[/Match it Against the Generated Number\]
IsIt[\Is It?/] --> |No| PromptUserForInput[\Prompt User For Input/]
MatchAgainstGeneratedNumber[/Match it Against the Generated Number\] --> DoesItMatch[\Does it Match?/]
DoesItMatch[\Does it Match?/] -->|No| PromptUserForInput[\Prompt User For Input/]
DoesItMatch[\Does it Match?/] -->|Yes| End([End])
```
* The First step is to start the game, then upon starting the game generates a random number. 
* After that number is generated it will prompt the user to guess that number by asking for input. 
* Once that input is recieved it will check the input to make sure it is a number, which if it isnt' it will loop back to asking for input, and if it is the game will then check to see if it matches the random number generated. 
* If the number does not match the number generated the game will loop back to askinf for input, if it does match, the game will then end.
