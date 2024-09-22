# Book_ZeroDeepLearning6
# ゼロから始めるDL (生成モデル編)

## 内容
1. 多次元正規分布
2. 潜在変数モデル $p(x) = \int_{z} p(x, z) dz$
3. KL情報量 (相互情報量) $D_{KL}(p(x) || q(x)) = E_{p(x)}[log\frac{p(x)}{q(x)}] = \int_{x}p(x)log\frac{p(x)}{q(x)}>= 0$
4. ELBO (Evidence Lower Bound) $ELBO = \sum_{k=1}^{K}q(z^{k})\frac{p(x,z^{k})}{q(z^{k})}$
5. log-sum形式の尤度=ELBO + KL情報量
6. KL情報量の最小化は, ELBO最大化. つまり log-sum形式の尤度=ELBO( $\theta_{old}$ ) 
7. 潜在変数zの確率分布 $q(z)$ を 厄介な確率分布 $q(z | x)$ に近づけることが, EMアルゴリズム.
8. 負担度: $q(z | x)$
9. VAE (Variational Auto Encoder)
10. 拡散モデル
