# Welcome to Team 1's Read Me!

Team 1's repo for the Asurion Client project.
Team members: Aleksandra Cvetanovska, Rachel Montgomery, Yahan Yang, Yunfei Lyu


### Prerequisites
To most easily run this code out of the box, the following packages must be installed:
* pandas
* numpy
* scikit-learn
* tensorflow
* matplotlib
* seaborn
* pmdarima

# Quick navigation
[Background](#background)    
[Goals](#goals) 
[Data](#data)  
[Models](#models)  
[Timeline](#timeline)  
[Repo Structure](#repo-structure)  
[Logistics](#project-logistics)  
[Resources](#resources)  

# Background  

The broad vision of this project is to learn and utilize machine learning techniques, using Python packages, in a real world application. 

Our team mission is to use forecasting models with historical data, to accurately predict the weekly iPhone 14 claim volume for March, 2023. Predictions will serve as a guideline for the business on how many iPhone 14s, and of which color and storage size, they need to keep in stock. 

# Goals

Use forecasting models with historical data, to accurately predict the weekly iPhone 14 claim volume for March, 2023. Predictions will serve as a guideline for the business on how many iPhone 14s, and of which color and storage size, they need to keep in stock. 

# Data
In light of the non-disclosure agreement pertaining to this project, it is imperative to note that no factual information shall be shared on our GitHub repository. All pertinent data will be securely stored in the 'team1' directory located on the ACCRE platform. This designated folder encompasses details regarding the segmentation of testing and training data for our machine learning models.


# Models
Our methodology encompasses the development of a regression model to deliver weekly predictions for March volumes. Additionally, we will create a neural network-based forecasting model in Python, leveraging historical data for training and subsequently generating weekly predictions for March volumes.

The assortment of models utilized in our analysis includes:

* Gradient Boosting
* XGBoost
* Neural Network
* Long Short-Term Memory (LSTM)
* Random Forest

We utilized a fixed split point of "2022-12-26" for partitioning our dataset, training on earlier data and testing on later data to emulate real-world scenarios, focusing exclusively on iPhone-related data.

The evaluation metric, weighted mean absolute percentage error (WMAPE), was chosen to assess the model's performance, particularly its ability to predict higher sales values accurately.

Our models were trained on two feature sets to predict iPhone 14 sales overall and for each storage size, with the base feature set consisting of 'claim', 'generation', 'weeks_since_release', 'weeks_monday', 'week_of_month', 'month', 'year', and 'day', and an additional 'phone size' feature for the storage feature set.


# Timeline

Sprint 1: Week of Feb 13 - 19
* Client visit and Q&A
* Create team charter
* Create Github repo
* Set up ACCRE for each team member

Sprint 2: Week of Feb 19- 26
* Data cleaning and validation 
* Exploratory data analysis
* Generate dataset to use for analysis  

Sprint 3: Week of Feb 26- March 5
* Feature engineering 
* Begin building regression and neural net models 

Sprint 4: Week of March 5-March 19
* Client visit and Q&A Mar 6th
* Present findings
* Verify process follows past procedure with company 
* Edit models based on client feedback (future sprints may need to be adjusted based on this)

Spring break: March 11-19

Sprint 5: Week of March 19- March 26
* Finetune models 
* Complete models 
* Begin models for predicting volume based on specific color and storage size 

Sprint 6: Week of March 26- April 2
* Begin creating Web App (Gradio)
* Finish models for predicting volume based on specific color and storage size & finetune model
* Create presentation for client meeting 
* Ensure to show final feature set and class distribution as part of data story (from feedback on presentation #1)

Sprint 7: Week of April 3 - April 9
* Client visit and Q&A Apr 3
* Present findings 
* Receive feedback on progress and adjust tasks if needed 
* Finish Web App & make model adjustments if needed
* If true data for March is available, generate WMAPE value to assess accuracy of models

Sprint 8: Week of April 9 - April 16
* Model Value Assessment by Jesse on Monday, April 10
* Implement new model assessments based on presentation  
* Finish presentation 
* Practice presenting (at least 3 times, once must in be classroom)
* Client presentations in class April 17th
* Share findings

# Project logistics

**Sprint planning**: Thursdays

**Demo**: Mondays

**Data location**: The data is stored in the 'team1' directory located on the ACCRE platform


# Resources 
* **Python usage**: Whirlwind Tour of Python, Jake VanderPlas ([Book](https://learning.oreilly.com/library/view/a-whirlwind-tour/9781492037859/), [Notebooks](https://github.com/jakevdp/WhirlwindTourOfPython))
* **Data science packages in Python**: [Python Data Science Handbook, Jake VanderPlas](https://jakevdp.github.io/PythonDataScienceHandbook/) 
* **HuggingFace**: [Website](https://huggingface.co/transformers/index.html), [Course/Training](https://huggingface.co/course/chapter1), [Inference using pipelines](https://huggingface.co/transformers/task_summary.html), [Fine tuning models](https://huggingface.co/transformers/training.html)
* **fast.ai**: [Course](https://course.fast.ai/), [Quick start](https://docs.fast.ai/quick_start.html)
* **nbdev**: [Overview](https://nbdev.fast.ai/), [Tutorial](https://nbdev.fast.ai/tutorial.html)
* **Git tutorials**: [Simple Guide](https://rogerdudler.github.io/git-guide/), [Learn Git Branching](https://learngitbranching.js.org/?locale=en_US)
* **ACCRE how-to guides**: [DSI How-tos](https://github.com/vanderbilt-data-science/how-tos) 

