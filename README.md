[llm_report_template (2).md](https://github.com/user-attachments/files/27054717/llm_report_template.2.md)
# Solid-State-LLM-HW2# LLM Report — Problem Set 2
**Your name: Chang-Chi Kao
**Date submitted:2026/04/24
**Problem set number:**

---

## Instructions

For each LLM interaction, copy the **Interaction Block** below and fill it in completely. You may have as many blocks as interactions. At minimum you must include:

- One **Tier 2** prompt (two different models)
- One **Tier 4** prompt (two different models)

So you will have at least four blocks. For PS5, also include at least one synthesis prompt block and one block for your own original prompt.

Delete these instructions before submitting.

---

## Interaction 1

**Problem this relates to:** PS_1_ , Problem _1_

**Tier:** (circle one) &nbsp; Tier 1 &nbsp;|&nbsp; Tier 2 &nbsp;|&nbsp; Tier 3 &nbsp;|&nbsp; Tier 4 &nbsp;|&nbsp; Synthesis &nbsp;|&nbsp; Original

**Model name and version:** Chatgpt thinking 5.4 and Gemini Pro

### Prompt

```
Please solve the problem in the image.
```

### Model Response

```
# Chatgpt Thinking : 
This is the standard solution expected if the problem explicitly asks for a **two-fold degeneracy**.

## 1. Free-electron energy

The free-electron energy is

$$
E^{(0)}_{\mathbf{k}}=\frac{\hbar^2|\mathbf{k}|^2}{2m}.
$$

Two free-electron states are degenerate when

$$
E^{(0)}_{\mathbf{k}}=E^{(0)}_{\mathbf{k}-\mathbf{G}}.
$$

Because the energy only depends on the magnitude of the wave vector, this means

$$
|\mathbf{k}|^2=|\mathbf{k}-\mathbf{G}|^2.
$$
Expanding,

$$
|\mathbf{k}-\mathbf{G}|^2
=
|\mathbf{k}|^2-2\mathbf{k}\cdot\mathbf{G}+|\mathbf{G}|^2.
$$

Therefore,

$$
|\mathbf{k}|^2
=
|\mathbf{k}|^2-2\mathbf{k}\cdot\mathbf{G}+|\mathbf{G}|^2.
$$

Canceling \( |\mathbf{k}|^2 \),

$$
\mathbf{k}\cdot\mathbf{G}=\frac{|\mathbf{G}|^2}{2}.
$$
## 2. Choose one Bragg plane

For FCC real space, the reciprocal lattice is BCC. Choose

$$
\mathbf{G}=\frac{2\pi}{a}(1,1,1).
$$

At

$$
\mathbf{K}=\frac{2\pi}{a}\left(\frac34,\frac34,0\right),
$$

we have

$$
\mathbf{K}\cdot\mathbf{G}
=
\left(\frac{2\pi}{a}\right)^2
\left(
\frac34+\frac34+0
\right)
=
\left(\frac{2\pi}{a}\right)^2\frac32.
$$
Also,

$$
|\mathbf{G}|^2
=
\left(\frac{2\pi}{a}\right)^2(1^2+1^2+1^2)
=
3\left(\frac{2\pi}{a}\right)^2.
$$

So

$$
\frac{|\mathbf{G}|^2}{2}
=
\frac32\left(\frac{2\pi}{a}\right)^2.
$$
Thus,

$$
\mathbf{K}\cdot\mathbf{G}
=
\frac{|\mathbf{G}|^2}{2}.
$$

Therefore,

$$
E^{(0)}_{\mathbf{K}}
=
E^{(0)}_{\mathbf{K}-\mathbf{G}}.
$$

So the two plane waves

$$
|\mathbf{k}\rangle
$$

and

$$
|\mathbf{k}-\mathbf{G}\rangle
$$

are degenerate at \(K\).

---
## 3. Set up the two-state perturbation matrix

The periodic lattice potential is written as

$$
V(\mathbf{r})
=
\sum_{\mathbf{G}}U_{\mathbf{G}}e^{i\mathbf{G}\cdot\mathbf{r}}.
$$

In the basis

$$
\left\{
|\mathbf{k}\rangle,
|\mathbf{k}-\mathbf{G}\rangle
\right\},
$$

the Hamiltonian is

$$
H=
\begin{pmatrix}
E^{(0)}_{\mathbf{k}} & U_{\mathbf{G}}\\
U_{\mathbf{G}}^* & E^{(0)}_{\mathbf{k}-\mathbf{G}}
\end{pmatrix}.
$$

where

$$
E^{(0)}_{\mathbf{k}}
=
\frac{\hbar^2|\mathbf{k}|^2}{2m},
$$

and

$$
E^{(0)}_{\mathbf{k}-\mathbf{G}}
=
\frac{\hbar^2|\mathbf{k}-\mathbf{G}|^2}{2m}.
$$

---
## 4. Solve the eigenvalue equation

We solve

$$
\det(H-EI)=0.
$$

That is,

$$
\det
\begin{pmatrix}
E^{(0)}_{\mathbf{k}}-E & U_{\mathbf{G}}\\
U_{\mathbf{G}}^* & E^{(0)}_{\mathbf{k}-\mathbf{G}}-E
\end{pmatrix}
=0.
$$

So

$$
\left(E^{(0)}_{\mathbf{k}}-E\right)
\left(E^{(0)}_{\mathbf{k}-\mathbf{G}}-E\right)
-
|U_{\mathbf{G}}|^2
=
0.
$$

The two eigenvalues are

$$
E_{\pm}
=
\frac{
E^{(0)}_{\mathbf{k}}
+
E^{(0)}_{\mathbf{k}-\mathbf{G}}
}{2}
\pm
\sqrt{
\left(
\frac{
E^{(0)}_{\mathbf{k}}
-
E^{(0)}_{\mathbf{k}-\mathbf{G}}
}{2}
\right)^2
+
|U_{\mathbf{G}}|^2
}.
$$

Therefore the energy splitting is

$$
\Delta E
=
E_+-E_-.
$$

So

$$
\Delta E
=
2
\sqrt{
\left(
\frac{
E^{(0)}_{\mathbf{k}}
-
E^{(0)}_{\mathbf{k}-\mathbf{G}}
}{2}
\right)^2
+
|U_{\mathbf{G}}|^2
}.
$$

At the exact \(K\) point,
$$
E^{(0)}_{\mathbf{K}}
=
E^{(0)}_{\mathbf{K}-\mathbf{G}},
$$

so

$$
\boxed{
\Delta E(K)=2|U_{\mathbf{G}}|
}
$$

---
```
### Mode2 Response

### Your Verdict

**Overall assessment:** (circle one) &nbsp; Correct &nbsp;|&nbsp; Partially correct &nbsp;|&nbsp; Wrong &nbsp;|&nbsp; Hallucinated

**Specific errors identified:**
<!-- Cite your own derivation, the textbook, or lecture notes. Be precise: "The model's secular matrix omits the off-diagonal term V_G" rather than "the model was wrong." -->

-

**What the model did better than expected:**

-

**What the model failed to do:**

-

### Revised Prompt (if you iterated)

```
Paste your follow-up prompt here, or delete this section if you did not iterate.
```

### Follow-up Response

```
Paste follow-up response verbatim, or delete if not applicable.
```

### Reflection

<!-- Which prompting strategy worked best for this type of problem? What would you do differently next time? (2–4 sentences) -->



---

## Interaction 2

**Problem this relates to:** PS___ , Problem ___

**Tier:** (circle one) &nbsp; Tier 1 &nbsp;|&nbsp; Tier 2 &nbsp;|&nbsp; Tier 3 &nbsp;|&nbsp; Tier 4 &nbsp;|&nbsp; Synthesis &nbsp;|&nbsp; Original

**Model name and version:**

### Prompt

```
Paste your exact prompt here.
```

### Model Response

```
Paste the model's response verbatim.
```

### Your Verdict

**Overall assessment:** (circle one) &nbsp; Correct &nbsp;|&nbsp; Partially correct &nbsp;|&nbsp; Wrong &nbsp;|&nbsp; Hallucinated

**Specific errors identified:**

-

**What the model did better than expected:**

-

**What the model failed to do:**

-

### Revised Prompt (if you iterated)

```

```

### Follow-up Response

```

```

### Reflection



---

## Interaction 3

**Problem this relates to:** PS___ , Problem ___

**Tier:** (circle one) &nbsp; Tier 1 &nbsp;|&nbsp; Tier 2 &nbsp;|&nbsp; Tier 3 &nbsp;|&nbsp; Tier 4 &nbsp;|&nbsp; Synthesis &nbsp;|&nbsp; Original

**Model name and version:**

### Prompt

```

```

### Model Response

```

```

### Your Verdict

**Overall assessment:** (circle one) &nbsp; Correct &nbsp;|&nbsp; Partially correct &nbsp;|&nbsp; Wrong &nbsp;|&nbsp; Hallucinated

**Specific errors identified:**

-

**What the model did better than expected:**

-

**What the model failed to do:**

-

### Revised Prompt (if you iterated)

```

```

### Follow-up Response

```

```

### Reflection



---

## Interaction 4

**Problem this relates to:** PS___ , Problem ___

**Tier:** (circle one) &nbsp; Tier 1 &nbsp;|&nbsp; Tier 2 &nbsp;|&nbsp; Tier 3 &nbsp;|&nbsp; Tier 4 &nbsp;|&nbsp; Synthesis &nbsp;|&nbsp; Original

**Model name and version:**

### Prompt

```

```

### Model Response

```

```

### Your Verdict

**Overall assessment:** (circle one) &nbsp; Correct &nbsp;|&nbsp; Partially correct &nbsp;|&nbsp; Wrong &nbsp;|&nbsp; Hallucinated

**Specific errors identified:**

-

**What the model did better than expected:**

-

**What the model failed to do:**

-

### Revised Prompt (if you iterated)

```

```

### Follow-up Response

```

```

### Reflection



---

<!-- Add more Interaction blocks as needed by copying the block above -->

---

## Summary

**Total interactions this problem set:** ___

**Models used:**
- Model 1:
- Model 2:
- Other (if any):

**Overall observation:** In 3–5 sentences, describe the most important pattern you noticed across all your interactions this week. For example: did one model consistently outperform the other? Did the models do better on derivations or on conceptual questions? Was there a type of error that appeared repeatedly?

