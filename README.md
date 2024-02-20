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

Let us say that: <br/>
$T(n) = log_{5}(n)$ and $f(n) = log_{3}(n)$ and $c = 1$ and $n_0 = 1$ and $n = 2$ <br />

$log_{5}(2) <= 1 * log_{3}(2)$ <br/>
$.431 <= .631$ <br/>

$log_{5}(n) \in O(log_{3}(n)$ <br/>

Now Let us look at T(n) = $log_{3}(n)$: <br/>
$T(n) = log_{3}(n)$ and $f(n) = log_{5}(n)$ and $c = 2$ and $n_0 = 1$ and $n = 2$ <br />

$log_{3}(2) <= 2 * log_{5}(2)$ <br/>
$.631 <= .862$ <br/>

$log_{3}(n) \in O(log_{5}(n)$ <br/>

Since both belong to the big O of each other it is irrelevant which base we use. 



