# Algorithmic-Trading

## Introduction
Dive into the Algorithmic Trading Optimization repository, where machine learning meets trading algorithm fine-tuning. Our ambition? To forge an algorithm superior to its forerunners and meticulously gauge its performance.

## Project Contents
This repository provides:

A main Jupyter notebook, the heart of our machine learning models and trading strategies.
The 'Resources' folder: a treasure trove of plots visualizing trading algorithm outcomes.

## Tasks & Highlights

# 1.Baseline Performance Establishment

* Kickoff with a simple moving average crossover (SMA) trading strategy, enhanced by sklearn's support vector machine (SVM) classifier.
* Visualization: Cumulative Returns Plot 1 for baseline performance insights.

#2. Refinement of Baseline Trading Algorithm

* Initial Setting:
* * Training data endpoint: offset of 3 months
SMA windows: short at 4, long at 100
First Iteration:
Modified training data endpoint: offset of 5 months
Refined SMA windows: short at 2, long at 60
Outcome: After adjusting parameters, strategy returns rose from 1.5 to 1.6, with actual returns jumping from 1.4 to 1.5.
Visualization: Cumulative Returns Plot 2 captures the results post-refinement.
Evaluation of a New Classifier

A leap into the AdaBoost classifier realm.
Outcome: A dip in strategy return to 1.3, indicating an underwhelming performance compared to the baseline.
Visualization: Cumulative Returns Plot 3 offers a view into this classifier's results.
Final Insights

The baseline trading algorithm, post-refinement, displayed pronounced improvements.
Experimentation extended to classifiers such as AdaBoost, DecisionTreeClassifier, LogisticRegression, and GradientBoostingClassifier. However, the enhanced baseline algorithm outperformed consistently.
Visual snapshots (in PNG format) throughout the repository provide a clear comparative view of different strategies' performances.
Disclaimer
This project primarily aims at academic exploration. It shouldn't be perceived as a trading manual for real-world scenarios. The strategies explored might not always mirror real-world trading. Prior to any live trading based on this work, seeking guidance from financial professionals is paramount.
