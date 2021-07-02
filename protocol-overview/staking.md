# Staking

Users can stake the claim tokens they receive from underwriting the Risk Harbor pool in exchange for non-transferable tickets \(tix\), which will eventually be redeemable for governance tokens. We designed the staking rewards to incentivize underwriters to provide capital at low price points in pools that have low underwriting capital. To achieve this, we provide additional weight to underwriting positions at low price points and distribute a fixed amount of tickets at each block. Since total ticket rewards are fixed at each block, pools with more underwriting capital will have lower per dollar ticket rewards. Since weight scales inversely to price point, low price points maximize ticket rewards. 

The price point weights are given by:

$$
w_p = \frac{1}{2^p}
$$

Plotted Below

![](../.gitbook/assets/w_pvsprice_point.png)





We use the following formula to calculate individual staking rewards per block:

$$
R_{ib}= \tau_b \frac{\overbrace{\sum_{p \in \mathcal{P}} a_{ip}w_{p}}^{\text{Weighted Individual Capital}}}{\underbrace{\sum_{j =1}^n\sum_{p \in \mathcal{P}} a_{jp}w_{jp}}_{\text{Weighted Total Capital}}}
$$



Where$$R_{ib}$$are the returns for underwriter $$i$$ in block $$b$$, $$\tau_b$$ is the total ticket rewards allocated to stakers at block $$b$$, $$a_{ip}$$ is the amount that underwriter $$i$$ has staked at price point $$p$$, $$w_{ p} $$ is the weight associated with the price point $$p$$ and  $$\mathcal{P}$$ is the set of all supported price points.



