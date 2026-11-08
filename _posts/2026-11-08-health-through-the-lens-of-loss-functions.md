---
title: "thoughts: health through the lens of loss functions"
date: 2026-11-08
categories: til
---

for machine learning models, the loss function typically is a simple average of the loss of all training datapoints, or for a random sample of them in stochastic batch approaches.

so for example loss = $$ \frac{1}{n} \sum_{i=1}^{n} (\hat{y}_i - y_i)^2 $$

evolution has designed the brain to work similarly. instead of multiple training datapoints, the brain keeps track of multiple different features. how well are you performing in your work, how well are you performing socially, how well is your health and so on. 

the issue with evolution's design is that y isn't fixed. its relative. as a simple example, one proxy for the brain to analyse how well you're doing in work is to compare your income with your peers. the issue is that the brain adapts, which means it keeps on updating the value of ideal y for the income feature. in the income case, loss is not the squared distance but only one way (like ReLU). 

this adaptive feature of the brain is double-edged. the negative is that despite 2026 humans having access to what the wealthiest kings of the past would consider literal magic, there hasn't been much change in the well-being and happiness. the positive is that this relativity keeps humans ambition and making the world (hopefully) an even better place. 

digression aside, the point is that the brain's loss function is not a simple average, it is a weighted average. and the weight for health feature is the highest, so high infact that it overshadows all other features combined. for example, loss = 1000000*(health y - health y current)^2 + other feature loss. 

which is why when you're ill, you forget all the other problems your mind was troubled with. all that matters when you're ill is to recover. and while it kind of sometimes seems stupid in the modern civilization, i think that was the best strategy evolution had. to ensure survival, the best strategy is to infact forget everything else in your life, no matter how important it felt when you were healthy, and focus only and only on your health.

but another health from lens of ML is how health issues are rarely self-diagnosed linearly. they're like ReLU but where the activation starts not at 0 but at some x > 0. you only come to realise something is wrong in your body when a threshold is crossed. i could have a cancer rapidly reproducing inside my body but i won't know it until a threshold point. 
