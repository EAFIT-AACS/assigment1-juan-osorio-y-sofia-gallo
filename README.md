[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/95BWY5mA)
DFA Minimization Project

## Student Information
- **Full Name:** Sofia Gallo and Juan Jose Osorio
- **Class Number:** 7309

## Environment
- **Operating System:** Windows 10
- **Programming Language:** Java (JDK 17)
- **Tools Used:** Visual Studio Code

## Instructions to Run the Implementation
1. **Clone the Repository:**
   ```sh
   git clone <repository-url>
   cd <repository-directory>

## Algorithm Explanation
The algorithm implemented in this project minimizes a Deterministic Finite Automaton (DFA) using the following steps:

1. **Mark Pairs of States:**
Initialize a 2D boolean array distinguishable to keep track of distinguishable state pairs.
Mark pairs where one state is a final state and the other is not.

2. **Mark Pairs Based on Transitions:**
Iteratively mark pairs of states as distinguishable if their transitions lead to distinguishable states.
Continue this process until no more changes occur.

3. **Collect Equivalent States:**
After marking distinguishable pairs, collect pairs of states that are not distinguishable.
These pairs represent equivalent states in the minimized DFA.
   
The program reads the number of test cases, the number of states, the alphabet, the final states, and the transition table from the input. It then applies the minimization algorithm and prints the equivalent state pairs for each test case.

## Example Input
 ```sh
    2
    5
    a b
    1 3
    0 1
    1 2
    2 3
    3 4
    4 0
    3
    a b
    0 2
    0 1
    1 2
    2 0
 ```
## Example Output
 ```sh
  (1, 2) (3, 4)
  (0, 2)
 ```
