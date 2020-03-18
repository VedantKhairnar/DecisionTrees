# DecisionTrees

<div align="center">
<img src="https://img.shields.io/github/license/VedantKhairnar/DecisionTrees">	
<img src="https://img.shields.io/github/stars/VedantKhairnar/DecisionTrees">
<img src="https://img.shields.io/github/forks/VedantKhairnar/DecisionTrees">
<img src="https://img.shields.io/github/issues/VedantKhairnar/DecisionTrees">
<img src="https://img.shields.io/badge/PRs-welcome-informational">
</div>


> “When your values are clear to you, making decisions become easier.”
>  — Roy E. Disney


A decision tree is a decision support tool that uses a tree-like graph or model of decisions and their possible consequences, including chance event outcomes, resource costs, and utility. It is one way to display an algorithm that only contains conditional control statements.

In simple words, it is a flowchart-like structure in which each internal node represents a “test” on an attribute (e.g. whether a coin flip comes up heads or tails), each branch represents the outcome of the test, and each leaf node represents a class label (decision taken after computing all attributes). The paths from root to leaf represent classification rules.

<p align="center">
  <img width="590" height="491" src="https://github.com/VedantKhairnar/DecisionTrees/blob/master/img/dtree.png">
</p>

Tree based learning algorithms are considered to be one of the best and mostly used supervised learning methods. Tree based methods empower predictive models with high accuracy, stability and ease of interpretation. Unlike linear models, they map non-linear relationships quite well. They are adaptable at solving any kind of problem at hand (classification or regression). Decision Tree algorithms are referred to as CART (Classification and Regression Trees).

For detailed theoretical explanation, click [here](https://medium.com/greyatom/decision-trees-a-simple-way-to-visualize-a-decision-dc506a403aeb)

## Part 1) From Scratch
        
  ### 2 Applications : 
        
       
        All examples do the following steps:
        1. Load training data
        2. Let the decision tree grow
        3. Plot the decision tree
        4. classify without missing data
        5. Classifiy with missing data
        (6.) Prune the decision tree according to a minimal gain level
        (7.) Plot the pruned tree
        
   #### 1.a) Determine the disease as Pneumonia and Tuberculosis based on given impurity report of patient.
   
   ##### Output:
   
   
        Column 4 == blubbernd?
        yes -> Lungenentzuendung: 4
        no  -> Column 2 == Punkt?
                        yes -> Column 0 == ohne?
                                        yes -> Tuberkulose: 1
                                        no  -> Lungenentzuendung: 1
                        no  -> Tuberkulose: 4
        {'Tuberkulose': 4}
        {'Tuberkulose': 3.3000000000000003, 'Lungenentzuendung': 0.1}

   ![snap](https://github.com/VedantKhairnar/DecisionTrees/blob/master/DecisionTrees/from_scratch/tbc.png)
        
 ####  1.b) Classify the flower into type of Iris flower (virginica, versicolor and setosa)based on Sepal Length, Sepal Width, Petal Length, Petal Width using the fishiris dataset.
   
   ##### Output: 
        A branch was pruned: gain = 0.146094
        PetalLength >= 3?
        yes -> PetalWidth >= 1.8?
                        yes -> PetalLength >= 4.9?
                                        yes -> virginica: 43
                                        no  -> SepalLength >= 6?
                                                        yes -> virginica: 2
                                                        no  -> versicolor: 1
                        no  -> PetalLength >= 5?
                                        yes -> PetalWidth >= 1.6?
                                                        yes -> SepalLength >= 7.2?
                                                                        yes -> virginica: 1
                                                                        no  -> versicolor: 2
                                                        no  -> virginica: 3
                                        no  -> versicolor: 47, virginica: 1
        no  -> setosa: 50
        
        {'virginica': 3}
        {'virginica': 0.5315890699277861, 'versicolor': 21.039735820299743, 'setosa': 26.218383713756943}
        
![snap](https://github.com/VedantKhairnar/DecisionTrees/blob/master/DecisionTrees/from_scratch/iris.png)
        
## Part 2) Using scikit-learn python library
   ###     Application:  
   #### Ensemble Learning : Predict whether a person be employed on the basis of Previous employment, Internship, Years of Experience and Level of Education.
   
    
    Using  a random forest of 10 decision trees to predict employment of specific candidate profiles
   
   ##### Output:
![snap](https://github.com/VedantKhairnar/DecisionTrees/blob/master/DecisionTrees/using_sklearn/pastHires.png)

   Nt: Code explained in the .py and .pynb file of the respective subdirectories.


## Complexity Analysis: 

In general, the run time cost to construct a balanced binary tree is O(n_{samples}n_{features}\log(n_{samples})) and query time O(\log(n_{samples})) .

Although the tree construction algorithm attempts to generate balanced trees, they will not always be balanced. Assuming that the subtrees remain approximately balanced, the cost at each node consists of searching through O(n_{features}) to find the feature that offers the largest reduction in entropy. 

This has a cost of O(n_{features}n_{samples}\log(n_{samples})) at each node, leading to a total cost over the entire trees (by summing the cost at each node) of O(n_{features}n_{samples}^{2}\log(n_{samples})) .


#### Incase of any queries, connect me at :
[Vedant Khairnar](http://vedantkhairnar.ml/)
