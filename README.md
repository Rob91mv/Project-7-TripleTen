# Predictive Model for Recommending Smart and Ultra Plans for Megaline
![](https://content.vodafone.co.nz/dims4/default/a532f4d/2147483647/strip/true/crop/3840x640+0+0/resize/4720x786!/format/webp/quality/100/?url=http%3A%2F%2Fvodafonenz-brightspot.s3.amazonaws.com%2F0e%2Fb8%2Fb3ca7c114ae1badc75886388956f%2Focs00307-mobile-plans-1920x320-2x.jpg)

## Project Overview:
The next project consists of the development of a model that can analyse customer behaviour in the use of legacy plans in order to be able to offer them the new Megaline plans: Smart or Ultra.

The objective is to find the best model based on its accuracy (reference: accuracy of more than 0.75), i.e. minimising errors even if that means not detecting all cases.

## Data Dictionary:

| Variable   | Description                                              |
|------------|----------------------------------------------------------|
| calls      | Number of calls made                                     |
| minutes    | Total call duration in minutes                           |
| messages   | Number of text messages sent                             |
| mb_used    | Internet traffic used in megabytes (MB)                  |
| is_ultra   | Current mobile plan: Ultra (1) or Smart (0) (target)     |

## Impact

The project focused on developing a predictive model to analyse customer behaviour and recommend a transition from legacy mobile plans to one of Megaline’s new offerings: Smart or Ultra.

Three models were evaluated for this binary classification task: Decision Tree, Random Forest, and Logistic Regression. A hyperparameter tuning process was conducted for the tree-based models by varying max_depth from 1 to 5. Logistic Regression was included as a baseline model without hyperparameter adjustment.

The best-performing model was the Random Forest classifier with a max_depth of 4, achieving an accuracy of 0.8116 on the validation set. When tested on unseen data, the model maintained solid performance with an accuracy of 0.8087, indicating a slight overfitting but still surpassing the required accuracy threshold. This confirms the model’s reliability and suitability for supporting Megaline’s plan recommendation strategy.

"TripleTen" Project #7
