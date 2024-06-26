## Neural Network Model Analysis 

Deep learning and neural networks were employed to assess the potential success of applicants seeking funding from Alphabet Soup, a philanthropic organization that has supported over 34,000 initiatives in the past

### Data Processing 
The dataset underwent preprocessing to eliminate irrelevant information, leading to the removal of the EIN and NAME columns from the model. The remaining columns were designated as features for the model, with the NAME column being reintroduced in a subsequent test. Due to high fluctuation, CLASSIFICATION and APPLICATION_TYPE were replaced with 'Other'. The dataset was then split into training and testing sets. The target variable, "IS_SUCCESSFUL," was defined, where a value of 1 represented success and 0 denoted failure. Analysis of application data was conducted, with CLASSIFICATION values used for binning. Each unique value served as a cutoff point to group "rare" categorical variables together under a new value, 'Other'. Subsequent checks were performed to ensure the success of binning. Categorical variables were encoded using 'pd.get_dummies()'.

### Compiling, Training, and Evaluation the Model 
A Neural Network was employed for each model with multiple layers, totaling three layers in all. The number of hidden nodes in each layer was determined by the number of features present in the dataset.
![image](https://github.com/HSaleem352/deep-learning-challenge/assets/60048058/a87d875f-7ebb-46b9-9cb2-da37644b0614)

The training model, consisting of three layers, encompassed a total of 477 parameters. In the initial trial, it achieved a performance of approximately 72%, falling slightly short of the desired 75% threshold.

![image](https://github.com/HSaleem352/deep-learning-challenge/assets/60048058/2a298d86-2e83-41be-b1b9-7bd7615fc618)
![image](https://github.com/HSaleem352/deep-learning-challenge/assets/60048058/080a7347-af49-425f-bedf-2b69aacca524)

### Optimization
In the second iteration, 'NAME' was reintroduced into the dataset, resulting in an improved performance of 79%, exceeding the target by 4%. The model comprised a total of 3,298 parameters.

![image](https://github.com/HSaleem352/deep-learning-challenge/assets/60048058/3c2320dc-636e-4a3f-bff8-ef2207a68688)

Deep learning models benefit from having multiple layers because they enable the machine to effectively filter inputs. Through these layers, the computer learns to predict and classify information.

![image](https://github.com/HSaleem352/deep-learning-challenge/assets/60048058/ebca9dff-3540-4e06-96a4-73ce36541cbf)
