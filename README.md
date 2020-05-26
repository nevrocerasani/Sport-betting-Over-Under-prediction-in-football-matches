# Sport-betting-Over-Under-prediction-in-football-matches

Have you ever had to rip a sport bet at the 90th minute for an undesired goal? If the answer is yes, you may be interested
in this project.
Basically, what I did is trying to predict whether a football match will end with more than 2.5 goals or less (over/under),
and eventually elaborate a betting strategy.
How I did it: I implemented a Machine Learning algorithm (Logistic Regression) to predict the binary outcome
(0 for under, 1 for over), and a Deep Neural Network to predict the probability associated with it
(initially I assume that if the probability was less than 0.5 we would bet under, and if it was greater than 0.5 we would bet
over).
Based on the results, at the end I modified this strategy a little bit in order to make it less risky (everything is explained
in the project step by step, as well as the features used to make the predictions).
Surprisingly, despite all the several factors that may influence a football match, I obtained an accuracy of 95%.
Further improvements of this project may be, for example, its complete automation by adding an API that automatically adds
the result of each match. By doing so, the algorithm could be able to continuously predict the outcome of the next matches
without the user intervention.


DESCRIPTION OF THE FEATURES USED FOR THE PREDICTIONS:

- HAS (Home Attacking Strenght): 5 periods exponential moving average of the number of the goals scored by the home team
when playing home;
- HDS (Home Defending Strenght): 5 periods exponential moving average of the number of the goals conceded by the home team
when playing home;
- AAS (Away Attacking Strenght): 5 periods exponential moving average of the number of the goals scored by the away team
when playing away;
- ADS (Away Defending Strenght): 5 periods exponential moving average of the number of the goals conceded by the away team
when playing away;
- OH (Over Home): 5 periods exponential moving average of the number of the over/under 2.5 achieved by the home team
when playing home. Example: if in the last 5 home matches a team achieved 3 under and 2 over, the value of OH would be the
exponential moving average of 0,0,0,1,1 (in this order);
- OA (Over Away): 5 periods exponential moving average of the number of the over/under 2.5 achieved by the home team
when playing home.

For any other doubt do not hesitate to contact me!
