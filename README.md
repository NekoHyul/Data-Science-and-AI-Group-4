# Data-Science-and-AI-Group-4

# ADDRESSING FOOD LOSS ACROSS THE PHILIPPINE AGRICULTURE

*A Course Requirement for the Subject Data Science and Artificial Intelligence*

Submitted by: Almirol, John Loyd
              Alviar, Irvin Ace
              De Silva, Jelyn P.
              Micua, Mark Olsen

Submitted to: Labastilla, Aisa M.

Date: January 4, 2024

# Introduction / Problem Statement
  In developing nations such as the Philippines, food loss takes place prior to consumption, posing a growing concern for Filipino farmers and posing threats to both food security and agricultural sustainability.  
According to [1], various factors contribute to food loss and waste throughout the entire food supply chain, including preharvest, harvesting, post-harvest, storage, distribution, retail, and consumption. The primary factor behind food loss is the challenges faced by small-scale farmers in implementing effective postharvest handling, encompassing the provision of storage facilities, infrastructure, cooling chains, packaging, and marketing systems. These challenges, combined with the country's climatic conditions, create an environment conducive to spoilage and diseases, leading to significant quantities of food losses. In the Philippines, being a tropical nation, valuable crops like fruits and vegetables are susceptible to factors such as early ripening due to the inherent high temperature and relative humidity prevalent in the environment. 
In line with the food losses, last January 2020, the Philippines faced a disaster triggered by the eruption of the Taal Volcano, resulting in agricultural losses totaling P3.06 billion. Crops such as coffee, cacao, rice, coconut, and others were adversely affected. Furthermore, the fisheries sector around Taal Lake suffered the most substantial setback, incurring a loss of P1.6 billion. Subsequently, last February 2020, the country grappled with the introduction of African swine fever (ASF), leading to a total loss of P56 billion due to this animal disease. The ASF outbreak resulted in the culling of approximately 350,000 pigs. Given its tropical climate, the Philippines is accustomed to facing numerous typhoons annually. The Department of Agriculture (DA) reported an estimated loss of 322,041 metric tons of unmilled rice due to the typhoons, equivalent to eight days of rice consumption [2].
The adverse effects of this on the country's agricultural sector are profound and varied, necessitating the development of a comprehensive strategy to address this critical issue. These alarming concerns prompted researchers to devise a solution through the training and evaluation of gathered data. Aligned with the United Nations' Sustainable Development Goals (SDGs), this initiative primarily targets SDG 2: Zero Hunger. By addressing food loss at its source, the group strives to contribute to the overarching global effort to eliminate hunger and ensure food security. As the group begins the training and assessment processes, their dedication to attaining SDG 2 becomes a driving principle, guiding the development of pragmatic solutions based on data-driven insights.

  
# Review of Related Literature
  Describe here the technical know how that you learned and researched related to your problem
  
# Gathered Data / Dataset 
 
 The dataset that was chosen by the group is World Food Production by Rafsun Ahmad. This dataset offers extensive details regarding the overall production of different food types in each country spanning the years 1961 to 2023. The author provided some key insights from the dataset which will helped the group in identifying the problem and some of the possible solutions with its corresponding specifications. This includes: 
 
•	Observing Trends Across Time:
Over the years, there has been a general upward trend in the global production of most food items. As an illustration, maize production has experienced substantial growth, increasing from approximately 1.32 billion tonnes in 1961 to nearly 7.97 billion tonnes in 2021.
•	Identifying Primary Producers in the Latest Year:
The dataset pinpoints the countries that held the top production positions for each food item in the most recent year available, which is 2021. For instance, the leading producer of maize may differ from the leading producer of wheat, highlighting the variability in top producers across different food items.
•	Analyzing Disparities in the Latest Year:
In the most recent year (2021), there were significant disparities in the total production volumes of various food items. Certain items such as rice, wheat, and maize exhibited considerably higher production levels compared to others like avocados or tea, emphasizing the diverse magnitudes of production within the same timeframe.
•	Exploring Correlations:
The correlation matrix within the dataset unveils relationships between production volumes of distinct food items. For instance, a robust correlation might exist between yams and cocoa bean production, indicating that nations excelling in yam production also tend to excel in cocoa bean production. This underscores interconnections in the agricultural output of different food categories.

Type of dataset:
Categorized as a longitudinal dataset, this data compilation spans an extensive timeframe from 1961 to 2023. The longitudinal design facilitates the exploration of patterns and shifts in food production over the years, offering valuable insights into the development of agricultural practices.
	
Size of the dataset:
The dataset is diverse, including details about the production of numerous food varieties. Considering its coverage from 1961 to 2023, it is anticipated to be extensive, containing a significant number of data entries. The dataset's magnitude may fluctuate depending on factors such as the number of countries covered, the frequency of data collection (e.g., annually), and the level of detail in production measurements.

Repositories of the dataset:
The dataset is likely to obtain its information from various repositories, including global agricultural organizations, national agricultural agencies, and international databases.
There is a possibility that the dataset includes data sourced from online databases and agricultural publications. Valuable information from repositories hosting agricultural statistics and research findings may contribute to the compilation and periodic updates of this dataset.
Lastly, given its global coverage, the dataset is likely to integrate agricultural records specific to individual countries. This integration may entail collaboration with the agricultural agencies or ministries of each country, ensuring a detailed and country-specific representation of food production.

Link of the dataset:
The dataset was able to be obtained through the suggested website that mostly consists of datasets known as Kaggle. Kaggle functions as a hub and resource for individuals in the fields of data science, machine learning, and research. It offers an extensive collection of datasets spanning various subjects, allowing users to acquire and download datasets to hone their skills and create machine learning models.
With that, the link of the dataset from the aforementioned website is: https://www.kaggle.com/datasets/rafsunahmad/world-food-production/data 

  
# Objectives

The main objective of this project is to analyze and evaluate datasets in addressing food loss across the Philippine agriculture. Specifically, this study aims: 
1.	To identify the problem and to gather dataset based on the problem.
2.	To analyze the dataset for evaluating and training purposes, while exploring and identifying compatible models based on the dataset.
3.	To develop regression models using:
3.1. Linear Regression
3.2. Logistic Regression
4.	To formulate solutions for mitigating food loss in Philippine agriculture using insights from dataset analysis and regression models

  
# Conceptual


  ![Picture1](https://github.com/NekoHyul/Data-Science-and-AI-Group-4/assets/147147734/9fcd17f9-9ade-435a-9d9b-9ed3d4f53393)

  In the pursuit of gaining comprehensive insights into the trends and patterns of agricultural production in the Philippines, a systematic data manipulation and analysis process has been devised. The flowchart encapsulates a series of steps aimed at preparing, visualizing, and modeling agricultural data to achieve the overarching objective of understanding and predicting production rates for maize, rice, and livestock.
First is to address missing values within the dataset by identifying them and subsequently handling them, through imputation or removal.
Once the missing values are addressed, the next step involves isolating relevant data pertaining to the Philippines. This would require filtering the dataset to focus solely on information related to the Philippines, laying the groundwork for a more targeted analysis of agricultural production trends within the country.
Following data cleaning and isolation, the creation of scatter plots to visualize the production rates of maize, rice, and livestock over the years. Visualization is crucial for gaining preliminary insights into potential patterns and trends that could inform subsequent analyses.
Moving forward, the data needs to be prepared for machine learning tasks. This involves splitting the dataset into training and testing sets using techniques like the train_test_split function. Each agricultural product—maize, rice, and livestock—requires a specific dataset containing relevant features (such as 'Year') and corresponding target variables (production rates) for model training.
The next phase involves selecting appropriate machine learning models, such as linear regression for production rate prediction and logistic regression for classification tasks. These models will be trained on the training datasets, and their performance will be evaluated using various metrics like Mean Absolute Error (MAE), Mean Squared Error (MSE), accuracy, precision, recall, and F1 score.
Moreover, the introduction of a classification threshold is suggested as a step for categorizing production rates into high or low categories. This additional layer of analysis enhances the interpretability of the models and contributes to informed decision-making based on classification outcomes.


# Data and Results
In this Capstone Project, the group, consisting of John Loyd Almirol, Irvin Ace Alviar, Jelyn De Silva, and Mark Olsen Micua, embarked on the task of constructing predictive models for world food production. The chosen techniques included linear regression, logistic regression, and deep learning. The initial phase involved the exploration and preprocessing of the dataset, which was acquired from Kaggle and detailed information about global food production. Using libraries such as NumPy, Pandas, Matplotlib, and Seaborn, the students loaded the data into a Jupyter Notebook, conducted an initial check for missing values, and handled them by filling with zeros.

Descriptive statistics and visualizations were then employed to understand the distribution of data, with specific attention given to the production rates of Maize, Rice, and Livestock in the Philippines over the years. Notably, the dataset was processed using linear and logistic regression models rather than more advanced machine learning methods, as the students found the nature of the dataset to be better suited to these classical statistical techniques.

Moving into the predictive modeling phase, linear regression models were implemented to predict production rates for Maize, Rice, and Livestock based on the 'Year.' Despite encountering relatively high errors, especially in predicting Maize and Rice production rates, the model for Livestock production demonstrated comparatively lower errors. Subsequently, logistic regression models were employed for classification tasks, distinguishing between high and low production based on predefined thresholds. The logistic regression models exhibited high accuracy and precision, indicating success in classifying production levels. However, perfect recall in all models hinted at potential bias towards predicting the majority class.

As the students shared their insights, it became clear that the choice of linear and logistic regression over more complex machine learning models was intentional. They highlighted that the dataset's characteristics, presumably with a relatively simple structure, made these classical statistical techniques more suitable for the given task. The students concluded by offering recommendations for future improvements, suggesting exploration into feature engineering, hyperparameter tuning, and investigation of biases in the dataset, while also leaving room for the potential integration of advanced modeling methods for more complex patterns in the data.

  
# Conclusion
In summarizing the Capstone Project, the group of students set out to construct predictive models that could provide valuable insights into the complex dynamics of global food production. Employing various techniques, including linear regression, logistic regression, and deep learning, their exploration commenced with the acquisition of a comprehensive dataset from Kaggle, offering detailed information on global food production dynamics.

In the initial phases, the students meticulously analyzed and organized the dataset. Utilizing tools such as NumPy, Pandas, and visualization libraries, they prepared the data by addressing missing values and focused on understanding the production rates of Maize, Rice, and Livestock in the Philippines.

Transitioning into the modeling phase, the students implemented linear regression models to predict production rates, encountering challenges, especially with Maize and Rice predictions, but gaining valuable insights, particularly in the context of Livestock production. Logistic regression models were then employed to effectively classify production levels, exhibiting high accuracy and precision.

The deliberate selection of classical statistical techniques over more intricate models was a strategic decision made by the group of students. This choice was underpinned by a recognition of the apparent simplicity inherent in the dataset. In essence, the students opted for methods like linear regression and logistic regression as they believed these traditional statistical approaches were better suited to capture the underlying patterns within the dataset.

In conclusion, the Capstone Project not only deepened the group's understanding of global food production trends but also laid the groundwork for future explorations and improvements in predictive modeling methodologies. The process has been about uncovering insights and recognizing the potential for continued growth and refinement in the realm of food production analysis.


# Program Codes / Google colab / Jupyter notebook or spyder IDE
Directly access the Jupyter notebook: CAPSTONE_Jupyter Code_Group 4.ipynb
