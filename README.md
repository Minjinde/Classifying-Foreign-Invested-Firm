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


## Topics from LDA output:

| Topic ID | Dominant Theme                           | Example Keywords                                |
| -------- | ---------------------------------------- | ----------------------------------------------- |
| **0**    | Consulting & Events                      | consulting, information, management, exhibition |
| **1**    | Food & Agriculture                       | food, packaging, real estate, transport         |
| **2**    | Manufacturing (Electronics & Automotive) | manufacture, equipment, components, R&D         |
| **3**    | Retail & Wholesale                       | wholesale, retail, cosmetics, apparel           |
| **4**    | Trade & Regulation                       | regulation, import/export, license              |
| **5**    | Consumer Goods & Fashion                 | clothing, furniture, decoration, toys           |
| **6**    | Chemicals & Technology                   | chemicals, R&D, tech transfer                   |
| **7**    | Enterprise Consulting                    | management, design, planning, investment        |
| **8**    | Brokerage & Auctions                     | acting, commission, auction, molds              |
| **9**    | Regulatory Compliance                    | approval, prohibition, licensing laws           |

