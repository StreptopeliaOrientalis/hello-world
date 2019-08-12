## Stat thinking-Youtube Channel - Cassie Kozyrkov 

### 1 What is statistics?

[1] How many fish are in this fishbowl?
[2] Is it possible for goldfish to be of different colors from one another?
[3] Is it possiblw for goldfish not to be gold-colored?
Are these questions about data?
Are these statistical questions?

No. That's analytics, not statistics. 
[1] Statistics is about going beyond the data.
[2]\[3] You can answer the questions with certainty. 

So what is statistics?

> Statistics is the science of **making decisions** under **uncertainty**. 
>
> —Savage, The foundations of Statistics, 1954

I like to think of statistics as the science of changing your mind. 

**Bayesian** statisticians change their minds about beliefs. They like to report results using credible interbals.

**Frequentist** (classical) statistician change their minds about acitons. 

### 2 Population, Sample, Observation

**Population**: the collection of **all items** ==we are interested in==(for your decision).

**Sample**: any subset of the population of interest

**Observation**: any single measurement in the sample

A legal contract in Statistics: The truth (population), the whole truth (population) and nothing but the truth (population). 

### 3 What is s statistic?

**statistic**: a summary measure computed from a sample

(anyway of mushing up data.)

**Statistics**: the science of changing your mind under uncertainty.

### 4 Proof that statistics are boring

By definition, only the population is interested to you.

We took some boring trees, and get some data of the boring trees, and we mash up these data. What comes out must be boring.

**The Digestion of Statistics ==)Statistics**

Statistics digests your statistic into something that helps you take a reasonable course of action involving the population.

### 5 Parameter

**parameter**: summary measure of a population

**statistics**: a summary measure computed from a sample

When you have all the data you're interested in, the sample is the population. You've got the answer with certainty.

Let's make a reasonable decision based on partial information.

### 6 Uncertainty

If you don't have all the information, you can't know the answer. That's what it means to be uncertain.

### 7 What is a hypothesis?

**parameter**: the number we wish we knew for our decision. 

**hypothesis:** description of how the parameter might look

### 8 Estimate

the facts(data) we have:

- Sample: subset of the population of interest
- Statistic: summary computed from a sample
- observation: a single measurement in the sample

the facts we wish we have:

- Population: collection of all items we are interested in
- ParameterL summary in a poopulation

attempts to bridge the gap:

- hypothesis: description of how the parameter might look
- Estimate: a best guess about the true value of a parameter

method of moments estimation, maximum likelilhood estimation...

Which of those two guesses, the first, based on one data point, or the second, based on all those, forms the better guess.

More data makes the estimate better!

(as long as it's relevant data.)

**But how much better? And is your best guess good enough?**

【TBC】



### P-value: how ridiculous is "rediculous"?

我的理解：

我们做的事：

先提出一个想象的世界，

用真实值测出来和它相差不远的话（p不小），我们就接受这个假设（不拒绝：样本值与总体值相差不远）

真是值测出来与它相差很大的话，（在那个假想的世界里面测出这个值的概率很小的话），我们就拒绝这个假设

All of hypothesis testing is about asking: does our evidence make the null hypothesis look rediculous? Rejecting the null hypothesis means we change our minds. Not rejecting the null means we ==leaned nothing interesting==, just like ==going for a hike in the woods and seeing no humans doesn't prove that there are no humans on the planet.==It just means we didn't learn anything interesting about humans existing. If you learned nothing, you have no reason to change your mind, so keep doing that default action. 

---

review:

So what is statistics?

> Statistics is the science of **making decisions** under **uncertainty**. 
>
> —Savage, The foundations of Statistics, 1954

We can walk to class together (default action) if you ususally take under 15 minutes to get ready (null hypothesis), but if the evidence (data) suggests it's longer (alternative hypothesis), you can walk by yourself because I am otta here (alternative action).

---

Type I: 弃真（太严）

Typr II: 纳伪（太宽）