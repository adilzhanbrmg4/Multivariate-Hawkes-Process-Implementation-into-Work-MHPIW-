We will be integrating Multivariate Hawkes Process and Rough Path Theory in this paper. To start, let's define what we are working with. 
**Rough Path Theory**
Let ∆T = {(s, t) : 0 ≤ s ≤ t ≤ T }. A control function is a continuous map ω: ∆T → [0, ∞) which is super-additive,
i.e. ω(s, t) + ω(t, u) ≤ ω(s, u) for all 0 ≤ s ≤ t ≤ u ≤ T. Here the control function measures the local size of the path over [s,t]. It also states that control function is a continuous map function that will map every time increment to a specific value. That super - additive function will help us to measure how irregular the path is. That means the combined values will be equal or greater than their sum. There is also an interesting detail here, which states, that w - function (control function/continuous function) is regulated in size, due to constant beta. This ensures that any error vanishes rapidly in order to form unique path from convergence of Riemann type sums.
"Lemma 2.1 (Sewing). Consider β > 1, a real Banach space V , and a control function ω. Let
Ξ: ∆T → V be a continuous map such that, for all 0 ≤ s ≤ u ≤ t ≤ T ,
kδΞs,u,tk ≤ ω(s, t)^β,
where δΞs,u,t = Ξs,t − Ξs,u − Ξu,t. Then there exists a unique function ξ : [0, T ] → V such that
ξ0 = 0 and
|ξs,t − Ξs,t| ≤ Cω(s, t)^β"
In this extract, you can see the whole Sewing Lemma quotation.

Now, the Sewing Lemma assumes the Banach Space foremost, which means we are dealing with complete normed vector space. In the market, those vectors in Banach Space V could be cumulative filled volume, order flow imbalance, or aggregate sentiment scores derived from discrete event streams. Now, above in the quote provided, you saw the unique function mentioned. This function is essentially mapping the time increments onto a Banach space. This further solidifies the idea of implementing time - series model and metrics directly into Rough Path Theory, because it normalises metrics into complete space of normed vectors.
