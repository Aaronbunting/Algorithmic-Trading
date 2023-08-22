# Algorithmic-Trading

Algorithmic Trading Optimization Repository

## Introduction
Welcome to the Algorithmic Trading Optimization repository! Within these digital walls lies a captivating machine learning-based project focused on the fine-tuning of trading algorithms and the subsequent comparison of their performances. The driving force behind this endeavor is to craft an algorithm that transcends its predecessors and, in turn, evaluate its performance.

## Project Essence
This repository houses a collection of Jupyter notebooks, datasets, and resultant plots. Here's an insight into what each file/section entails:

The central Jupyter notebook embodies the core of the machine learning models and trading algorithms.
The 'Resources' folder serves as the vault for plots showcasing diverse trading algorithm performances.
Pioneering Tasks
Within the contours of this project, four primary tasks take the center stage:

## 1. Establishing a Baseline Performance
Our voyage commences with the implementation of a rudimentary moving average crossover (SMA) trading strategy, bolstered by sklearn's support vector machine (SVM) classifier. This initial trading algorithm sets the stage by offering a performance baseline. To capture this essence visually, a cumulative return plot makes its appearance:

## Cumulative Returns Plot 1

2. Refining the Baseline Trading Algorithm
To elevate the baseline algorithm's performance, meticulous steps are undertaken:

* Tweaking the Training Algorithm: The training dataset's dimensions are adjusted. The dataset is segmented across different timeframes, and the notebook is rerun with these new parameters. The outcome is a noticeable enhancement in algorithm performance, with strategy returns rising from 1.5 to 1.6 and actual returns escalating from 1.4 to 1.5.
* Initially, the training data endpoint was set with an offset of 3 months, accompanied by short and long windows for the SMA set at 4 and 100, respectively.
* Setting the training data endpoint with a 3-month offset
* training_end = X.index.min() + DateOffset(months=3)
* Configuring the short and long windows
* short_window = 4 long_window = 100

Following this adjustment, the training data endpoint was shifted with a 5-month offset, while the short and long windows were refined to 2 and 60, respectively.
* Setting the training data endpoint with a 5-month offset training_end = X.index.min() + DateOffset(months=5)
* Fine-tuning the short and long windows short_window = 2 long_window = 60

Fine-tuning the Training Algorithm: The SMA algorithm's windows underwent further refinement. Post adjustment, the notebook was rerun, yielding improved trading algorithm performance.
* After fine-tuning, the parameters that yielded the most substantial boost to trading algorithm returns were retained. A revised cumulative return plot was fashioned:

## Cumulative Returns Plot 2

3. Assessing a Novel Machine Learning Classifier
The next phase witnesses an evaluation of a fresh machine learning classifier - the AdaBoost algorithm. The model is trained using the training data, and its performance is rigorously backtested. The results, however, indicate a subpar performance when compared to baseline models. The strategy return dwindles to 1.3, signifying weaker trading prowess in comparison. Below lies the PNG image encapsulating the cumulative returns plot for this updated trading algorithm:

## Cumulative Returns Plot 3

4. Conclusive Evaluation
Our analysis draws to a close, culminating in a comprehensive evaluation report. Here, we outline our observations and discoveries:

- The meticulous fine-tuning of the baseline trading algorithm, encompassing the adjustment of training dataset size and SMA input features, led to substantial enhancements in algorithmic performance. Strategy returns surged from 1.5 to 1.6, while actual returns escalated from 1.4 to 1.5.

- The exploration extended to include a novel machine learning classifier, encompassing AdaBoost, DecisionTreeClassifier, LogisticRegression, and GradientBoostingClassifier. Across these models, the fine-tuned baseline algorithm consistently showcased superior performance, firmly establishing its trading prowess.

- Within the preceding sections, you will find PNG images unveiling cumulative returns plots for both the baseline and the fine-tuned algorithms. These visual aids seamlessly depict the performance disparity between distinct strategies.

## Disclaimer
It is crucial to acknowledge that this project serves an academic purpose. It should not be misconstrued as a definitive guide for real-world trading. The algorithms and strategies enacted in this project may not align with practical trading scenarios. It is highly recommended to consult financial experts and advisors before translating any findings into live trading actions.
