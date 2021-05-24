# Rainbow Option Valuation

FinPricing provides valuation models for
	Rainbow Option without Bucketing
	Rainbow Option with Bucketing
	Rainbow Option with Floor
	Asian Rainbow Option
	Digital Rainbow Option

A rainbow option is an option on a basket that pays a non-equally weighted sum of returns over all assets in the basket according to their performance, where individual asset returns are computed as the percentage growth from initial levels to final levels that may be averages over multiple dates.

Rainbow options are multi-asset options that have a payoff depending on the assets by their performance at maturity. When the rainbow only pays the best (worst) performing asset of the basket, it is also called the best (worst) of performing option.

The number of assets is called the number of colours of the rainbow, as the option is based on a combination of various assets just like a rainbow is a combination of various colours. The assets are sorted by their performance at payment date. Asian rainbow option is a common version of rainbows where the return of an asset takes an average, as the Asian rainbow is usually cheaper than the vanilla one. 

The payoff function can be specified in the form of a put, call or a forward (pure return). The structure is unique in the way the weights are applied to assets in computing the payment. First, assets may be grouped into buckets each containing one or more asset. A vector of weights is then applied to the ranked bucket returns based on performance. 

Rainbow options are appealing to investors due to its natural risk diversification, cost efficiency, and weighted average on the best or worst performing assets. The best version offers higher returns, whereas the worst version is normally cheap.


Due to the complexity of the payoff structure, the option is normally priced via Monte Carlo simulation. 


References:

https://finpricing.com/lib/EqRainbow.html

https://bitbucket.org/cmrm11/eqrainbow/downloads/EqRainbow-24.pdf

