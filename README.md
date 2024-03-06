# Graph Neural Networks for Twitter Data

This project focuses on link prediction in a Twitter network using Graph Neural Networks (GNNs), specifically GraphSage. Link prediction involves predicting future relationships between nodes in a complex network, such as estimating the likelihood of a link between two Twitter users based on network structure and node attributes.

## Project Overview

### Dataset
The Twitter data is obtained using Tweepy to scrape tweets with the hashtag "#python." The network is constructed by identifying authors and their connections, forming the basis for link prediction.

### Project Roadmap
1. **Scrape Twitter Network:** Utilize Tweepy to retrieve tweets and user connections.
2. **Create Social Graph:** Use NetworkX for data wrangling and visualization to understand the Twitter network structure.
3. **Build GNN Model:** Implement a GraphSage GNN model for link prediction.
4. **Conclusion:** Evaluate the model's performance and draw conclusions.

## Code Sections

### 1. Scraping Twitter Data
The Tweepy library is employed to scrape tweets, authors, and user connections. API keys are used for authentication.

### 2. Creating Social Graph
Data wrangling is performed, and NetworkX is used to create and visualize the Twitter social graph. A subset of the graph is visualized to improve plotting time.

### 3. Building GNN Model
StellarGraph, a library for graph machine learning, is used to create the training and test sets. GraphSage is implemented for link prediction, treating the problem as supervised learning. Fake features are assigned to nodes, and the model is trained for a specified number of epochs.

### 4. Model Evaluation
The model's performance is evaluated using metrics such as accuracy, precision, recall, and F1-score. The training and validation loss curves are also plotted.

## Conclusion
The project demonstrates the construction and testing of a GraphSage GNN model for Twitter link prediction. Despite using fake features, the model achieves 80% accuracy on the test set. The implications include making friendship recommendations on Twitter.

## References
- [Graph Machine Learning](https://github.com/PacktPublishing/Graph-Machine-Learning/blob/main/Chapter06/01_Social_network_analysis.ipynb) by C. Stamile, A. Marzullo, E. Deusebio (2021)
- Martinčić-Ipsˇić S, Močibob E, Perc M (2017). [Link prediction on Twitter](https://doi.org/10.1371/journal.pone.0181079).
- [Obviously.AI](https://www.obviously.ai/post/machine-learning-model-performance) (2022). How To Know if Your Machine Learning Model Has Good Performance.
