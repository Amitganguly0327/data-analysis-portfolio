# data-analysis-portfolio

I have compiled my independent data analysis projects to date in this repository. It shows an approximate extent of my knowledge of data analysis. 

Currently, my projects are available as .ipynb files above. Below are key aspects of each project.

I learnt text analysis using Python through the featured tutorials by experts on JSTOR Constellate. I have stored answers to the exercises included in the tutorials, in which I preserved Constellate's comments for guiding learners, and for which I occasionally had to consult online forums for mysterious errors, in this [.ipynb](https://colab.research.google.com/drive/13c7_YY3ehox7xAEWyYjyrLv97OUQpMwN?usp=sharing). Recently, I have added Reflection or Active Recall cells for reinforcing my memory of the practices and underlying concepts related to the problems/solutions. 

## Python:
### Chess Puzzles
  - **Context:** I applied data analysis, preprocessing, and analysis to check whether there are certain themes more commonly present in puzzles rated >=2000 than in lower-rated ones.
  - **Data:** I used Amelia Wattenberger's [Dataset Finder](https://dataset-finder.netlify.app/) which is based on Jeremy Singer-Vine's [Data Is Plural — Structured Archive](https://docs.google.com/spreadsheets/d/1wZhPLMCHKJvwOkP4juclhjFgqIY8fQFMemwKL2c64vk/edit?usp=sharing) to find Lichess's open database on [database.lichess.org](database.lichess.org). I have downloaded the .csv present [here](https://database.lichess.org/#puzzles). 
  - **Methodology:** I used pandas to handle missing values and group data by theme words. I used matplotlib and seaborn for creating a bar plot that allows visual assessment how well theme words differentiate puzzles of different difficulties.
  - **Results:** There were about 20 theme words that appeared 1.5 times more frequently in higher-rated puzzles than in lower-rated puzzles.
  - **Conclusion:** It is likely the null hypothesis that the frequency distribution of themes in puzzles rated >=2000 is the same as that than in lower-rated ones would be rejected post-statistical analysis.
  - **Potential areas for improvement:** I can perform statistical analysis for a more reliable determination of which themes appear significantly more likely in one puzzle group. As an alternative to statistical analysis, I could try predicting puzzle ratings based on their theme words using a LLM and make a decision based on the R-squared value. I should also find other strong determiners of puzzle difficulty rating.

### AI Hallucinations in Legal Matters
  - **Context:** I applied advanced techniques text analysis including topic modeling, automatic classification using a LLM, and dashboard creation to check whether certain AI tools are more frequently associated with specific attorney outcomes compared to others, in other words, if the distribution of attorney outcomes varies depending on the AI tool employed.
  - **Data:** I found [Damien Charlotin’s AI Hallucination Cases database](https://www.damiencharlotin.com/hallucinations/) using Amelia Wattenberger's [Dataset Finder](https://dataset-finder.netlify.app/) to find Lichess's open database on [database.lichess.org](database.lichess.org) which is based on Jeremy Singer-Vine's [Data Is Plural — Structured Archive](https://docs.google.com/spreadsheets/d/1wZhPLMCHKJvwOkP4juclhjFgqIY8fQFMemwKL2c64vk/edit?usp=sharing).
  - **Methodology:** I used gensim's LDA topic modeling to identify leading outcomes for attorneys caught for unverified AI use, then openai for automatically classifying outcomes into the leading outcomes, finally creating a bar graph of the leading outcomes grouped by AI tools for a sample of rows. I also used pyLDAvis for creating an interactive dashboard for the gensim output.    
  - **Results:** Based on the resulting graph, it seems Claude has a more frequent association with sanctions than other AI tools, while for all other leading outcomes, the distribution of associated AI tools is uniform.
  - **Conclusion:** Since the data on AI tools and associated outcomes was highly limited (only 2 rows could be sampled for some AI tools), it is difficult to tell if any tool caused their attorneys to face an outcome more often than other tools.
  - **Potential areas for improvement:** I should further search for data sources with a higher represented of identified AI tools. I should also use statistical analysis to ensure that any tools caused their attorneys to face an outcome more often than other tools.

