# 12.Markov-model
Markov Model and Word Probability Calculation
Let us assume a Markov model having four states:
| State (Si) | Letter | Initial Probability πi |
| ---------- | ------ | ---------------------- |
| S₁         | a      | 0.3                    |
| S₂         | c      | 0.2                    |
| S₃         | e      | 0.1                    |
| S₄         | t      | 0.4                    |
Transition Probabilities (First-Order Model)
| From \ To | a   | c   | e   | t   |
| --------- | --- | --- | --- | --- |
| a         | 0.0 | 0.4 | 0.0 | 0.6 |
| c         | 0.2 | 0.0 | 0.4 | 0.4 |
| e         | 0.5 | 0.0 | 0.0 | 0.5 |
| t         | 0.4 | 0.0 | 0.6 | 0.0 |
### Step 1: Word Probability Calculation
P(word) = π[first_letter] × P(second_letter | first_letter) × P(third_letter | second_letter)

### Step 2: Implement Markov Word Generator
Implement a function that generates words of given length using only uniform random sampling.
You must not use built-in HMM tools (e.g., hmmgenerate in MATLAB or hmmlearn in Python).
### Step 3: Compare with Simulated Frequencies
Generate a large number of 3-letter words (e.g., 1,000,000).
Count the occurrences of the words: cat, eat, act, and tea.
Compare the empirical frequencies with the calculated probabilities from Step 1.

Use uniform random distribution to sample from a finite discrete set.

You can implement sampling using cumulative probability and a single random number between 0 and 1.
![image](https://github.com/user-attachments/assets/0144032d-2599-4b6c-8b35-63cb0a4b82ad)
