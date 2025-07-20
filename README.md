# data-analysis-portfolio

I have compiled my independent data analysis projects to date in this repository. It shows an approximate extent of my knowledge of data analysis. 

Currently, my projects are available as .ipynb files above. Below are key aspects of each project.

I learnt text analysis using Python through the featured tutorials by experts on JSTOR Constellate. I have stored answers to the exercises included in the tutorials, in which I preserved Constellate's comments for guiding learners, and for which I occasionally had to consult online forums for mysterious errors, in this [.ipynb](https://colab.research.google.com/drive/13c7_YY3ehox7xAEWyYjyrLv97OUQpMwN?usp=sharing). Recently, I have added Reflection or Active Recall cells for reinforcing my memory of the practices and underlying concepts related to the problems/solutions. 

## Python:
### Chess Puzzles
  - Context: I applied data analysis, preprocessing, and analysis to check whether the underlying themes are a good determinor of the rating of chess puzzles.
  - Data: Dataset Finder which showed me to Lichess's open database on [database.lichess.org](database.lichess.org). I have downloaded the .csv present [here](https://database.lichess.org/#puzzles).
  - Methodology: I used pandas to handle missing values and group data by theme words. I used matplotlib and seaborn for creating a bar plot that allows visual assessment how well theme words differentiate puzzles of different difficulties.
  - Results: There were about 20 theme words that appeared 1.5 times more frequently in higher-rated puzzles than in lower-rated puzzles.
  - Conclusion: It is plausible that theme words are a good determinor of puzzle difficulty.
  - Potential areas for improvement: I can perform statistical analysis for a more reliable determination of which themes appear significantly more likely in one puzzle group. As an alternative to statistical analysis, I could try predicting puzzle ratings based on their theme words using a LLM and make a decision based on the R-squared value. I should also find other strong determiners of puzzle difficulty rating. 
