# DecisionTrees

<div align="center">
<img src="https://img.shields.io/github/license/VedantKhairnar/DecisionTrees">	
<img src="https://img.shields.io/github/stars/VedantKhairnar/DecisionTrees">
<img src="https://img.shields.io/github/forks/VedantKhairnar/DecisionTrees">
<img src="https://img.shields.io/github/issues/VedantKhairnar/DecisionTrees">
<img src="https://img.shields.io/badge/PRs-welcome-informational">
</div>

A decision tree is a decision support tool that uses a tree-like graph or model of decisions and their possible consequences, including chance event outcomes, resource costs, and utility. It is one way to display an algorithm that only contains conditional control statements.

A decision tree is a flowchart-like structure in which each internal node represents a “test” on an attribute (e.g. whether a coin flip comes up heads or tails), each branch represents the outcome of the test, and each leaf node represents a class label (decision taken after computing all attributes). The paths from root to leaf represent classification rules.

![Snap](https://github.com/VedantKhairnar/DecisionTrees/blob/master/img/dtree.png)


Tree based learning algorithms are considered to be one of the best and mostly used supervised learning methods. Tree based methods empower predictive models with high accuracy, stability and ease of interpretation. Unlike linear models, they map non-linear relationships quite well. They are adaptable at solving any kind of problem at hand (classification or regression). Decision Tree algorithms are referred to as CART (Classification and Regression Trees).

For detail theoretical explanation, click [here](https://medium.com/greyatom/decision-trees-a-simple-way-to-visualize-a-decision-dc506a403aeb)

## Part 1) From Scratch
        
  ### For 2 Applications : 
        
   1.a) Pneumnia Symptoms
        
   1.b) Fishiris dataset : (Flower : SepalLength,SepalWidth,PetalLength,PetalWidth,Name)
        
        All examples do the following steps:
        1. Load training data
        2. Let the decision tree grow
        3. Plot the decision tree
        4. classify without missing data
        5. Classifiy with missing data
        (6.) Prune the decision tree according to a minimal gain level
        (7.) Plot the pruned tree
        
## Part 2) Using scikit-learn python library
   ###     Application:  
   
   Ensemble Learning
    
    Using  a random forest of 10 decision trees to predict employment of specific candidate profiles
   
   Nt: Code explaned in the .py and .pynb file
