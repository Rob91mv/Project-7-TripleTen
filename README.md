# Predictive Model for Recommending Smart and Ultra Plans for Megaline
![]([600%2C400&ssl=1](https://mobile.everyday.com.au/medias/Banner-EDMobile-HomePage-Jen-3-halfprice-Tablet-768x322.png?context=bWFzdGVyfEV2ZXJ5ZGF5IE1vYmlsZV9Ib21lcGFnZSBNYWluIEltYWdlc3wxNzUwMzl8aW1hZ2UvcG5nfEV2ZXJ5ZGF5IE1vYmlsZV9Ib21lcGFnZSBNYWluIEltYWdlcy9oNjAvaDhkLzg5NTYxMjY1NjAyODYucG5nfDE0YzBiYjg2YzUwMWY3OTljYzJkOTdmMTVkYWJhZDg0NTQwYzhiMzQ1Yzg0YzA5NGRjNThhYTU5MGNiNDY1NjM))

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
