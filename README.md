# L-HSAB Dataset: Context and Topics
The Levantine Hate Speech and ABusive (L-HSAB) is the first Arabic Levantine Hate Speech and Abusive Language Dataset proposed in the 3rd Workshop ALW-2019 co-located with ACL-2019, Florence, Italy.

The volatile political/social atmosphere in Levantine-speaking countries, particularly, Syria and Lebanon, has been always associated with intensive online debates of toxic contents: Hate speech and abusive language.
L-HSAB combines 5,846 Syrian/Lebanese political tweets labeled as normal, abusive or hate. 
Coping with hot political debates, the collected tweets were posted between March 2018 and February 2019.


# Data Collection & Resources

L-HSAB was constructed out of Levantine tweets scraped via Twitter API (Tweepy). We collected the tweets based on multiple queries
formulated from the potential entities that are usually targeted by abusive/hate speech such as “اللاجئين” (refugees), "البنات" (females), “العرب” (Arabs), “الدروز” (Druze), etc. 

Aiming to get pure Syrian/Lebanese tweets rich of toxic contents, some user timelines (verified or having more than 100k followers) which belong to certain politicians, social/political activists and TV anchors, were adopted as data resources. 


# Data Annotation Guidelines
Our annotation process was conducted by 3 Levantine-speaking annotators. The annotation instructions defined the 3 label categories as:

• Normal tweets are those instances with no offensive, aggressive, insulting and profanity content.

• Abusive tweets are those instances that combine offensive, aggressive, insulting or profanity content.

• Hate tweets are those instances that: (a) contain an abusive language, (b) dedicate the abusive language towards a specific person or 
  a group of people and (c) demean or dehumanize that person or that group of people based on their descriptive identity (race, gender, 
  religion, disability, skin color, belief).
 
• The annotators were provided by the nicknames usually used, within hate/abusive contexts, to refer to certain political parties, 
  minorities and ethnic/religion groups. For example, “تيار المستقبل” (Future Movement Party), which represents the Sunnis ethnic 
  group, is usually called by its nickname “تيار المستهبل” (Dumb Party) in hate speech contexts.

# Annotation Evaluation: Methods & Results
The annotation credibility was evaluated using several evaluation measures:

1- Pairwise Percent Agreement Measure (PRAM): best value between annotator 1 & annotator 3 = 87.24%

2- Cohen's Kappa (K): best value between annotator 1 & annotator 3 = 75.8%

3- Krippendorff’s Alpha (α)= 76.5% 

# L-HSAB: Classification Experiments

1- Binary Classification (Normal, Abusive):
   
   Best performance by Naive Bayes with an F-measure of 89.6%
   
2- Multi-Class Classification (Normal, Abusive, Hate):
   
   Best performance by Naive Bayes with an F-measure of 74.4%



# Paper Citation

@inproceedings{mulki2019hsab,
  title={L-HSAB: A Levantine Twitter Dataset for Hate Speech and Abusive Language},
  
  author={Mulki, Hala and Haddad, Hatem and Ali, Chedi Bechikh and Alshabani, Halima},
  
  booktitle={Proceedings of the Third Workshop on Abusive Language Online},
  
  pages={111--118},
  
  year={2019}
  
}
