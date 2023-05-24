# Basic Notions

(under construction)

We use **order** as a generic word for pre-order or posets. The category **Ord** is either the category **Pos** of posets or the category **Pre** of pre-orders, depending on the context.

## Order-Regular Categories

An **order-enriched** category is a category enriched over **Ord**.

An **order-regular** category is an order-enriched category which has
- finite weighted limits and
- coinserters that are stable under pullback.

For the remainder of this section, let us fix an order regular category $\mathcal C$. We denote objects by $A,B,\ldots$ and arrows by $f,g,\ldots$. We write $f\le g$ to express that two arrow $f,g:A\to B$ are ordered.


## Weighted Limits and Colimits

... spans, cospans, ...

- comma objects
- co-comma objects
- co-inserters

**Example:** The order $\sqsubseteq_A$ on $A$ is the comma of the cospan $(1_A,1_A)$.

**Lemma:** $(R,p,q)$ is the comma object of the cospan $(f,1)$ if and only if there is $d$ such that $pd=1, dp\le 1, qd=f$.

*Proof:* Only if is a straight-forward verification. For the other direction see [here](../img/drewslemma.png).

## Factorisation System

Every order-regular category has a factorisation system (E,M) where E is the class of coinserters and M is the class of representably fully-faithful arrows. This factorisation system supports an appropriate 2-dimensional version of the diagonalization property.

We call the arrows in E order-epis and the arrows in M order-monos.

**Example:** In the category Ord, the order-epis are precisely the surjections and the order-monos are precisely the embeddings (=order-reflecing maps).

## Relations

In every order-regular category we can talk about relations and weakening relations. 

A **relation** is a span that is jointly order-mono. [^jointlyOrderMono]

[^jointlyOrderMono]: The span $A\stackrel f \leftarrow C \stackrel g \rightarrow B$ of jointly order-mono if $\langle f,g\rangle: C\to A\times B$ is order-mono. In Ord that means that $C$ can be identified with a subset of $A\times B$ that is ordered pointwise.

**Composition of relations** is via pullback and image factorisation. The identity relation $I_A$ on $A$ is the span $(1_A,1_A)$.

Given an order-regular category $\mathcal C$, we can form the order-enriched category **category of relations** $\sf Rel \mathcal C$, which has as objects the objects of $\mathcal C$ and as arrows the relations of $\mathcal C$.

One can understand the definition of order-regular category as providing precisely what is needed to get the following result.

**Proposition:** In an order-regular category, composition of relations is associative.

**Proposition:** 
- $I_A \ \le \ {\sqsubseteq_A}$ 
- $\sqsubseteq_A \,; \sqsubseteq_A \ = \ {\sqsubseteq_A}$ 


To summarize, the category $\sf Rel\mathcal C$ has:
- For every object $A$ an order $\sqsubseteq_A$.
- For every object $A$ an identity relation.
- For any two relations $R:A\to B$ and $S:B\to C$ the composition $R\,;S:A\to C$.
- Composition is order-preserving and associative.

## Weakening Relations

A relation $R:A\to B$ is a weakening relation if 

$$\sqsubseteq_A\,;R\,;\sqsubseteq_B {} = {} R$$

...

##


