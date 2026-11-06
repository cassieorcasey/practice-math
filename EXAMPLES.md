# Example sessions

Three sessions showing how the skill behaves. Each AI turn gives one hint or one step and ends with one task. Section numbers (§) refer to the rules in [`practice-math/SKILL.md`](practice-math/SKILL.md).

## 1. A calculation, with a mistake

Covers the four Pólya stages, the hint ladder (§5), looking back (§12), and the closing summary (§13).

> **User:** Solve $3x - 7 = 11$.
>
> **AI:** Here's the problem: $3x - 7 = 11$. Before we start, what is the problem asking you to find?
>
> **User:** The value of $x$.
>
> **AI:** Right. To get $x$ alone, which part of the left side should go first?
>
> **User:** The $-7$. So $3x = 11 - 7 = 4$.
>
> **AI:** Close. Something is off in the step where you moved the $7$. Check it again.
>
> **User:** Hmm, I still get $4$.
>
> **AI:** Look at the sign. When $-7$ moves to the right side, what does its sign become?
>
> **User:** Oh, it becomes $+7$. So $3x = 18$.
>
> **AI:** That's it. What's the next step?
>
> **User:** Divide both sides by $3$, so $x = 6$.
>
> **AI:** Before we call it done, substitute $x = 6$ back into $3x - 7$. What do you get?
>
> **User:** $18 - 7 = 11$. It matches.
>
> **AI:** Nicely checked. The core move here was undoing operations in reverse order. The common trap is the sign flip when a term crosses the equals sign, which is exactly where you slipped. You fixed it with only two hints, so want to try a slightly harder one, like $\frac{2x + 1}{3} = 5$?

The AI never wrote $3x = 18$ itself. It gave the location of the mistake first, then its type, and the user fixed it.

## 2. A proof by induction

Covers guiding the skeleton before the details (§8).

> **User:** Prove that $1 + 3 + 5 + \dots + (2n - 1) = n^2$.
>
> **AI:** The claim is $1 + 3 + 5 + \dots + (2n - 1) = n^2$ for every natural number $n$. Which proof method suits a statement about every natural number?
>
> **User:** Induction?
>
> **AI:** Yes. Before any algebra, write the two parts an induction proof needs, just the headings.
>
> **User:** Base case and inductive step.
>
> **AI:** Good skeleton. Start with the base case. Which $n$ do you check, and does it hold?
>
> **User:** $n = 1$. Left side is $1$, right side is $1^2 = 1$. It holds.
>
> **AI:** Correct. For the inductive step, what do you assume, and what do you need to show?
>
> **User:** Assume $1 + 3 + \dots + (2k - 1) = k^2$. Show $1 + 3 + \dots + (2k + 1) = (k + 1)^2$.
>
> **AI:** Exactly right. The new sum is the old sum plus one more term. Using your assumption, write the new sum in terms of $k$.
>
> **User:** $k^2 + (2k + 1)$.
>
> **AI:** Can you rewrite that as a square?
>
> **User:** $k^2 + 2k + 1 = (k + 1)^2$. Done.
>
> **AI:** That completes the proof. Read your base case and inductive step together once: does every line follow from the one before? The core idea was splitting the $(k + 1)$ sum into "old sum plus one term" so the assumption can be used. The common trap is writing the last term as $2k - 1$ instead of $2(k + 1) - 1 = 2k + 1$.

## 3. Revealing the solution

Covers the escape hatch (§3): the user tried once, then asked for the solution.

> **User:** How many ways can I choose 2 people from a group of 5?
>
> **AI:** We're choosing 2 people out of 5. Does the order you pick them in matter here?
>
> **User:** I don't think so. I'll say $5 \times 4 = 20$.
>
> **AI:** Good start. $5 \times 4$ counts something real, but check it against your answer about order. If you pick Ana then Budi, and Budi then Ana, how many times does $5 \times 4$ count that pair?
>
> **User:** I give up.
>
> **AI:** No problem, you've made an attempt, so here is the full solution.
>
> 1. Pick the first person: 5 choices. Pick the second: 4 choices. That gives $5 \times 4 = 20$ **ordered** picks.
> 2. Every pair appears twice in those 20 (Ana then Budi, and Budi then Ana), because order doesn't matter for a group. **This is the step where you got stuck.**
> 3. Divide by 2 to remove the double count: $\frac{20}{2} = 10$.
>
> In general this is $\binom{5}{2} = \frac{5!}{2! \, 3!} = 10$.
>
> Now try a similar one with the same idea: how many ways can you choose 2 people from a group of 6? What's your first step?

The AI revealed the solution only because the user had made an attempt. The follow-up problem comes without its answer, so the normal flow starts again.
