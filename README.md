# Asymptotic Equivalences

In the lectures, we said that logarithms with different bases don't affect the
asymptotic complexity of an algorithm. Prove that $O(\log_{2} n)$ is the same as
$O(\log_{5} n)$. Use the mathematical definition of $O$ -- do a formal proof,
not just the intuition.

I have started with the formal definition of $O$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$T(n) \in O(f(n)) \iff \exists c, n_0: T(n) \leq c \cdot f(n) \forall n \geq n_0$



Claim:
\begin{center}
    $O(\log_{2} n) \iff O(\log_{5} n)$
\end{center}

Proof:

Let $f(n) \in O(\log_{2} n)$. We have, $f(n) \in O(\log_{2} n) \iff \exists c, n_0: f(n) \leq c \cdot \log_{2} n \; \forall n \geq n_0$

Consider:

$\log_{2} n$. 

$\log_{2} n = \log_5(n) \cdot \frac{1}{\log_5(2)}$

Thus, if $\exists c, n_0: f(n) \leq c \cdot \log_{2} n  = c \cdot \log_5(n) \cdot \frac{1}{\log_5(2)} = c_2 \cdot \log_5(n) \; \forall n \geq n_0$
where $c_2$ is a constant.

Thus,
$O(\log_{2} n)$ is the same as
$O(\log_{5} n)$



I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

I used the website to review the properties of logarithms:

https://www.andrews.edu/~calkins/math/webtexts/numb17.htm
