# Classifying-Foreign-Invested-Firm

## Data Loading & Cleaning
- Loaded a 590k+ record dataset from Google Drive.

- Dropped nulls (~1.3%).

- Removed repetitive and legal boilerplate text (e.g., "除依法须经批准的项目外...").

 - Normalized punctuation and spaces.

## Preprocessing

- Combined English and Chinese stopword filtering.

- Tokenized Chinese text with Jieba.

- Built a Gensim dictionary of ~56,000 tokens.

## LDA Modeling

- Created a Latent Dirichlet Allocation model with 10 topics using Gensim.

- Extracted interpretable themes like manufacturing, consulting, trading, and licensing.

## Translation

- Used googletrans to translate topic keywords into English for interpretability.
