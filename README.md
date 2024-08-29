# Martingale


The Martingale model is a concept in probability theory that describes a fair game. In a martingale, the conditional expectation of the next value in a sequence, given all prior values, is equal to the current value. This means that, on average, the future expected value of the sequence is the same as the present value, reflecting the notion of "fairness" or "no advantage."


A sequence of random variables {X_t} is called a martingale with respect to a filtration {F_t} (which represents the information available up to time t) if for all t:
E[X_{t+1} | F_t] = X_t
Here:
X_t is the value of the process at time t.
E denotes the expectation (average value) given the information available up to time t (F_t).

Fair Game:
The martingale property implies that the process has no "drift," meaning that the expected future value is simply the current value. There is no systematic tendency for the process to increase or decrease, reflecting a fair game where there is no predictable advantage.

Martingale in Betting Strategies:
In gambling and finance, a martingale strategy involves doubling the bet after each loss, with the idea that a win would recover all previous losses plus a profit equal to the original bet. The simplest form is the Martingale betting strategy.

Betting Strategy:
Start with an initial stake.
If you win, collect your profit and start again with the initial bet.
If you lose, double your bet and try again.
The expectation is that eventually, you'll win and recover all losses.

Problems with Martingale:
While theoretically sound under the assumption of infinite wealth and no betting limits, the martingale strategy faces practical issues:
Capital Limits: Players may run out of money before they win.
Betting Limits: Casinos and financial markets often impose limits on the size of bets, making it impossible to continue doubling.
Risk of Ruin: The strategy can lead to large losses if a long losing streak occurs.


Consider a simple game where you bet on a coin toss:
Let X_t be the amount of money you have after t coin tosses.
You start with X_0 = 100 dollars.

On each toss, you bet 1 dollar. If the coin comes up heads, you win 1 dollar; if tails, you lose 1 dollar.
The sequence {X_t} is a martingale because:
E[X_{t+1} | X_t] = X_t
This is because the expected value after the next toss is just your current amount of money, as the game is fair.

If the outcome of the t-th coin toss is denoted by Y_t, where Y_t = 1 for heads and Y_t = -1 for tails, the wealth after t tosses is:
X_t = X_0 + sum_{i=1}^{t} Y_i

The martingale property asserts that:
E[X_{t+1} | X_1, X_2, ..., X_t] = X_t
This means that knowing all previous outcomes does not change the expected future value of the process.
