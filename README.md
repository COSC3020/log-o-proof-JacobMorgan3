[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/fbkbKZ5N)
# Asymptotic Equivalences

In the lectures, we said that logarithms with different bases don't affect the
asymptotic complexity of an algorithm. Prove that $O(\log_{2} n)$ is the same as
$O(\log_{5} n)$. Use the mathematical definition of $O$ -- do a formal proof,
not just the intuition.

I have started with the formal definition of $O$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$T(n) \in O(f(n)) \iff \exists c, n_0: T(n) \leq c \cdot f(n) \forall n \geq n_0$ <br />

We want to show that $O(log_5(n)) = O(log_2(n))$ <br/>
### Case 1: $log_5(n) \in O(log_2(n))$ <br/>
$log_5(n) = log_2(n) / log_2(5)$ <br/>
$T(n) \leq cf(x)$
$log_5(n) \leq c * (log_2(n) / log_2(5))$ <br/>
$log_5(n) \leq c * log_2(n)$ <br/>
$log_5(n) \in O(log_2(n))$ <br/>

### Case 2: $log_2(n) \in O(log_5(n))$ <br/>
$log_2(n) = log_5(n) / log_5(2)$ <br/>
$T(n) \leq cf(x)$
$log_2(n) \leq c * (log_5(n) / log_5(2))$ <br/>
$log_2(n) \leq c * log_5(n)$ <br/>
$log_2(n) \in O(log_5(n))$ <br/>
