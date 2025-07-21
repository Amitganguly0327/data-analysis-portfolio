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

### AI Hallucinations in Legal Matters
  - Context: I applied advanced techniques in text analysis to check whether any model has caused their attorneys to face an outcome more often than other models.
  - Data: [Damien Charlotin’s AI Hallucination Cases database](https://www.damiencharlotin.com/hallucinations/) 
  - Methodology: I used gensim's LDA topic modeling to identify leading outcomes for attorneys caught for unverified AI use, then openai for automatically classifying outcomes into the leading outcomes, finally creating a bar graph of the leading outcomes grouped by AI models for a sample of rows. I also used pyLDAvis for creating an interactive dashboard for the gensim output.    
  - Results: Based on the resulting graph, it seems Claude is especially associated with sanctions while other models are fairly equally associated with other kinds of leading outcomes.
  - Conclusion: Since the data on AI models and associated outcomes was highly limited (only 2 rows could be sampled for some AI models), it is difficult to tell if any model caused their attorneys to face an outcome more often than other models.
  - Potential areas for improvement: I should further search for data sources with a higher represented of identified AI models. I should also use statistical analysis to ensure that any model caused their attorneys to face an outcome more often than other models.

