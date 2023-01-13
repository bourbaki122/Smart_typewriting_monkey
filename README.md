# Smart_typewriting_monkey
__________
Provide a monkey with a typewriter keyboard and give him the enough amount of time. What would be the result? Most people assert that the result will be the entire work of Shakespiere (see the [Infinite monkey theorem](https://en.wikipedia.org/wiki/Infinite_monkey_theorem)). The reason behind this is the following: from the monkey point of view, language is just a random process that samples the letters from the english alphabet $\mathcal{A}=\{a,b,c,d,e,\dots,x,y,z\}$, with some particularly probability measure $P:\mathcal{A}\rightarrow [0,1]$. If the monkey is unaware of the statistical structure of the english language he will, as a first guess, choose the distribution $P$ to be the uniform one. In this case, there is a probability that the monkey indeed type the whole work of Shakespiere. However, this probability is ridiculously low. As an example consider the probability of only typing the word "Hamlet" from a uniform alphabet of $|\mathcal{A}|$ letters, e.g.

$$\text{prob}(\text{Hamlet})=\left(\frac{1}{|\mathcal{A}|}^{6}\right) = e^{-6\log|\mathcal{A}|}.$$

This probability exponentially decreases with the length of the word and to get an idea of how ridiculously improbable becomes to write a single page, notice that in a typical book the number of characters per page is around 1000, now try to put this number in an standard calculator to see the result.

On the other hand, if the monkey is initially aware of the inherit statistically structure in the english language, he will immediately recognize that there are correlations between letters, and certain combinations among them that are highly forbidden. This is what I mean by an "smart" monkey, i.e. one capable to recognize the correlations for his benefit!

In this notebook we will build up an smart monkey, which is capable to retrieve the information form a dataset of approximately three-million words taken from [here](https://github.com/dwyl/english-words). This project is intended with pedagogical reasons, but who knows, maybe in the future it could turn into something else.
