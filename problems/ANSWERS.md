# Answers

Final answers to [PROBLEMS.md](PROBLEMS.md), each with the key idea in one line. Use these to check your work after you finish, not to start.

## Algebra

**ALG-E1.** $x = 4$. Collect the $x$ terms on one side: $3x = 12$.

**ALG-E2.** $(x + 3)(x + 4)$. Find two numbers with product 12 and sum 7.

**ALG-M1.** $x = 3$, $y = 1$. Add the equations to eliminate $y$: $3x = 9$.

**ALG-M2.** $x = 5$ or $x = -2$. Split into $2x - 3 = 7$ and $2x - 3 = -7$.

**ALG-H1.** $x = 4$. Factor out $2^x$: $3 \cdot 2^x = 48$, so $2^x = 16$.

**ALG-H2.** $x = 4$. Combine the logs: $x(x - 2) = 8$ gives $x = 4$ or $x = -2$, and $x = -2$ is rejected because $\log_2 x$ needs $x > 0$.

## Discrete math

**DIS-E1.** 16. Each of the 4 elements is either in or out: $2^4$.

**DIS-E2.** Yes, they are equivalent. $\neg q \to \neg p$ is the contrapositive of $p \to q$, and both are false only when $p$ is true and $q$ is false.

**DIS-M1.** 5040. $10 \cdot 9 \cdot 8 \cdot 7$.

**DIS-M2.** 9. By the handshake lemma, the sum of degrees is twice the number of edges: $6 \cdot 3 = 18 = 2E$.

**DIS-H1.** Base case $n = 1$: $1 - 1 = 0$, divisible by 3. Inductive step: $(k + 1)^3 - (k + 1) = (k^3 - k) + 3k^2 + 3k$. The first part is divisible by 3 by the hypothesis, and $3k^2 + 3k = 3(k^2 + k)$.

**DIS-H2.** 60. Six letters with A repeated 3 times and N repeated 2 times: $\frac{6!}{3! \, 2!}$.

## Calculus

**CAL-E1.** $f'(x) = 12x^3 - 2$. Power rule on each term.

**CAL-E2.** 4. Factor the numerator: $\frac{(x - 2)(x + 2)}{x - 2} = x + 2$ for $x \neq 2$.

**CAL-M1.** $f'(x) = 2x \sin x + x^2 \cos x$. Product rule.

**CAL-M2.** 10. The antiderivative is $x^3 + x$, and $(8 + 2) - 0 = 10$.

**CAL-H1.** $x \sin x + \cos x + C$. Integration by parts with $u = x$ and $dv = \cos x \, dx$.

**CAL-H2.** A $5 \times 5$ square, with area 25. With width $w$, the area is $w(10 - w)$, which is largest at $w = 5$.

## Probability and statistics

**PRB-E1.** $\frac{1}{6}$. Six of the 36 outcomes sum to 7.

**PRB-E2.** 7. The sum is 35, divided by 5.

**PRB-M1.** $\frac{3}{28}$. $\frac{3}{8} \cdot \frac{2}{7}$.

**PRB-M2.** 4. The mean is 5, the squared deviations sum to 32, and $32 / 8 = 4$.

**PRB-H1.** $\frac{5}{16}$. $\binom{5}{3} / 2^5 = 10 / 32$.

**PRB-H2.** $\frac{2}{13} \approx 0.154$. Bayes' theorem: $\frac{0.01 \cdot 0.9}{0.01 \cdot 0.9 + 0.99 \cdot 0.05} = \frac{0.009}{0.0585}$.

## Linear algebra

**LIN-E1.** $\begin{pmatrix} 1 & 3 \\ 4 & 4 \end{pmatrix}$. Add entry by entry.

**LIN-E2.** 5. $2 \cdot 4 - 3 \cdot 1$.

**LIN-M1.** $\begin{pmatrix} 2 & 1 \\ 4 & 3 \end{pmatrix}$. Row of $A$ times column of $B$. Multiplying by $B$ swaps the columns of $A$.

**LIN-M2.** $\begin{pmatrix} 3 & -1 \\ -5 & 2 \end{pmatrix}$. The determinant is 1, so swap the diagonal and negate the off-diagonal.

**LIN-H1.** $\lambda = 5$ and $\lambda = 2$. The characteristic equation is $(4 - \lambda)(3 - \lambda) - 2 = \lambda^2 - 7\lambda + 10 = 0$.

**LIN-H2.** $x = 1$, $y = 2$, $z = 3$. Add the first and third equations to eliminate $z$: $2x + 3y = 8$. Subtract the first from the second: $x - 2y = -3$.

## Geometry and trigonometry

**GEO-E1.** 10. $\sqrt{6^2 + 8^2} = \sqrt{100}$.

**GEO-E2.** 1. Both terms equal $\frac{1}{2}$.

**GEO-M1.** $49\pi$. $\pi r^2$.

**GEO-M2.** $x = \frac{\pi}{6}$ or $x = \frac{5\pi}{6}$. $\sin x = \frac{1}{2}$ in the first and second quadrants.

**GEO-H1.** 5. $\sqrt{(4 - 1)^2 + (6 - 2)^2} = \sqrt{25}$.

**GEO-H2.** $60^\circ$. Law of cosines: $\cos \theta = \frac{5^2 + 8^2 - 7^2}{2 \cdot 5 \cdot 8} = \frac{40}{80} = \frac{1}{2}$.
