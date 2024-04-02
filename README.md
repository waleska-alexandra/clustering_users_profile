# Users Segmentation in Python

The objective is to perform a cluster analysis to segment users according to their profiles on the platform.

The variables are:
- User ID: Unique identifier for each user.
- Age: Age range of the user.
- Gender: Gender of the user.
- Location: User’s location type (Urban, Suburban, Rural).
- Language: Primary language of the user.
- Education Level: Highest education level achieved.
- Likes and Reactions: Number of likes and reactions a user has made.
- Followed Accounts: Number of accounts a user follows.
- Device Usage: Primary device used for accessing the platform (Mobile, Desktop, Tablet).
- Time Spent Online (hrs/weekday): Average hours spent online on weekdays.
- Time Spent Online (hrs/weekend): Average hours spent online on weekends.
- Click-Through Rates (CTR): The percentage of ad impressions that lead to clicks.
- Conversion Rates: The percentage of clicks that lead to conversions/actions.
- Ad Interaction Time (sec): Average time spent interacting with ads in seconds.
- Income Level: User’s income level.
- Top Interests: Primary interests of the user.


### Exploratory Data Analysis

#### Demographic Variables

![image](https://github.com/waleska-alexandra/clustering_users_profile/assets/76563412/393c3727-92d0-44bb-9fce-ab896c6a94a6)


Understanding the demographic distribution of the variables is key to identify clusters and make better user segmentations.
For example, most of the users are between 25 and 34 years old. Although the gender gap is not as wide, women outnumber men. As might be expected, there are more urban users than suburban and rural users, although there are undoubtedly many users from rural areas. The most spoken language is English followed by Spanish.
In terms of education level, a large number have some technical degree, followed by master's and high school. Finally, income level has the highest volume of data in the $100k+ range.


#### If we want to know which device they use, we can see that most of them connect from the computer or from the phone

![image](https://github.com/waleska-alexandra/clustering_users_profile/assets/76563412/38657665-9fc5-4ade-8d04-f94307a94637)


#### The marketing insights are:

![image](https://github.com/waleska-alexandra/clustering_users_profile/assets/76563412/1d08868b-243d-4dfd-92b8-8530002301dc)


#### The most popular interest between users is: Digital Marketing.

![image](https://github.com/waleska-alexandra/clustering_users_profile/assets/76563412/ec28ec20-a6ac-4e47-9599-25af4c8d1fdb)



### Segmentation

What type of segmentation can be done?
Demographic, according to the behavior in the application, or aligned to interests.
To obtain a result, the clustering technique of the sklearn library will be applied.

#### Dendogram

We can see four groups.
![image](https://github.com/waleska-alexandra/clustering_users_profile/assets/76563412/0baafebe-05b2-4f3c-a3bc-e206d26a1145)

After some calculations we have the following results:

- Cluster 0 - "Weekend Fan": These are users who are very active on weekends. They have moderate tastes and reactions. Mostly women, between 25-34 years old. Their income level is between 80k - 100k. They live in urban areas and their educational level is high school.

- Cluster 1 - "Balanced professionals": Their online activity is balanced, with many likes and reactions. Mostly female, aged 25-34. They are located in suburban areas, and have technical professions. Their income is between 20k - 40k.

- Cluster 2 - "Active Explorers / Low Budget": These users have moderate to high activity on weekends. But they have a large number of likes and reactions. Mostly male. from rural areas, with technical professions, but with an income between 0-20k. Their ages are between 25-34 years old.

- Cluster 3 - "Low Profile Professionals": They are users committed to their weekly work, so their main activity is on weekends. Although they tend to be low profile, as they are the least likely to "like" or react to publications. It is noticeable that they only enter the application to review content. They are mostly women, from urban areas, with a master's degree and income between 80k-100k. Their age is between 55-64 years old.

- Cluster 4 - "Reacts to everything": Users with predominant activity on weekends. They are the ones who react the most and give likes to publications. Mostly men, between 55-64 years old, from suburban areas and their educational level is high school. Their income is between 20k - 40k.


Finally the next chart  and the analytical situation are useful for marketers to understand the behaviour of different user segments and tailor their advertising campaigns efficiently. For example, a well-crafted campaign would be targeted only on weekends for weekends fans, who are the most active on those days. While balanced professionals might respond better to weekday campaigns.

![newplot](https://github.com/waleska-alexandra/clustering_users_profile/assets/76563412/5c5e140d-edf4-4eaf-996d-dadbd0c99f97)


Thank you for staying here. You can follow me on my social networks:

![Waleska_Rangel](https://github.com/waleska-alexandra/clustering_users_profile/assets/76563412/72f0e46a-4369-431b-8c42-84b4252e8b94)

