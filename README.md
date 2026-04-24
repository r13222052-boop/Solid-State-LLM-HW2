[llm_report_template (2).md](https://github.com/user-attachments/files/27054717/llm_report_template.2.md)
# Solid-State-LLM-HW2# LLM Report — Problem Set 2
**Your name: Chang-Chi Kao
**Date submitted:2026/04/24
**Problem set number:**

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
Because two Bragg planes intersect at K, we should include three states:

∣k⟩,∣k−G
1
	​

⟩,∣k−G
2
	​

⟩

with

G
1
	​

=
a
2π
	​

(1,1,1),G
2
	​

=
a
2π
	​

(1,1,−1)

The perturbation matrix is

H=
	​

E
k
(0)
	​

U
G
1
	​

∗
	​

U
G
2
	​

∗
	​

	​

U
G
1
	​

	​

E
k−G
1
	​

(0)
	​

U
G
1
	​

−G
2
	​

	​

	​

U
G
2
	​

	​

U
G
2
	​

−G
1
	​

	​

E
k−G
2
	​

(0)
	​

	​

	​


At exactly K,

E
K
(0)
	​

=E
K−G
1
	​

(0)
	​

=E
K−G
2
	​

(0)
	​


so without the lattice potential, these free-electron states are degenerate.

If we assume

U
G
1
	​

	​

=U
G
2
	​

	​

=U

and temporarily neglect the coupling

U
G
2
	​

−G
1
	​

	​

=U
(0,0,−2)
	​


then the matrix becomes

H=E
K
(0)
	​

I+
	​

0
U
∗
U
∗
	​

U
0
0
	​

U
0
0
	​

	​


The eigenvalues are

E
1
	​

=E
K
(0)
	​

+
2
	​

∣U∣
E
2
	​

=E
K
(0)
	​

−
2
	​

∣U∣
E
3
	​

=E
K
(0)
	​


So the full splitting at the intersection of two Bragg planes is larger than the simple two-state result:

ΔE
top-bottom
	​

=2
2
	​

∣U∣

instead of

2∣U∣
Physical meaning

At a Bragg plane, the electron wave ∣k⟩ and the scattered wave ∣k−G⟩ have the same kinetic energy. Therefore, the weak periodic crystal potential mixes them strongly.

That mixing forms standing-wave-like combinations. One combination has more charge density near ion cores, while the other has more charge density between ion cores. Because these feel different potential energies, the original free-electron degeneracy is lifted.

So near the FCC K point:

degeneracy occurs because two Bragg reflection conditions are satisfied simultaneously
	​


and the nearly-free-electron perturbation matrix should ideally include all degenerate plane-wave states connected by those reciprocal lattice vectors.
### Your Verdict
I think the way they calculating the physics is sufficient and efficient. But I think they should put more wrok on the preturbatioln
theory in quantum mechanis. The detailed process should be considered when construct the matrix.

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

I think the biggest problem in the HW is the answer cannot be transferred into the markdown file well. Even I asked the LLM transfer all the formulas or matrix to a code, I still cannot see a proper format of them in the preview. Btw, I use Github to write codes and see the result of previews or outputs.  



---

## Interaction 2

**Problem this relates to:** PS_2_ , Problem _2_

**Tier:** (circle one) &nbsp; Tier 1 &nbsp;|&nbsp; Tier 2 &nbsp;|&nbsp; Tier 3 &nbsp;|&nbsp; Tier 4 &nbsp;|&nbsp; Synthesis &nbsp;|&nbsp; Original

**Model name and version:**Chatgpt thinking 5.4 and Gemini Pro

### Prompt

```
Please solve the problem in the image.
```

### Model Response

```
Chatgpt Thinking 5.4:

The density of states is

D(E)=
(2π)
3
1
	​

∫d
3
k δ(E−E(k))

Define

ϵ=E−E
c
	​


and rescale variables:

u=
2m
x
	​

	​

ℏk
x
	​

	​

,v=
2m
y
	​

	​

ℏk
y
	​

	​

,w=
2m
z
	​

	​

ℏk
z
	​

	​


Then

ϵ=u
2
+v
2
−w
2

So

D(E)∝∫dudvdw δ(ϵ−u
2
−v
2
+w
2
)

Use cylindrical coordinates in u,v:

u
2
+v
2
=r
2

Then

D(E)∝∫dw∫rdr δ(ϵ−r
2
+w
2
)

The delta function gives

r
2
=w
2
+ϵ

So the singular part comes from the change in allowed w-range near ϵ=0.

The result in 3D is not a true divergence:

D(E)=D(E
c
	​

)+A(E−E
c
	​

)ln∣E−E
c
	​

∣+⋯
	​


Therefore,

dE
dD
	​

∼ln∣E−E
c
	​

∣
	​


So D(E) is finite, but its slope is singular.Paste the model's response verbatim.

Gemini Pro:
Near a critical point, any band can be expanded as

E(k)=E
c
	​

+λ
x
	​

q
x
2
	​

+λ
y
	​

q
y
2
	​

+λ
z
	​

q
z
2
	​


Here the signs are

(+,+,−)

because the x and y terms are positive, while the z term is negative.

The number of negative curvatures is the Morse index.

Here:

Morse index=1

Therefore this is an

M
1
	​

 Van Hove singularity
	​


In 3D:

Type	Curvature	DOS behavior
M
0
	​

	+,+,+	
E−E
c
	​

	​

 onset
M
1
	​

	+,+,−	finite cusp / slope singularity
M
2
	​

	+,−,−	finite cusp / slope singularity
M
3
	​

	−,−,−	
E
c
	​

−E
	​

 ending

So this dispersion corresponds to

M
1
	​

	​


and the DOS has a finite cusp, not a strong divergence.

Final Answer
E(k)=E
c
	​

+q
x
2
	​

+q
y
2
	​

−q
z
2
	​

	​


has two positive curvatures and one negative curvature.

Therefore:

It is an M
1
	​

 3D Van Hove singularity
	​


and

D(E) remains finite near E
c
	​

, but dD/dE is singular.
	​


More specifically,

D(E)=D(E
c
	​

)+A(E−E
c
	​

)ln∣E−E
c
	​

∣+⋯
	​

```

### Your Verdict
I think the models can put more affort on the expansion in mathematical way. Everything seems okay except of this point. 

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

**Problem this relates to:** PS_2_ , Problem _3_

**Tier:** (circle one) &nbsp; Tier 1 &nbsp;|&nbsp; Tier 2 &nbsp;|&nbsp; Tier 3 &nbsp;|&nbsp; Tier 4 &nbsp;|&nbsp; Synthesis &nbsp;|&nbsp; Original

**Model name and version:**

### Prompt

```
Solve the problems in the images.
```

### Model Response

```
Chatgpt Thinking 5.4:
For each fixed n, the electron is a 2D free electron.

The 2D DOS per area is constant:

D
2D
	​

(E)=
πℏ
2
m
	​


including spin degeneracy.

But subband n only contributes when

E>E
n
	​


So the total DOS is

D(E)=
πℏ
2
m
	​

n=1
∑
∞
	​

Θ(E−E
n
	​

)
	​


This is a staircase function.

At each E=E
n
	​

, a new subband becomes available, so D(E) jumps upward by

ΔD=
πℏ
2
m
	​

	​
Gemini Pro:
ecause motion in z is quantized, the electron can only occupy discrete standing waves:

k
z
	​

=
d
nπ
	​


For each allowed k
z
	​

, the electron still has continuous k
x
	​

,k
y
	​

.

So each subband behaves like an independent 2D electron gas.

Therefore:

D(E)=D
2D
	​

×number of occupied subbands
	​


So:

D(E)=
πℏ
2
m
	​

N(E)
	​


where N(E) is the number of subband bottoms below E.

That is why the DOS forms a staircase.

Tier 3: Estimate well width for true 2D behavior

Given:

V
0
	​

=100 meV
T=20 mK

Thermal energy:

k
B
	​

T≈0.0017 meV

For true 2D behavior, need:

E
1
	​

<V
0
	​


so the first subband is bound, and

E
2
	​

−E
1
	​

≫k
B
	​

T

so thermal energy cannot populate higher subbands.

For an infinite well:

E
1
	​

=
2md
2
π
2
ℏ
2
	​


Bound-state condition:

E
1
	​

<V
0
	​


gives approximately

d>1.9 nm
	​


Thermal condition:

E
2
	​

−E
1
	​

=3E
1
	​

≫k
B
	​

T

gives approximately

d≪0.81 μm
	​


So a rough allowed range is

2 nm≲d≪0.8 μm
	​


For a real finite well, the lower bound should be larger than this estimate, so practically:

d∼5–100 nm
	​


is a reasonable true-2D quantum-well range.

Final answer:

D(E)=
πℏ
2
m
	​

n
∑
	​

Θ(E−E
n
	​

)
	​

```

### Your Verdict
I think the LLMs should derive the 2D DOS in the very bigging, then start to apply the conditions in the problems. It's a common situation that the LLM tends to choose a well-known model without a direct instruction or demands in the prompt.

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

**Problem this relates to:** PS_2_ , Problem _4_

**Tier:** (circle one) &nbsp; Tier 1 &nbsp;|&nbsp; Tier 2 &nbsp;|&nbsp; Tier 3 &nbsp;|&nbsp; Tier 4 &nbsp;|&nbsp; Synthesis &nbsp;|&nbsp; Original

**Model name and version:**

### Prompt

```
Solve the problems in the images.
```

### Model Response

```
Chatgpy Thinking 5.4:
Tight-binding form:

E(k)=ϵ
s
	​

+t
δ
∑
	​

e
ik⋅δ

Summing over the 12 FCC nearest neighbors gives

E(k)=ϵ
s
	​

+4t[cos
2
k
x
	​

a
	​

cos
2
k
y
	​

a
	​

+cos
2
k
y
	​

a
	​

cos
2
k
z
	​

a
	​

+cos
2
k
z
	​

a
	​

cos
2
k
x
	​

a
	​

]
	​


This is the FCC nearest-neighbor s-band dispersion.

Along ΓX

Use

k=
a
2π
	​

(q,0,0),0≤q≤1

Then

E
ΓX
	​

(q)=ϵ
s
	​

+4t[1+2cos(πq)]
	​

Along ΓL

Use

k=
a
2π
	​

(
2
q
	​

,
2
q
	​

,
2
q
	​

)

Then

E
ΓL
	​

(q)=ϵ
s
	​

+12tcos
2
(
2
πq
	​

)
	​

Along ΓK

Use

k=
a
2π
	​

(
4
3q
	​

,
4
3q
	​

,0)

Then

E
ΓK
	​

(q)=ϵ
s
	​

+4t[cos
2
(
4
3πq
	​

)+2cos(
4
3πq
	​

)]
	​

Along ΓW

Use

k=
a
2π
	​

(q,
2
q
	​

,0)

Then

E
ΓW
	​

(q)=ϵ
s
	​

+4t[cos(πq)cos(
2
πq
	​

)+cos(
2
πq
	​

)+cos(πq)]
	​
Gemini Pro:
FCC nearest-neighbor hopping must be invariant under cubic symmetry.

The lowest allowed symmetric combination from nearest-neighbor hopping is

cos
2
k
x
	​

a
	​

cos
2
k
y
	​

a
	​

+cos
2
k
y
	​

a
	​

cos
2
k
z
	​

a
	​

+cos
2
k
z
	​

a
	​

cos
2
k
x
	​

a
	​

.

Therefore the dispersion must have form

E(k)=ϵ
s
	​

+4t(C
x
	​

C
y
	​

+C
y
	​

C
z
	​

+C
z
	​

C
x
	​

)
	​


where

C
i
	​

=cos
2
k
i
	​

a
	​

.

Then substitute the symmetry-line coordinates above to obtain the same four expressions.

Tier 4: Is ∇
k
	​

E=0 necessarily zero on the square BZ face?
No, not necessarily.
	​


On the square face, symmetry only forces the normal component of velocity to vanish:

∂k
⊥
	​

∂E
	​

=0
	​


because the square face is a Bragg plane, and reflection symmetry makes

E(k
⊥
	​

)=E(−k
⊥
	​

)

locally around that face.

But the tangential components are not forced to vanish:

∂k
∥
	​

∂E
	​


=0

in general.

So:

∇
k
	​

E=0
	​


only at special high-symmetry points such as X, W, or other critical points, not everywhere on the square face.
```

### Your Verdict

No comment on this question

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

**Total interactions this problem set:** _4_

**Models used:**
- Model 1: Chatgpt Thinking 5.4
- Model 2: Gemini Pro
- Other (if any):

**Overall observation:** In 3–5 sentences, describe the most important pattern you noticed across all your interactions this week. For example: did one model consistently outperform the other? Did the models do better on derivations or on conceptual questions? Was there a type of error that appeared repeatedly?

