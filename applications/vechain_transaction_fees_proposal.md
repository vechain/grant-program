# VeChain grant research proposal template

## Title

Transaction fees stability; policy making and incentives in VeChain

## Applicants

**(Mr) Nicola Dimitri (the only applicant)**, https://docenti.unisi.it/en/nicoladimitri, Professor of Economics, Department of Economics and Statistics www.deps.unisi.it, University of Siena www.unisi.it, Piazza San Francesco 7, 53100 Siena-Italy.

This proposal is a follow-up of a previous project, “The Economics of VeChain”, and therefore my profile is already well known to VeChain. However, for your perusal, below I replicate the information I introduced in the previous project. 

“For completeness I have mailed my CV to grant@vechain.org from which you can evince my profile and experience. As you can see, my main recent research interests are in game theory, auctions and their applications, blockchain and cryptocurrencies. I would also like to point out that, besides Vechain, I’ve been involved in few other blockchain-based projects.  

Let me also notice I am currently Associate Editor of the journals “Frontiers in Blockchain” and “IET Blockchain”.


## Payment Address
USDT(ERC-20):0x57c1aaab04c8de5f4404f1b0cf2cf795159f9204


## Summary

The project is a follow up of the previous one, and its goal is to develop a point which has been just mentioned in the Improvement paper. Indeed, in that paper, taking up from the following sentence drawn from the Vechain White Paper 

 > "The design of the two-token model intends to maintain stable and predictable transaction cost (in fiat) of using the VeChainThor blockchain" (italics is mine) (1)

I begun a discussion on the needed relationship, between the gas price in terms of $E$ (VTHOR) tokens and the $E$ token market price in terms of a fiat currency ($), for (1) to be satisfied. In fact, while it is intuitive that to satisfy (1) the two prices should be related, to our knowledge no work has been undertaken to investigate in what precise relation they should stand. This is a very important point for VeChain policy making, and that’s why the analysis of such relation is a main goal of this project. In the paper we also plan to discuss what kind of policy decisions and incentives schemes VeChain may consider, in case the market would not spontaneously satisfy (1). Indeed, this may occur because E tokens are requested for different, independent, reasons: to pay for gas but also to buy crypto and fiat currencies in exchange nodes. Therefore, it is immediate to realize that several quantities should take the right value for (1) to obtain, and to achieve those values VeChain may need to introduce a proper incentive scheme for the users.                


### Main field of research

Transaction fees; policy making; incentive mechanisms 


### Keywords

Monetary dynamics; transaction fees; incentives

## Research proposal (main body)

The applicants may use any preferred structure to state this part as clear as possible. It is recommended for the applicant to include the following parts.

### Problem Statement

Based on the above Summary, the project aims to produce one paper to study in details how sentence (1) could be satisfied. The main conceptual point underlying the study is that transaction costs in fiat do not depend only of the gas price expressed in terms of E tokens, but also on the E tokens price in fiat, because this will also contribute to drive demand for E tokens to pay gas. In general, the higher the market price for E tokens the lower demand for gas we expect to be. Empirical evidence suggests that the market price in fiat of E tokens changes over time, which implies that (1), namely stability of the transaction fees in fiat, must be guaranteed by a proper adjustment of other relevant quantities. Broadly speaking, such adjustment could be obtained by introducing policy measures and appropriate incentive compatible schemes, by VeChain, inducing the users to undertake the actions desired by the platform. Below, when discussing the approach, I elaborate more on this. For this reason, I believe that the outcome of the analysis could offer to the platform users, and governors, a fruitful perspective on how to stabilise transactions fees in fiat and, relatedly, how the main monetary variables should evolve to fulfil such goal.


### Contributions
To the best of my knowledge, the paper would be the first contribution presenting a rigorous investigation on how to satisfy (1) in a two-token blockchain platform such as VeChain. 

### Background
Together with the VeChain White Paper, the relevant background is represented by the two papers that I wrote for the project previously funded by VeChain. Indeed both the main paper and, more notably, the Improvement Proposal Document contain (with their related literature) the main economic elements, and questions, that I plan to develop in this follow up project.  

### Approach

The approach I intend to adopt takes its main inspiration from a discussion already undertaken in the Improvement Proposal Document of the previously funded project. To briefly illustrate the issue consider the following very simple formalization of the problem, drawn from that document.

For the sake of simplicity consider just two blocks $b=0,1$, and suppose that (1), over the two blocks, is formalised by the following formula 


$$ p(0)G(0)w(0)=p(1)G(1)w(1) \quad  with \  b=0,1 \quad(2)$$ 


where $p(b)$ is the average, unit, price of the Gas ($G$) at block $b$, expressed in terms of $\frac{E}{G'}G(b)$  the total amount of gas used for the transactions included in block $b$ and $w(b)=\frac{D(b)}{S(b)}$ the market price of E tokens expressed in terms of fiat (US Dollar) $\frac{\\$}{E'}$, at block $b$, with $D(b)$ being the demand (in $\\$$) for $E$ tokens and $S(b)$ the supply of $E$ tokens in the market. Notice that alternative notions of transaction fees stability are conceivable, as in fact I do in the VeChain Improvement Proposal with the condition $w(0)=w(1)$.

It turns out that to satisfy (1) the following relation must hold between $p(1)$ and $p(0)$ 

$$ p(1)=sp(1)=\frac{d(01)(Vv+p(0)G(0)0.3-h(1))}{(Vv-p(0)G(0)(1-d(01))-h(0))} - \frac{G(0)_0}{G(1)}p(0) \quad(3)$$

where $sp(1)$ stands for the level of $p(1)$ which establish stable transaction fees in fiat,  $d(01)=\frac{D(0)}{D(1)}$, $V$ is the total quantity of $VET$ tokens, $v$ the rate at which $E$ tokens are generated from $VET$ tokens and $h(b)$ the total holdings of $E$ tokens in the users’ wallets at block $b$. According to (3) it is evident that $p(1)$ must be related to $p(0)$ in a way that is precisely determined by several different quantities. Since $p(b)$ is freely chosen by the users, in principle there is no guarantee that (3) would obtain. So, what could VeChain do to satisfy equations like (3)? 
 
If, for example, $p(1)>sp(1)$ and, based on such difference, VeChain expects that also for the next block $p(2)>sp(2)$ an analogous inequality may hold, then the platform could try to obtain $p(2)=sp(2)$  for $b=1,2$ in several different ways. Indeed, it could decide to operate directly on the open market by intervening on the market demand/supply before the next block is validated, alternatively may change the overall supply $V$, the rate $v$ or else. 

However, it may not be easy to stabilize transactions fees in fiat currency almost instantaneously, between two or even few consecutive, blocks by VeChain. From a decision making point of view then, the above policy measures could be taken when $p(b)$ differs from $sp(b)$  on a certain number of blocks, and/or possible differences between $p(b)$ and $sp(b)$ are within a specified band of tolerance. 

Alternative, or complementary, ways to target transaction fees’ stability could be to introduce some kind of automatic stabilizers, for example, as follows. Suppose $4p(1)>sp(1)$. Then, to smooth out an expected increasing trend the price effectively paid by the users $ep(2)$ could the equal to the one that they offered $p(2)$ minus $p(1)-sp(1)$, that is    

$$ ep(2)=Max(0,p(2)-(p(1)-sp(1)))  \quad (4) $$

That is, subtracting from $p(2)$ the difference $p(1)-sp(1)$ may automatically revert the price trend towards the level providing transaction fee stability, of course if the expectations on such trend were correct.

Finally, if $p(1)>sp(1)$, and if Vechain is expecting that it will also be $p(2)>sp(2)$ then it may introduce an incentive scheme such that $ep(2) < p(2)$ if the monetary holdings and/or demand for gas take the values needed to establish  $p(2)=sp(2)$.
   
Analogous arguments could be followed adopting $w(0)=w(1)$ as stability condition. 
  
To summarise, the above considerations illustrated in a very simple way the issues that I intend to enquire.  In the paper I plan to develop extensively the investigation, which will be discussed for any number of blocks and with the due details in so far as the effectiveness of the alternative mechanisms, to target transaction fees stability, is concerned.



### Risks
As for the previous project, the study will be based on economic (mathematical) models, and so no particular risks are expected.


## Milestones

Upon approval, the project will start at an agreed upon date.
Then, these are the proposed milestones
1.	Presentation, possibly in a seminar, of the draft of the paper for comments (after 5 months from the start)
2.	Finalization of the paper, in collaboration with the VeChain team for an improvement plan of VeChain's monetary policy (after 10 months from the start)
3.	Submission of a VeChain Improvement Proposal (VIP) on the monetary policy of VeChain (after 12 months from the start)


## Budget

The budget requested is, as for the previous project, 30.000$. This is because I plan to dedicate about 60 days of work to the paper, over the year-long project. Considering that for academic, scientific, consultancy on average I’m paid a daily rate of about 450€ (roughly 500$) this explains my request.

My proposal would be to split the payment, over the three milestones, according to the following criterion:

1.	12000$ at the beginning
2.	9000$ upon approval of the first draft of the paper
3.	9000$ upon approval of the final version of the paper and of the VIP



## References
The following are three standard references on closed and open macroeconomic systems, micro-founded.

-	Blanchard O. Fisher S., Lectures in Macroeconomics, MIT Press (1989)
-	Romer D., Advanced Macroeconomics (4th Ed), McGrawHill (2012)
-	Obstfeld M., Rogoff K., Foundations of Intyernational Macroeconomics, MIT Press (1996)
This is a standard reference for the game theory part of the paper
-	Osborne M., Rubinstein (1994) A Course on Game Theory, MIT Press
This list of papers is drawn from my CV, as my publications closed related to blockchain and cryptocurrencies
-	Coordination in an EMAIL Game without “Almost Common Knowledge: Journal of Logic, Language and Information 12, 1-11 (2003)
-	Correlated Communication; in “Cognitive Processes and Economic Behavior” (Dimitri-Basili-Gilboa eds), Routledge-London (2003)
-	Efficiency and Equilibrium in the EMAIL Game; The General Case : Theoretical Computer Science, 314, 335-349, (2003)
-	Bitcoin Mining as a Contest, Ledger, 2, 31-37 (2017)
-	The Blockchain Technology; Some Theory and Applications, Maastricht School of Management Working Paper, 2017/3 (2017)
-	Transaction Fees, Block Size Limit and Auctions in Bitcoin, Ledger, 4, 68-81, (2019)
-	Monetary Dynamics with “Proof of Stake”, Frontiers in Blockchain doi: 10.3389/fbloc.2021.443966 (2021)
-	Consensus: Proof of Work, Proof of Stake and Structural Alternatives, in Enabling the Internet of Value, (Tasca P.-Vadgama N. eds) pag. 29-36, Springer Verlag, (2022)
- The Economics of Consensus in Algorand, Fintech, 2,164-179 (2022)
-	Quadratic Voting in Blockchain, Information, 13,305 (2022)
-	Proof of Stake in Algoorand, ACM Diistributed Ledger Technologies: Research and Practice (2022) 
-	Liquid Proof of Stake in Tezos: An Economic Analysis, Information, 13,556 (2022) 
I truly hope that also this project will be found interesting for the VeChain Foundation and considered for additional collaboration and funding. 
