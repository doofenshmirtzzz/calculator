# Global structure

Calculator has kind of a state-driven design:

There are a few modules:

1. **Input module**: collects user input

2. **Controller module:** controls the flow, updates the **state** of the calculator

3. **State module:** contains the current state

4. **Calculation module:** performs the calculations on the state called by the controlle

5. **Display module:** displays the current state in a controlled way


Flow (idk, probably):

```
user input -> input -> controller -> state -> controller -> display
                                         ^         |
                                         |         v
                                         calculation
```