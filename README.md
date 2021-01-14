# KhedekarN-Online-Social-Network-Analysis-Project--Fairness-in-Recommender-System
Recommendation Systems are one of the most important applications in machine learning which provides many services to give relevant suggestions to the users and match them to products and information. Fairness in the recommendation system is essential to make sure there are no unbalanced recommendations. When a user has rated 8 Indian restaurants and 2 Italian restaurants, it is more likely that that the user will be a personalized list of restaurant recommendations where 80% are Indian restaurants and 20% are Italian restaurants. The recommendations will comprise of all his preferences in specific percentages without ignoring the least rated ones and hence leading to balanced recommendations. This is called calibration. Calibration has recently received renewed attention in the context of fairness in machine learning. In Calibration based on the user’s history, the areas of interest are taken into consideration with their corresponding proportions. Calibration is used to improve the accuracy of the recommendations. The outline metrics and re-ranking algorithms are simple yet effective and are used to post-process the output of the recommendation systems.

Project description: The project goal is to achieve fairness for objects in the recommender system.  we will implement similar methods in calibrated recommendations[1] as post-processing, but use different recommender approaches and datasets.

Introduction of fairness in recommendation:
Recommender system is very essential for today’s online purchase websites. While many researchers are trying to promote the accuracy of the recommender system, some researchers find a new research direction of RS: fairness in recommendation. 

Fairness in recommendation can be divided into many categories. Three categories: fairness for subjects, fairness for objects, and multi-stakeholder recommendation.

Fairness for subjects: 
Consider a recommender system suggesting job opportunities to job seekers. An operator of such a system might wish, for example, to ensure that male and female users with similar qualifications get recommendations of jobs with similar rank and salary. The system would therefore need to defend against biases in recommendation output, even biases that might arise entirely due to behavioral differences: for example, male users might be more likely to click optimistically on high-paying jobs.

Fairness for objects: 
Calibrated recommendation: a user has played 70 romance and 30 action movies in the offline training data: our objective is to generate a list of, say, 10 recommended movies such that we maximize the probability of predicting the test movies of this user. The result is if we use a recommender list, most of the movies in that list will be romance movies.

Popularity bias: popular items are being recommended too frequently while the majority of other items do not get the deserved attention.
  

Multi-stakeholder recommendation: For example, at the same time that the system is ensuring that male and female users to get recommendations with similar salary distributions, it might also need to ensure that jobs at minority-owned businesses are being recommended to the most desirable job candidates at the same rate as jobs at white-owned businesses.

Calibrated recommendation:
Calibrated recommendations[1] proposed a post-processing procedure to get similar distributions over genres.
Distributions over genres of use’s history and recommended list:
  
To get the similarity between these two distributions, we use Kullback-Leibler divergence (or Jensen-Shannon Divergence):
 
To determine the recommendation list I:
 
Overview of project workflow: 
Step 1: Get the dataset provided as below, extract useful attributes (userID, itemID, rating, item category) of the data and do preprocessing. Get the number of unique users, items and item categories.
Step 2: Get a ranked list for each user using basic approaches such as CF or SVD++. 
Step 3: Implement the re-rank approach introduced above on the rank list of the previous step. 
Step 4: Use different hyper parameters and compare the results. Report what you find from the results.   
Dataset for this project: 
http://liu.cs.uic.edu/download/yelp_filter/ 
password: y4Filter

Yelp restaurant dataset: contains yelp restaurant ratings, reviewer information and restaurant information.

