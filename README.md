# Yiwei's Problem Set 1
## Project information
- **Author**: Yiwei Liang, Computation and Design with tracks in Computer Science, Class of 2025, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Problem Set No.1 or Final Project for [COMPSCI/ECON 206 Computational Microeconomics, 2023 Spring (Seven Week - Second)](https://ce.pubpub.org/) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: [How to Acknowledge?](https://www.scribbr.co.uk/thesis-dissertation/acknowledgements/)
[notes: please include all professors, students, and staff who have contributed to your completetion of the project.]
- **Project Summary**: 
  - [Summarize the Background/Motivation]
  - [Research Questions]
  - [Application Scenario]
  - [Methodology]
  - [Results]
  - [Intellectual Merits and Practical impacts of your project.]
  
   
Note: please insert the screenshot of the answers to your research question by ChatGPT. The methodology that you use to address the research questions must be more innovative than both the current literature and ChatGPT. 

## Table of Contents

- model
- code
- spotlight
- more about the author
- references

### Model
- **Game Environment**:<br>
    A trust game is a social science experiment involving two participants who do not know each other and are isolated. Assume there are two rational participants who do not know each other. One participant, known as the trustor, is given a sum of money that has 100$ and must decide whether to send some or all of it to the other participant. The amount of money the trustor sends will be squared, and then the trustee can send some or all of the amount back to the trustor. Then the people with less money from those with more can take the amount ranging from zero to three fourth with the condition of difference of their money is bigger than 2$, the transferred money will be timed by a factor of two. This will play two rounds. The trustor and the trustee will change their role for the second round. Then accumulate the money for the two rounds to decide who is the winner. In the end, the people with more money at least 5$ compared to the opponent can take the money in his account away, but the people with less money will gain nothing.If they have the same money, they both win what they have.<br>
    The game's goal is to test the trustor's willingness to take a risk and send money to the trustee and the trustee's desire to reciprocate the trust by sending back some of the squared amounts. And then taking back will make the opponents consider the risk of not giving about half the money.<br>
    The game environment is designed to simulate a situation where one must decide whether to trust another person they do not know and cannot communicate with directly. The experiment provides insights into how trust and cooperation operate in various contexts.<br>
**Possible strategies for the trustor**:<br>
"Maximize profit": The trustor can send the maximum amount to the trustee, hoping to receive the most significant return. If the trustee decides to pay less than a fair number, the trustor can take back some of his money and times two.<br>
"Minimize risk": The trustor sends only a small amount of money to the trustee that they got the same amount after the change to minimize the risk of losing money.
"Reciprocity": The trustor sends an amount of money to the trustee that they believe is fair and that the trustee is probably to reciprocate by returning a similar amount.<br>
**Possible strategies for the trustee**:<br>
"Maximize profit": The trustee returns the most significant amount of money to the trustor, then uses the rule of taking money from the people with more money to have more profits.<br>
"Minimize loss": Give precisely the same half amount of money back to the trustor to avoid more losses or the trustor to gain more profits.<br>
"Reciprocity": Consider the money sent by the trustor, and send back a fair amount of money to let them both win.<br>
**Payoff:**<br>
Considering this situation, the payoff of the trust game divides into these situations.<br>
1. All of the players choose to have the maximum profit strategy. This situation will lead to a maximum overall income, which means the trustor gives all money to the trustee and the trustor reserve all cash, then the trustor takes three-fourths of the difference of their money. The second round will be the same. For this situation, they will all get 15000$+2500$=17500$.<br> 
2. One of the players decides to maximize its profits. If this player is the trustee for the first round, he will work with the trustor to have a 15000$ for the first round. For the second round, he will give 0$ to the trustee, such that the opponent will gain nothing and this guy will have the most money.<br>
3. None of the players decide to work together. They will keep all the money, and after two rounds, they will get 175$.
4. The trustor and the trustee use a certain number of transfers that they think are reasonable. The payoff of this will be between 175$ to 17500$.<br>
- **Solution Concept**:<br>
Based on the backward induction, we will analyze what will happen.<br>
**Second round:**<br>
For the part of taking money away from people with more money, the best choice is to take 3/4 of the difference of their money. Therefore, it is essential to have the chance to take money from whoever has more money after the trustee pays back the money since the gain can be doubled. To win the game, the people with less money have two choices: one is to take a precise amount of money to make them have the same amount, and the other is to take as much as this guy can.<br>
Therefore, the best choice of the trustee is to send all money to the trustor, such that the trustee has the chance to take away the money from the trustor. Or, to avoid the risk of losing, the trustee can take the money away such that the difference between them is lower than 2$, which will cause a win-win situation.<br>
Then for the first step of the second round, the trustor who used to be the trustee in the previous round can send the same number of money to make sure they have a win-win situation, or he can send less money to the trustee, such that the money amount of the trustee can not win the game. <br>
Then we will analyze what the first round will happen.<br>
**First round**:<br>
Considering the taking away progress of the first round, it is the wisest idea to take 3/4 of the differences in money. Or take less to make their difference less than 5$.<br>
Then for the payback progress, to show win the most benefit, the trustee should send all money back, to have the chance of taking away money, but to show fairness and sincerity, the trustee can also make their difference less than 2$.<br>
Considering the giving progress of the first round, the trustor can give all money to a trustee to have a higher total benefit. But if considering the chance of loss due to the second round, the trustor can give nothing to the trustee, such that both of them can win 175$ at the end instead of one of them having nothing.<br>
- Evaluations: e.g. efficiency and fairness

### Code
- Game Environment
- Strategic plays
- Equilibruim Evaluations: e.g. belief, strategy, and payoffs
- oTree Experimental Code 


### Spotlight
- Posters
- Figures
- Slides
- Presentations
- Review articles
- Media appearance

### More about the Author
- headshot
- self-introduction
- Final reflections 
  - intellectual growth
  - professional growth
  - living a purposeful life

### References

- Literature References in [Chicago Author-Date](https://www.chicagomanualofstyle.org/tools_citationguide/citation-guide-2.html) Style and [BibTex](https://scholar.google.com/) 

Levin, Dan, and Luyao Zhang. 2020. “Bridging Level-K to Nash Equilibrium.” *The Review of Economics and Statistics* 104 (6): 1329–40. https://doi.org/10.1162/rest_a_00990.

```
@article{levin2022bridging,
  title={Bridging level-k to nash equilibrium},
  author={Levin, Dan and Zhang, Luyao},
  journal={Review of Economics and Statistics},
  volume={104},
  number={6},
  pages={1329--1340},
  year={2022},
  publisher={MIT Press One Rogers Street, Cambridge, MA 02142-1209, USA journals-info~…}
}
```

