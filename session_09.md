# Frequentist definition of probability

# Law of Large numbers
- The law of large numbers states that the more experiments we run, the closer we will tend to get tot the expected probability

# Events and Sample Spaces
- Coin Toss example
- Dice throwing example

# Dependent and Independent Events
## Dependent and Independent Events: Examples

**1. Independent Events**

* **Definition:** Two events are independent if the occurrence of one event does not affect the probability of the other event occurring.
* **Example 1: Coin Flips**
    * Flipping a fair coin twice.
    * Event A: The first flip is heads.
    * Event B: The second flip is heads.
    * These events are independent because the outcome of the first flip has no influence on the outcome of the second flip.
    * $P(A) = 0.5$, $P(B) = 0.5$, and $P(A \text{and} B) = P(A) * P(B) = 0.25$.
* **Example 2: Rolling Dice**
    * Rolling two fair six-sided dice.
    * Event A: The first die shows a 4.
    * Event B: The second die shows a 3.
    * These events are independent. The result of one die roll doesn't change the odds of the other.

**2. Dependent Events**

* **Definition:** Two events are dependent if the occurrence of one event affects the probability of the other event occurring.
* **Example 1: Drawing Cards Without Replacement**
    * Drawing two cards from a standard deck without replacing the first card.
    * Event A: The first card is an ace.
    * Event B: The second card is an ace.
    * These events are dependent. If the first card drawn is an ace, there are fewer aces left in the deck, which changes the probability of drawing an ace on the second draw.
* **Example 2: Weather and Outdoor Activities**
    * Event A: It rains.
    * Event B: A person goes to the beach.
    * These events are dependent. Rain significantly decreases the probability that someone will go to the beach.
* **Example 3: Marbles in a Bag**
    * A bag contains 5 red marbles and 3 blue marbles.
    * Event A: The first marble drawn is red.
    * Event B: The second marble drawn is red (without replacing the first).
    * $P(A)$ = $\frac{5}{8}$.
    * If A occurs, then $P(B|A)$ = $\frac{4}{7}$.
    * Therefore, the events are dependent.

# Joint probability
## Joint Probability Example: Ice Cream Preferences

Let's say we're looking at ice cream preferences based on two factors:

* **Flavor:** Chocolate (C) or Vanilla (V)
* **Topping:** Sprinkles (S) or No Sprinkles (N)

We've collected data and summarized it in the following joint probability table:

|             | Sprinkles (S) | No Sprinkles (N) | Total |
| :---------- | :------------- | :--------------- | :---- |
| Chocolate (C) | 0.3            | 0.2              | 0.5   |
| Vanilla (V)   | 0.1            | 0.4              | 0.5   |
| Total       | 0.4            | 0.6              | 1.0   |

**Understanding Joint Probabilities:**

Each cell in the table represents the joint probability of two events occurring together:

* **$P(C, S)$ = 0.3:** The probability of someone choosing chocolate ice cream *and* sprinkles.
* **$P(C, N)$ = 0.2:** The probability of someone choosing chocolate ice cream *and* no sprinkles.
* **$P(V, S)$ = 0.1:** The probability of someone choosing vanilla ice cream *and* sprinkles.
* **$P(V, N)$ = 0.4:** The probability of someone choosing vanilla ice cream *and* no sprinkles.

**Example Explanation:**

* The probability that someone chooses chocolate ice cream *and* sprinkles is 0.3, or 30%.
* The probability that someone chooses vanilla ice cream *and* no sprinkles is 0.4, or 40%.

**Key Points:**

* Joint probabilities represent the likelihood of two or more events happening simultaneously.
* The sum of all joint probabilities in the table is equal to 1.
* The total column and row show the marginal probabilities, as explained in the previous example.

# Marginal Probability

## Marginal Probability Example: Weather and Activity

Let's consider the following scenario:

* **Weather:** Sunny (S) or Rainy (R)
* **Activity:** Walk (W) or Inside (I)

We have the following joint probability distribution:

|             | Walk (W) | Inside (I) | Total |
| :---------- | :------- | :--------- | :---- |
| Sunny (S)   | 0.4      | 0.1        | 0.5   |
| Rainy (R)   | 0.1      | 0.4        | 0.5   |
| Total       | 0.5      | 0.5        | 1.0   |

**Calculating Marginal Probabilities:**

* **Marginal Probability of Sunny (P(S))**:
    * $P(S) = P(S, W) + P(S, I)$ = 0.4 + 0.1 = 0.5
    * Therefore, $P(S)$ = 0.5 (50%)

* **Marginal Probability of Rainy (P(R))**:
    * $P(R) = P(R, W) + P(R, I)$ = 0.1 + 0.4 = 0.5
    * Therefore, $P(R)$ = 0.5 (50%)

* **Marginal Probability of Walk (P(W))**:
    * $P(W) = P(S, W) + P(R, W)$ = 0.4 + 0.1 = 0.5
    * Therefore, $P(W)$ = 0.5 (50%)

* **Marginal Probability of Inside (P(I))**:
    * $P(I) = P(S, I) + P(R, I)$ = 0.1 + 0.4 = 0.5
    * Therefore, $P(I)$ = 0.5 (50%)

**Key Observations:**

* The marginal probabilities are found in the "Total" row and column of the table.
* They represent the probability of a single event occurring, regardless of the other event.

# Conditional Probability

## Conditional Probability with Dice: Even and Odd

Let's use a standard six-sided die to illustrate conditional probability with even and odd numbers.

**Events:**

* **Event A:** Rolling an even number (2, 4, or 6).
* **Event B:** Rolling a number greater than 3 (4, 5, or 6).

**Probabilities:**

* **$P(A)$:** Probability of rolling an even number.
    * There are 3 even numbers (2, 4, 6) out of 6 possible outcomes.
    * $P(A)$ = 3/6 = 1/2.
* **$P(B)$:** Probability of rolling a number greater than 3.
    * There are 3 numbers greater than 3 (4, 5, 6) out of 6 possible outcomes.
    * $P(B)$ = 3/6 = 1/2.
* **$P(A and B)$:** Probability of rolling an even number *and* a number greater than 3.
    * The numbers that satisfy both conditions are 4 and 6.
    * There are 2 outcomes (4, 6) out of 6 possible outcomes.
    * $P(A and B)$ = 2/6 = 1/3.

**Conditional Probability: $P(A|B$)**

We want to find the probability of rolling an even number, *given* that we've rolled a number greater than 3. In other words, P(A|B).

* **Formula:** $P(A|B) = \frac{P(A and B)}{P(B)}$
* **Calculation:** $P(A|B)$ = (1/3) / (1/2) = (1/3) * (2/1) = 2/3.

**Therefore, the probability of rolling an even number, given that you've rolled a number greater than 3, is 2/3.**

**Conditional Probability: $P(B|A)$**

Now, let's find the probability of rolling a number greater than 3, *given* that we've rolled an even number. In other words, P(B|A).

* **Formula:** $P(B|A) = \frac{P(A and B)}{P(A)}$
* **Calculation:** $P(B|A)$ = (1/3) / (1/2) = (1/3) * (2/1) = 2/3.

**Therefore, the probability of rolling a number greater than 3, given you've rolled an even number, is 2/3.**

- Similarity to Hypothesis testing

# Bayes theorem
- Prior
- Likelihood
- Posterior
	
# Difference between conditional probability and Bayes theorem

# Expected value
## Expected Value: Understanding Averages in Probability

Expected value (or expectation) is a fundamental concept in probability theory. It represents the average value of a random variable over many trials. It's essentially a weighted average, where the weights are the probabilities of each outcome.

**Formal Definition:**

For a discrete random variable X with possible values x₁, x₂, ..., xₙ and corresponding probabilities P(x₁), P(x₂), ..., P(xₙ), the expected value E(X) is calculated as:

E(X) = x₁ * P(x₁) + x₂ * P(x₂) + ... + xₙ * P(xₙ)

**Example 1: Fair Coin Toss**

Let's consider a fair coin toss.

* If heads (H) appears, you win $1.
* If tails (T) appears, you win $0.

What is the expected value of your winnings?

* Possible outcomes: $1 (heads) and $0 (tails)
* Probabilities: P(H) = 0.5, P(T) = 0.5

E(X) = ($1 * 0.5) + ($0 * 0.5) = $0.5 + $0 = $0.5

Therefore, the expected value of your winnings is $0.50.

**Example 2: Rolling a Die**

Let's consider rolling a fair six-sided die.

What is the expected value of the number rolled?

* Possible outcomes: 1, 2, 3, 4, 5, 6
* Probabilities: P(1) = P(2) = P(3) = P(4) = P(5) = P(6) = 1/6

E(X) = (1 * 1/6) + (2 * 1/6) + (3 * 1/6) + (4 * 1/6) + (5 * 1/6) + (6 * 1/6)

E(X) = (1 + 2 + 3 + 4 + 5 + 6) / 6 = 21 / 6 = 3.5

Therefore, the expected value of the number rolled is 3.5.

**Example 3: Lottery Ticket**

Imagine a lottery where:

* You have a 1/1000 chance of winning $500.
* You have a 999/1000 chance of winning $0.

What is the expected value of a lottery ticket?

E(X) = ($500 * 1/1000) + ($0 * 999/1000) = $0.50 + $0 = $0.50

Therefore, the expected value of the lottery ticket is $0.50. If the ticket costs more than $0.50, on average you will lose money.

**Key Points:**

* Expected value is a long-term average.
* It's used to make decisions in situations with uncertainty.
* It's crucial in fields like finance, gambling, and insurance.

# Essense of Information theory
- Quantifying uncertainity
- Entropy
- Entropy curve calculation
- Cross entropy

# Problem 1: Medical Test Accuracy
A certain disease affects 1% of population. A test of the disease is 99% accurate meaning
- If a person has the disease the test will be positive 99%
- If the person does not have disease, the test will be negative 99%

$P(D)$ : Probability of person has disease
$P(T)$ : Probablity of test is positive

$P(D)$ = 0.01

$P(D')$ = 1-$P(D)$ = 1-0.01 = 0.99

$P(T|D)$ = 0.99

$P(T'|D')$ = 0.99

$P(T|D')$ = 1-$P(T|D)$ = 1-0.99 = 0.01

Find $P(D|T)$  and $P(D|T')$


# Problem 2: Spam Email Classification

Suppose and email is classified as spam if it contains the word "money". Past statistics show:
- 5% of all emails are spam
- 2% non-spam emails contains the word money
- 60% spam emails contains the word money

Find $P(Spam|money)$ and $P(Spam|money')$


# Problem 3 : Sample Space
- List the sample space for tossing two coins 
- What is the sample space for rolling two dice?
- How many possible outcomes exist in selecting a card from a standard deck of 52 playing cards?
- If an experiment consists of flipping a coin and rolling a die, what is the total number of outcomes?

# Problem 4 :Dependent and Independent Events
- A bag contains 4 red balls and 6 blue balls. If you pick one ball and then another with replacement, are the events independent or dependent?


# Problem 5: Joint and Marginal Probability
- A dataset shows that 40% of customers purchase Product A, 25% purchase Product B, and 15% purchase both. What is the probability that a customer purchases at least one product? 


# Problem 6:  Expected Value
- A lottery ticket costs ₹10 and has a 1% chance of winning ₹500. What is the expected value of the ticket?**  
  

# Problem 7:  Entropy & Information Theory
- What is the entropy of a fair coin toss?**  
 $H(X) = - (0.5 \log_2 0.5 + 0.5 \log_2 0.5)$ = 1

- A probability distribution is $P(X) = (0.8,0.2)$. Calculate its entropy 




