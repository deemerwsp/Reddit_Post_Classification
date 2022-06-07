### Contents:
- [Problem Statement](#Problem-Statement)
- [Executive Summary](#Executive-Summary)
- [Data Dictionary](#Data-Dictionary)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)

### Problem Statement

What characteristics of a post on Reddit are most predictive of the overall interaction on a thread (as measured by number of comments)?

---

### Executive Summary

We collected data from the Reddit home page on "hot" posts. The data we collected included several metadata. The metadata that we ended up using in our models was the title of the post, the subreddit it originated from, the length of time it had been up at the time the data was collected, the number of comments (our target for our models), if the posts was text only (no visual components), if the post was restriced to 18 and over, if the visual included a video, and if the post was a spoiler for a film or other media. From the Title and Subreddit, we process the language in order to include text in our models. 

With these features, we believe we will be able to more accurately predict if a post is "hot" than the baseline, which is the majority class of 51% of our dataset having fewer comments than the median number of comments for the entire dataset. The models we will use are Logistic Regression and Random Forest. 

### Data Dictionary

|Feature|Description|
|:--|:-:|
|**title**|processed text of Reddit posts used in natural language processing|
|**subreddit**|Name of subreddit post originates from|
|**length_time_seconds**|amount of time in seconds a post has been up at time of collection|
|**num_comments**|Number of comments on a post at time of collection|
|**lemmatized**|Lemmatized text from Reddit post title|
|**num_tokens**|Number of tokens in Lemmatized text in titles|
|**stemmed_title**|Stemmed text from Reddit post title|
|**stem_count**|Number of stemmed text in reddit post title|
|**is_original_content_True**|If a post was original (1 = yes)|
|**is_self_True**|If a post was text only (1 = yes)|
|**is_video_True**|If a post included video (1 = yes)|
|**over_18_True**|If a post was restricted to 18 and over (1 = yes)|
|**spoiler_True**|If a post was a spoiler for some entertainment (1 = yes)|
|**num_crossposts**|Number of times a post was cross posted on Reddit|
|**score**|The number of times a post was upvoted|
|**subreddit_subscribers**|The number of subscribers to the subreddit of a post|


### Conclusions and Recommendations

Based on our analysis, both the Logistic Regression model and the Random Forest model were able to accurately predict if a post was "hot" at a rate of 74%. Random forest had slightly better results. 

The top subreddits that were most predictive of a post's class were wholesomememes, PolicalCompassMemes, SquaredCircle, PoliticalHumor, and IdiotsInCars. Even though wholesomememes had over 1.2M members, posts from this subreddit were .8 times less likely to be "hot". This indicates that even though there are lots of members seeing these posts, they are not interacting with the posts. Political posts elicit high levels of responses. These posts are often opinionated and therefore encourage people to respond with their own opinions or criticisms. IdiotsInCars was interesting because these posts were 3 times more likely to be "hot". Many people enjoy commenting about videos and pictures of poeple doing stupid things in cars. 

The top predictive words were "world", "game", "feel", "people", and "cat". Posts that included "world" most likely have to do with current events, which results in high levels of interaction. Posts with "game" have high levels of interaction indicating there are many reddit users who are sports fans and enjoy commenting and entering into dialogues on reddit. "Feel" posts are most often opinionated and therefore elicit responses of other peoples opinions or criticisms. And "cat" posts are .8 times less likely to be hot, meaning fewer people in general comment on posts about cats. 

The most predictive metadata feature we included was if a post was text only (not including any visual component). These posts made up 5% of our dataset, but were 4 times as likely to be "hot". These posts are most often simple posts about opinions that elicit high levels of interaction. 

We recommend you pay attention to which subreddit a post originates from and what type of members that subreddit consists of. High number of members does not always lead to high levels of interaction. Sports, political, and opinionated subreddits and posts often elicit high levels of interaction and are "hot". There are some keywords that are important to look at, but for the most part, they are not as powerful in predicting the level of interaction on a post as the aforementioned features. 
