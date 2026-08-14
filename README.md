# Balanced Learning from Attribution Sets

## Abstract

\sloppy
Attribution sets replace the source label of each positive event by a set of candidate examples. The first learning guarantees for this model lose a factor $1/\\|\pi\\|_2^2$, where $\pi$ is the prior over candidates. For a uniform set of size $k$, this gives a leading rate $k/\sqrt n$. Whether that dependence is intrinsic was left open. We show that it is not under stationary attribution. Our estimator attaches a negative control to every reported set. Translation balance cancels both row and column effects of the irrelevant candidates, leaving a canonical order-two statistic. If $\Sigma=\\|\pi\\|_2^2$, its variance is $O(1/(n\Sigma))$ and finite-class empirical risk minimization has leading regret

$$O\\\\\\!\left(\sqrt{\frac{\log(|\mathcal H|/\delta)}{n\Sigma}}\right).$$

Uniform attribution therefore costs only $\sqrt{k}$ rather than $k$. The estimator is exactly unbiased, runs in $O(k)$ time per report, and requires neither the conversion rate nor population feature moments. A four-regime concentration theorem handles all overlap among reported sets through decoupling and sharp canonical U-statistic inequalities.

For uniform attribution, the rate is minimax sharp. On a stationary block instance, an exact likelihood projection gives a matching $\Omega(\sqrt{k/n})$ regret lower bound for two hypotheses and binary labels. We also extend the construction to ordinary paths when the reporter marks a source-defined target cohort. A max-flow argument produces diffuse boundary controls with the same rate. Simulations confirm exact debiasing and the predicted $\sqrt{k/n}$ scaling.

## Contributions

- We give an exactly unbiased score that uses no conversion rate or population moment. It is a weighted sum over the $k$ candidates minus a uniform control over their complement. A global feature sum makes evaluation cost $O(k)$ per report.
- We prove a single-log tail bound with leading scale $1/\sqrt{n\Sigma}$. The proof gives an exact Hoeffding decomposition. Decoupling and the four-parameter inequality of control the overlapping part without discarding reports.
- For finite $\mathcal H$, balanced empirical risk minimization attains $O(\sqrt{\log(|\mathcal H|/\delta)/(n\Sigma)})$ in its Gaussian range. We display the complete tail outside that range.
- For uniform attribution we prove the matching binary-label lower bound. A block-translation mechanism reduces each block to its positive count. Projection of the likelihood onto that count has exact chi-square divergence $\sum_{j=1}^k \rho^{2j}$. Le Cam's method gives $\Omega(\sqrt{k/n})$ regret even for $|\mathcal H|=2$.
- We remove the wraparound idealization for a reporting-cohort design on an ordinary path. A bounded avoidance coupling constructs nonnegative controls outside every candidate window. Numerical audits verify the flow identities and the synthetic experiment confirms the predicted scaling.

## Keywords

balanced, learning, attribution, sets, replace, source, label, each, positive

## Files

- `main.pdf`, `supplement.pdf`
- `main.tex`, `supplement.tex`
- `references.bib`
- `iclr2027_conference.sty`, `iclr2027_conference.bst`, `natbib.sty`, `fancyhdr.sty`
- `main.pdf.ots`, `supplement.pdf.ots`, `README.md.ots` OpenTimestamps priority proofs
