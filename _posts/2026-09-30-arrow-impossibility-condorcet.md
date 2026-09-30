---
title: "condorcet's paradox and arrow's impossibility theorem, spoiler effect"
date: 2026-09-30
categories: til
---

consider a election where there are 3 candidates and 3 voters. voter 1 prefers A>B>C, i.e. voter 1 likes A the most, then B and then at last C. Voter 2 has B>C>A, and voter 3 has C>A>B.

we can see that majority voting system doesn't work in this case. suppose A gets elected, then voter 2 and voter 3 would rather prefer C over A and since 2/3 is the majority, C should be elected. but if C is elected, then we have two voters who would rather prefer B over C. this argument can be extended ad infimum. therefore majority voting system doesn't always work properly.

arrow's impossibility theorem says that we cannot have any voting method that follows the 3 criterias of fairness. the 3 criterias are unanimity - if everyone prefers A to B, then the result also should have A over B. no dictatorship - one person's ordering should not determine the result. independence of irrelevant alternatives - adding a candidate C should not change people's ordering about A and B. for example if a person preferred A>B before C joined the race, their ordering afterwards could be C>A>B or A>C>B or A>B>C but cannot be B>C>A.

spoiler effect refers to the phenomenon where a losing candidate alters the result of voting simply by participating. that is, if the candidate hadn't participated, the result would have been different. 

the [wikipedia page](https://en.wikipedia.org/wiki/Spoiler_effect) has a nice explanation of the independence of irrelevant alternatives - 

>A man is deciding whether to order apple, blueberry, or cherry pie before settling on apple. The waitress informs him that the cherry pie is very good and a favorite of most customers. The man replies "in that case, I'll have the blueberry."
