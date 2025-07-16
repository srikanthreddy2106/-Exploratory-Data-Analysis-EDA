# -Exploratory-Data-Analysis-EDA

Exploratory Data Analysis (EDA) is an essential step in the data science process, allowing analysts to understand the structure, distribution, and relationships within a dataset. In this analysis, we explore a sample of the Titanic dataset comprising 20 records. The dataset contains various features related to passengers, such as demographic details, travel class, fare, and survival status. The objective of this EDA is to derive meaningful insights using summary statistics and visualizations and to understand patterns that may influence survival outcomes.

Dataset Overview The dataset includes 12 features: PassengerId, Survived, Pclass, Name, Gender, Age, SibSp, Parch, Ticket, Fare, Cabin, and Embarked. Among these, Survived is the target variable indicating whether a passenger survived (1) or not (0). Pclass represents the ticket class (1st, 2nd, or 3rd), while Age, SibSp, Parch, and Fare are numerical features. Other fields such as Name, Ticket, Cabin, and Embarked are either textual or categorical.

Summary Statistics Using pandas.describe(), we obtain central tendencies and dispersion metrics for numerical features. The average age is around 28 years, with a minimum of 2 and a maximum of 58. The fare ranges from 7.22 to 71.28, with an average of 22.19. Most passengers in this sample belong to the 3rd class, and about half survived, indicating a balanced sample in terms of survival outcome. The dataset contains missing values in the Age and Cabin fields, which is common in Titanic datasets and needs to be addressed in further analysis or modeling.

Visual Analysis To understand the distribution and relationships of features, we utilized visualizations using Seaborn and Matplotlib.

Histograms: The age histogram shows a spread between young children and middle-aged adults, suggesting a diverse passenger demographic. The fare histogram is right-skewed, indicating most passengers paid low fares, while a few paid very high prices. The passenger class count shows a higher frequency in 3rd class, representing lower economic status.

Boxplots: Comparing age and survival status, we notice a slight concentration of survivors in the younger age groups, hinting that children might have had a higher survival chance. The fare boxplot by class clearly demonstrates that 1st class passengers paid significantly more than those in lower classes, with a few outliers in higher fare ranges.

Pairplot: A pairplot of numerical features (Age, Fare, SibSp, Parch) colored by survival status reveals some patterns. Survivors tend to pay higher fares and have fewer siblings or parents aboard, indicating a possible link between economic status and survival.

Correlation Matrix: The heatmap shows a strong negative correlation between Pclass and Fare, as expected—higher class passengers paid more. There's a weak positive correlation between Fare and Survived, reinforcing the hypothesis that wealthier passengers had better chances of survival.

Conclusion This EDA on the Titanic dataset sample reveals important insights into how passenger class, fare, and age relate to survival outcomes. Although the dataset is limited in size, the patterns observed align with historical records of the Titanic disaster, where higher-class passengers and younger individuals had better survival rates. These insights are valuable for feature selection and model building in future predictive analyses.
