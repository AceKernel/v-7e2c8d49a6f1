# ECON2050 checked course guide

Compiled, source-referenced supplementary guide, not official teaching material, an exam answer key or a marking scheme. Original lectures govern course notation; official tutorials illustrate methods. Check current official corrections.

This text preserves the checked content of the earlier eight-page reference. Any numbered offline-bundle references refer to that earlier pack; use INDEX.md here to find complete original lectures and tutorials.

## Course profile and exam scope

This searchable reference is for ECON2050 revision. It supplements, rather than replaces, the original
course excerpts and official tutorial solutions. The formulas use explicit text notation so they remain
available after PDF-to-text conversion.
Verified exam profile
The revision lecture specifies 16 November 2026; consult the personalised timetable for time and
venue. Standard format: 120 working minutes plus 10 planning minutes; five short-answer questions
with sub-questions; 70 marks; 52% course weighting. Personal approved adjustments, if supplied, take
precedence over standard timing.
Closed book, with one double-sided A4 sheet of handwritten or typed notes permitted. Bring student ID
and a UQ-approved calculator. Write in the designated Gradescope booklet spaces; clearly cross-reference any permitted
additional pages used.
Coverage and priorities
The whole course is examinable. Recurring themes include limits, continuity, domains, graphing and
sets; applying definitions; multivariate differentiation; convexity and concavity; unconstrained and
constrained optimisation. Expect theory, calculations, interpretation and graphs, mostly in practical
applications. The lecturer gives no topic-by-topic mark allocation.
Basic economics is assumed, including marginal products, utility and production functions and shadow
prices. Black-Scholes, arbitrage theory and options-pricing theory are not required: they were
illustrations of linear systems. Do not exclude the underlying linear algebra, feasibility or Farkas
methods.
Source priority and answer style
Current official corrections and exam instructions govern scope. Use lectures for notation and theorem
statements; official tutorial solutions for methods and examples; assignments for style and
interpretation. Student answers are not an official key. Old exams may contain material no longer
applicable; no official old-exam solutions are supplied in the revision lecture.
Give precise variables, assumptions, domains and inequalities. A statement such as prices are positive
must specify whether zero is excluded. Show the necessary working and theorem hypotheses, but
avoid needless background. Treat this profile as a checked study aid, not a replacement marking
scheme.
Sources: Revision lecture, PDF pp. 3-11; Notation p. 3; course Lectures 1-11 and Tutorials 2-11. Tutorial 1 solutions were not
available.

## Notation and real analysis

Sets and vectors
N = {1,2,3,...}; R_+ = [0,∞); R_++ = (0,∞).
R^n_+ contains vectors with every coordinate nonnegative. In the course vector convention, y ≥ z is
coordinatewise; y > z means y ≥ z with at least one strict coordinate; y ≫ z means every coordinate is
strictly greater. Scalar > retains its usual meaning.
||x|| = sqrt(Σ_i x_i^2); B_r(a) = {x : ||x-a|| < r}.
Use |t| for scalar absolute value and ||x|| for vector norm. A × B is the Cartesian product; A \ B removes
elements of B. A point may belong to the boundary even if it does not belong to the set.
Convergence and continuity
x_n → x* iff ∀ε>0 ∃N∈N ∀n≥N: ||x_n-x*|| < ε.
For scalar sequences replace the norm by absolute value. Vector convergence is equivalent to
convergence of every coordinate. Use valid limit algebra and explicit estimates; for ε-proofs choose N
so the required inequality holds for all n ≥ N. Distinct subsequential limits or unboundedness can
establish divergence.
The course defines continuity at x by sequences: for every sequence x_n in the domain with x_n → x,
one has f(x_n) → f(x). One sequence violating this establishes discontinuity. Different path limits
disprove existence, but agreement on a few paths does not prove a multivariable limit.
The projections pr_i(x)=x_i are continuous. Sums, differences, products and valid compositions of
continuous functions are continuous; quotients require a nonzero denominator. Verify that the inner
function stays inside the outer function domain.
Interior boundary exterior and compactness
Interior: some open ball about the point lies in D. Exterior: some open ball about the point is disjoint
from D. Boundary: every open ball meets both D and its complement. Open sets contain only interior
points; closed sets contain all their boundary points.
Bounded: there is K with ||x|| ≤ K for all x in D. In Euclidean space compact means closed and
bounded. For optimisation existence, also establish that D is nonempty. An intersection of closed
half-spaces is closed; strict inequalities may exclude boundary pieces, but classify the actual set rather
than relying only on its displayed symbols.
Source locators: Lecture 1 slides 12,18,25-30; Lecture 2 slides 11,13-18; Notation p. 3. Lecture extracts in 01; worked
examples in Tutorials 2 and 8.

## Calculus domains and regularity

Domain before differentiation
Intersect all restrictions: log arguments > 0; square-root arguments ≥ 0; denominators ≠ 0. Do not
strengthen a square-root condition to strict positivity unless differentiability or the problem requires it.
Nonnegativity and strict positivity are not interchangeable.
Gradient total derivative and approximation
∇f(a) = (∂f/∂x_1(a),...,∂f/∂x_n(a)).
For a differentiable scalar-valued function the course identifies Df(a) with ∇f(a). Partial derivatives
alone do not establish total differentiability. Continuous partial derivatives on an open neighbourhood
are a sufficient condition for continuous differentiability. Differentiability implies continuity.
f(a+h) = f(a) + ∇f(a)·h + o(||h||).
T_a(x) = f(a) + ∇f(a)·(x-a).
T_a is the tangent affine approximation. The total differential is df = Σ_i f_{x_i}(a) dx_i. Distinguish the
approximate change df from the actual change Δf.
Chain rule and Hessian
d/dt f(x_1(t),...,x_n(t)) = Σ_i f_{x_i}(x(t)) x_i′(t).
∂/∂s f(x(s,t)) = Σ_i f_{x_i}(x(s,t)) ∂x_i/∂s.
Use product, quotient and chain rules before substituting a requested point. The Hessian Hf is the
matrix of second partial derivatives. State the row/column order consistently. Under the
continuous-second-partial hypotheses of Young’s theorem the mixed partials agree; symmetry alone is
not a proof of convexity.
Implicit function theorem
For G(x,y)=C near (x0,y0), first check the point is on the level set, G is continuously differentiable on
an open neighbourhood, and G_y(x0,y0) ≠ 0. Then y=g(x) exists locally and is continuously
differentiable.
g′(x0) = -G_x(x0,y0)/G_y(x0,y0).
∂g/∂x_i = -G_{x_i}/G_y (evaluated at the relevant point).
A tangent line is y = y0 + g′(x0)(x-x0). If G_y=0 the theorem does not certify this representation;
check whether solving for a different variable is valid. Do not claim that the local representation is
automatically global.
Source locators: Lecture 2 slide 33; Lecture 3 slides 4-10,22-25,31; Lecture 4 slides 4,7,12-14,19,24. See 01 and Tutorials 3-4.

## Linear algebra and feasibility

Span independence and rank
span(S) consists of real linear combinations of the vectors in S. A finite collection v^1,...,v^k is linearly
independent if Σ_j a_j v^j = 0 implies a_j=0 for every j; dependence requires a nontrivial coefficient
vector. Give explicit coefficients when proving dependence.
Rank is the maximum number of linearly independent vectors. A matrix has equal row and column
rank. To compute rank, identify independent rows/columns or use row operations with justification; do
not infer independence merely from different-looking vectors.
Ax=b is feasible iff b belongs to the span of the columns of A.
For unrestricted x, exactly one holds: (i) Ax=b has a solution; (ii) there exists a row multiplier y with
yA=0 and y·b ≠ 0. A feasible x is a direct certificate. An inconsistent row combination is a certificate of
infeasibility.
Cones and Farkas lemma
cone(A) = {Ax : x ≥ 0}.
cone(A) is generated by COLUMNS of A with nonnegative coefficients. Do not confuse a cone with a
span, whose coefficients may have either sign.
Exactly one: Ax=b, x≥0; OR yA≥0, y·b<0.
In this Farkas alternative y is not automatically nonnegative. Derive any extra sign restrictions from
the transformed system, not from memory of a different formulation. Verify every inequality in a
proposed certificate.
Useful inequality variants and conversions
Ax≤b, x≥0: alternative y≥0, yA≥0, y·b<0.
Ax≥b, x≥0: alternative y≥0, yA≤0, y·b>0.
Ax≤b, x free: alternative y≥0, yA=0, y·b<0.
Add a nonnegative slack for a ≤ constraint, subtract a nonnegative surplus for a ≥ constraint, and
replace a free variable by x_j = u_j-v_j with u_j,v_j ≥ 0. Check dimensions and keep the transformed
matrix columns in their declared order.
Source locators: Lecture 5 slides 4,6,10,19,21; Lecture 6 slides 3,5,8,16-18. See 02 and Tutorials 5-6. Finance-specific pricing
examples are not needed for the final.

## Convexity and concavity

Definitions
[x,y] = {λx+(1-λ)y : 0≤λ≤1}.
S is convex if [x,y] is contained in S whenever x,y are in S. For a proof, choose arbitrary x,y in S and λ
in [0,1], then verify the defining constraints at the convex combination. One counterexample segment
is enough to disprove convexity.
Convex f: f(λx+(1-λ)y) ≤ λf(x)+(1-λ)f(y).
Concave reverses the inequality. Strict convexity/concavity uses distinct x,y and 0<λ<1 with a strict
inequality. An affine function is both convex and concave, generally not strict. Verify the domain is
convex before applying these definitions/theorems.
Course closure and derivative methods
Nonnegative weighted sums preserve convexity or concavity. Negation exchanges them. An increasing
convex outer function composed with a convex inner function is convex; the analogous
increasing-concave composition is concave. An affine inner function allows convex/concave
composition without outer monotonicity, on the valid domain.
For a twice differentiable scalar function on an open interval: f″≥0 characterises convexity; f″≤0
characterises concavity. Strict positivity/negativity is sufficient for the corresponding strict property,
not a necessary condition at every point.
Concave differentiable f: f(x)-f(a) ≤ ∇f(a)·(x-a).
For the course first-order characterisation assume an open convex domain and continuous
differentiability. Convex reverses the displayed inequality. Concave graphs lie below their tangent
hyperplanes; convex graphs lie above. Follow a requested definition proof rather than substituting an
unrequested derivative/Hessian test.
Sets associated with functions
epi(f) = {(x,t): x∈S, t≥f(x)}.
hyp(f) = {(x,t): x∈S, t≤f(x)}.
Convex f has a convex epigraph; concave f has a convex hypograph, with converse equivalences on a
convex domain. Convex-function sublevel sets and concave-function superlevel sets are convex.
Intersections of convex sets remain convex; unions need not.
Source locators: Lecture 7 slides 4,9,11,13,16-18,20,22-26; Tutorial 7 Problems 1-5; Tutorial 8 Problem 1. See 02 and 04.

## Optimisation and linear programming

Existence and unconstrained optimisation
Extreme value theorem: a continuous real-valued function on a nonempty compact D attains a global
maximum and a global minimum. Establish nonemptiness, closedness, boundedness and continuity. If
an assumption fails, the theorem is unavailable; nonexistence does not follow automatically.
At an interior local extremum of a differentiable function, ∇f=0. Critical points need not be extrema. On
a convex domain, a critical point of a concave function is a global maximiser; for a convex function it is
a global minimiser. Strict curvature gives uniqueness when an optimiser exists.
For a compact feasible set, inspect interior critical points and all relevant boundary pieces/corners,
then compare objective values. A boundary optimum need not have zero ambient gradient. Convert
minimisation to maximisation of -f if using the course maximisation conventions. Strictly increasing
transformations preserve the optimiser set but change the objective value.
Primal dual and complementary slackness
Primal: max c·x subject to Ax≤b, x≥0.
Dual: min y·b subject to yA≥c, y≥0.
Use the course row-vector multiplier notation. Standardise signs carefully. A primal equality gives a
free dual multiplier; a free primal variable gives an equality dual constraint. Check the correct
correspondence before applying the general rule.
Weak duality: c·x ≤ y·b for feasible x and y.
If feasible primal and dual points have the same objective value, both are optimal. Strong duality
equates attained finite primal and dual optima. If the standard LP has an optimum, some feasible
extreme point is optimal; this does not mean every optimal point is a vertex.
y_i(b_i-(Ax)_i)=0; x_j((yA)_j-c_j)=0.
Binding means equality; slack means a strict inequality. Slack constraints have zero optimal multipliers
under complementary slackness, but a binding constraint can also have zero multiplier. At a
differentiable value function, the optimal resource multiplier is a local marginal change in optimal
value per unit of that resource. Interpret units and constraint scaling.
Source locators: Lecture 8 slides 4,6,11,16,18-19,23; Lecture 9 slides 7,9,11-13,17,24-26; Lecture 10 slides 2-4. See 03 and
Tutorials 8-9.

## Lagrange and KKT conventions

Maximisation with inequalities
max f(x), g_j(x)≤0; L(x,λ)=f(x)-Σ_j λ_j g_j(x).
∇f(x*)-Σ_j λ_j*∇g_j(x*)=0.
g_j(x*)≤0, λ_j*≥0, λ_j* g_j(x*)=0.
For equality constraints h_k(x)=0 use free multipliers μ_k and include -Σ_k μ_k h_k in L. Do not impose
nonnegative signs on equality multipliers. For a minimisation, convert the objective to -f before
applying these maximisation signs; do not mix conventions halfway through.
Reduced KKT form for nonnegative variables
When x_i≥0 is handled separately, the reduced Lagrangian omits explicit multipliers for these
nonnegativity constraints, but the following conditions retain their effect.
∂L/∂x_i ≤ 0; x_i(∂L/∂x_i)=0; x_i≥0.
g_j(x)≤0; λ_j≥0; λ_j g_j(x)=0.
If x_i>0 its reduced stationarity expression is zero. If x_i=0 it need only be nonpositive. Do not set all
reduced derivatives equal to zero and silently discard corner candidates.
Necessity sufficiency and candidate completeness
For necessity check the theorem hypotheses: an open domain, continuous differentiability and either
affine constraints or the relevant linear-independence constraint qualification. When checking active
gradients, include active nonnegativity constraints. At qualification-failure points, absence of
multipliers is not enough to rule out an optimum.
Use complementary slackness to enumerate binding/slack cases. Solve each case, check multiplier
signs, feasibility, domain and objective value, and retain qualification-failure candidates when the
course procedure calls for them.
For global sufficiency use a convex ambient domain, concave objective, convex inequality functions
and appropriate multipliers satisfying all conditions; affine equality constraints preserve the relevant
convex geometry. If this theorem is unavailable, establish existence and compare the complete
candidate set, or use another valid global argument. A solution of necessary equations alone proves
neither existence nor global optimality.
Source locators: Lecture 10 slides 13-15,25-28; Lecture 11 slides 5-7,9,16,18,20,22. See 03 and Tutorials 10-11. General
formulas here are checked; do not copy isolated typesetting slips in original slides.

## Checked revision examples and source map

Line segments and domains
Revision appended example: between (2,-1) and (-4,5), the midpoint is (-1,2). The point (0,1)
corresponds to λ=2/3 in λ(2,-1)+(1-λ)(-4,5), so it is on the segment. For endpoints (-3,2),(5,6), the
point (9,8) gives λ=-1/2: it is on the line, not the segment.
ln(4-x_1^2-x_2^2)+sqrt(x_1): D={x∈R²: x_1²+x_2²<4, x_1≥0}.
The straight diameter segment with -2<x_2<2 is included; the circular arc and both endpoints (0,±2)
are excluded. For 1/(x_1-x_2)+sqrt(x_1 x_2), the domain is {x∈R²: x_1 x_2≥0, x_1≠x_2}; the origin is
excluded.
Derivatives and optimisation
f(x,y)=x³y²-4xy+ln(y), y>0.
f_x=3x²y²-4y; f_y=2x³y-4x+1/y.
Hf=[[6xy², 6x²y-4], [6x²y-4, 2x³-1/y²]].
Hf(1,1)=[[6,2],[2,1]].
The function is C² on y>0, so Young’s theorem applies there. The correct reason is the regularity
hypothesis, not simply that a calculation happened to give equal mixed partials.
q(x,y)=-2x²+2xy-y²+4x = 4-(x-2)²-(x-y)².
Thus its unique global maximum is 4 at (2,2). There is no global minimum: along x=0, q(0,y)=-y² tends
to -∞. For the vectors (1,2),(3,6), 3(1,2)-(3,6)=0 is a nontrivial relation; they are dependent and have
rank one.
