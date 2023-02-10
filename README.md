# ML-Robustness-Membership-inference
The solution identify the robustness of ML model towards Membership inference attack which target to extract information about training data

## Product Overview
Membership inference attacks (MIA) can be staged just by observing the output of the model while having access to some datapoints of training data. MIA attack is a blackbox attack and does not need access to model's parameters. Such ML attacks can result in severe losses and cause security concerns, especially when the training data possess sensitive and/or private information of individuals. This solution builds another ML model to infer training dataset, often called attack model, based on prediction probabilities of target model (the model for which the robustness towards MIA to be calculated)

## Product Highlight 

* Membership inference attack triggers inference to the target model with training data and subject data. Subject dataset is supposed to have similar statistical properties of training data. Subject data helps to build attack model that tries to infer if the given data subject is part of the training dataset on which original target model is built. This solution measures robustness of ML models towards MIA attacks and provides insights about ease of inferring if the data subject is part of training? and how difficult is it to build an attack model that has better ability to attack?  
* This solution requires target model (pickle file), training data and 'subject data' (of same size as training dataset) for building attack model.  The solution accepts scikit-learn Randomforest, decision tress, adaboost and gradient boosting classifier as target model and train three attack models (pytorch neural network, random forest and gradient boosting) to measure robustness of the target model by using different proportions of training data. Attack efficiencies are observed and tabulated with varying proportions of availability of training datasets.  
* PACE - ML is Mphasis Framework and Methodology for end-to-end machine learning development and deployment. PACE-ML enables organizations to improve the quality & reliability of the machine learning solutions in production and helps automate, scale, and monitor them. Need customized Machine Learning and Deep Learning solutions? Get in touch!

## Amazon Marketplace Link
The product can be found [here](https://aws.amazon.com/marketplace/pp/prodview-x7xwuxwm5hiqa).

