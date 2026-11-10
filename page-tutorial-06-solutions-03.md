# Tutorial 6 solutions: P3: Deriving inequality alternatives

PDF page 3 of 4.

[Page map](map-tutorial-06-solutions.md) | [Original PDF page](tutorial-06-solutions.pdf#page=3) | [Previous](page-tutorial-06-solutions-02.md) | [Next](page-tutorial-06-solutions-04.md)

Topics: farkas.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
(1) There are (at least) two ways to solve this part. One way is the standard way: we
subtract a surplus variable s1 ≥0 to each of the inequalities, Pn
j=1 aijxj ≤bi to
convert it to an equality Pn
j=1 a1jxj −si = bi. For notational convenience, let s ≡
(s1, s2, . . . , sm) be the surplus vector; we have s ≥0. Determining the solvability of
Ax ≥b for x ≥0 is equivalent to solvability of Ax−s = b where x ≥0 and s ≥0,
which is in turn equivalent to solvability of Ax−Is = b, where I denotes the m×m
identity matrix.
Set B ≡[A| −I] and z ≡(x, s), the system can be written as Bz = b and z ≥0.
Applying the Farkas lemma to this system, we get y′B ≥0 and y′ · b < 0. Since
B = [A| −I], this is equivalent to
y′A ≥0,
y′ ≤0,
and
y′ · b < 0.
Finally, since we need to prove a statement about a non-negative y ∈Rm, we set
y ≡−y′ ≥0, and the Farkas alternative is
yA ≤0,
y ≥0,
and
y · b > 0.
The other approach, which is arguably much more straightforward but didactically less
helpful, is essentially a trick: note that Ax ≥b can be written as −Ax ≤−b; define
C ≡−A and d ≡−b, the system can be written as Cx ≤d and x ≥0. Then as we
discussed in the lecture, the Farkas alternative for the system is yC ≥0, y ≥0, and
y · d < 0. By the definition of C and d, this is equivalent to
yA ≤0,
y ≥0,
and
y · b > 0.
(2) Recall that in the lecture we mentioned that for a variable, xj, that is unrestricted
in sign, we can replace it by two non-negative variables zj and z′
j by setting xj =
zj −z′
j. Since x is unrestricted in sign, applying this to every component of x =
(x1, x2, . . . , xn), we get
x = z −z′,
where z ≡(z1, z2, . . . , zn) ≥0, and z′ ≡(z′
1, z′
2, . . . , z′
n) ≥0. Now the system
Ax ≤b is equivalent to the system
A(z −z′) ≤b,
z ≥0,
and
z′ ≥0;
and A(z −z′) ≤b can also be written as Az −Az′ ≤b.
Set D ≡[A| −A] and w ≡(z, z′), the system can be expressed as
Dw ≤b
and
w ≥0.
The Farkas alternative of this system is
yD ≥0,
y ≥0,
and
y · b < 0.
Since D = [A| −A], this system is equivalent to
yA ≥0,
yA ≤0,
y ≥0,
and
y · b < 0,
which can be further simplified to
yA = 0,
y ≥0,
and
y · b < 0.
3
```
