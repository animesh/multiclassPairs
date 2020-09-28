# multiclassPairs
Build single sample pair-based (rule-based) classifiers using top-score pairs or random forest for multi-class problems.

Description: A toolbox to train a single sample classifier that uses in-sample feature relationships. The relationships are represented as feature1 < feature2 (e.g. gene1 < gene2). We provide two options to go with. The first is based on 'switchBox' package which uses Top-score pairs algorithm. Second is a novel implementation based on random forest algorithm. For simple problems, we recommend to use one-vs-rest using TSP option due to its simplicity and for being easy to interpret.  For complex problems, RF performs better.  Both lines filter the features first then combine the filtered features to make the list of all the possible rules (i.e. rule1: feature1 < feature2, rule2: feature1 < feature3, etc...).  Then the list of rules will be filtered and the most important and informative rules will be kept. The informative rules will be assembled in a one-vs-rest model or an RF model.  We provide a detailed description with each function in this package to explain the filtration and training methodology in each line. 
