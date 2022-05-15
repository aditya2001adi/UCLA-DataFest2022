# UCLA DataFest 2022
## Rules and Overview
DataFest @ UCLA is an annual data analysis competition in which college students from schools across Southern California compete as they clean, wrangle, and analyze data from a given dataset. Students are given about 36 hours to come up with any meaningful insights they choose. After this, teams were given presentations among predetermined groups of ~15 teams in front of professors and data scientists working in industry. From this group, 3 teams were selected as finalists to present in front of the larger group, and a final panel of judges.

Presentations were limited to three slides (including one cover slide) and students had 5 minutes to present their findings. If a team was selected as a finalist, they gave the exact same presentation in front of the larger group. 

Of the final 15 teams, judges selected winners and honorable mentions across three categories: Best Use of Statistical Models, Best Insight, and Best Visualization. Two teams were also chosen to receive Judges' Choice awards if their work didn't fit cleanly into any one of the aforementioned categories.

## The Dataset
Students were tasked with analyzing longitudinal data about an educational online game meant to encourage children between the ages 11-14 to engage in safe behaviors, such as abstaining from drugs and alcohol. The data tracked 166 players as they moved through the game, which each move being timestamped and recorded as an observation. The entire dataset consisted of roughly 2.1 million observations and 134 variables. The organizers of DataFest asked that the data be deleted after this competition, so the data is not available in this repository.

## Our Project
My teammate and I were interested in how different players might play the game differently, and because the data didn't have much demographic data regarding the players, we decided that player speed could be an interesting metric of how they played the game. We wanted to know if there were noticeable differences in how certain players played, and what that meant about their outcomes. We used k-means clustering (with k = 3) to cluster the players into three categories: those who played the game quickly, those who played at a moderate pace, and those who played the game slowly. We used metrics such as scanning speed (the rate at which the player moved a magnifying glass across the screen in one portion of the game) and clicks per second (the number of moves a player made per second). Then, we evaluated these clusters' performance based on the number of mistakes they made in the game (for example, if they answered a question incorrectly). 

Using logistic regression, we found that players who played the game quickly were more likely to make more mistakes than the average player. Some of this may be intuitive; students who play more quickly may not engage with the question thoroughly, or may simply be trying to rush through the game. However, it could also be possible that students who play quickly may simply have a better understanding of the game and the questions. Our findings seem to confirm the former; students who played the game quickly were more prone to making more mistakes than the average student. 

After being selected as finalists, my teammate and I were awarded an Honorable Mention for Best Use of Statistical Modeling for our work. 
