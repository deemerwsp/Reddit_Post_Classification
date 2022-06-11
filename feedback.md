Problem Statement 3

The problem statement is provided for this project.

Data Collection 2

Was enough data gathered to generate a significant result? 3
- 10,075 posts were collected.
Was data collected that was useful and relevant to the project? 3
- Yes.
Was data collection and storage optimized through custom functions, pipelines, and/or automation? 1
- It appears you reran your scraping notebook 7 times in order to pull data. Consider trying to automate this in the future or putting the pipeline you created into custom functions in order to enhance the reusability.
Was thought given to the server receiving the requests such as considering number of requests per second? 3
- Yes, you limited the number of posts you were pulling and only made one request each time you ran your notebook.

Data Cleaning and EDA 2

Are missing values imputed/handled appropriately? 3
- Yes you dropped the columns with null values.
Are distributions examined and described? 3
- Yes.
Are outliers identified and addressed? 2
- You addressed outliers by removing posts that had over 1200 comments which is great. In the future show how you arrived at this number. Why was this number chosen as the benchmark for outliers? What graphs or information did you use to make this decision?
Are appropriate summary statistics provided? 2
- You talked about some statistics when you created all of your graphs. Consider pulling those statistics out as well as showing them in a graph.
Are steps taken during data cleaning and EDA framed appropriately? 3
- You did a great job including markdown in your data cleaning and EDA sections in order to guide your reader through the steps that you took and what the takeaways were.
Does the student address whether or not they are likely to be able to answer their problem statement with the provided data given what they've discovered during EDA? 2
- You individually addressed how each feature you looked at might impact your models later on but I was a bit unclear if you felt you would likely be able to answer your problem statement with the provided data.

Preprocessing and Modeling 3

Is text data successfully converted to a matrix representation? 3
- Yes
Are methods such as stop words, stemming, and lemmatization explored? 3
- Yes
Does the student properly split and/or sample the data for validation/training purposes? 3
- Good work fitting on only your training data.
Does the student test and evaluate a variety of models to identify a production algorithm (AT MINIMUM: two models)? 3
- 3 models were evaluated.
Does the student defend their choice of production model relevant to the data at hand and the problem? 3
- Good work explaining how your models are different relative to the data at hand.
Does the student explain how the model works and evaluate its performance successes/downfalls? 3
- You did a good job explaining how your random forest model is a better predictor for your target despite a reduction in interpretability.

Evaluation and Conceptual Understanding 2

Does the student accurately identify and explain the baseline score? 2
- You accurately identified the baseline score for your overall dataset but when evaluating the scores of your testing set the baseline would be the majority class within y_test. In your case this is 52.3%. Additionally it could be helpful to include a short explanation in your markdown explaining that the baseline is the majority class which in your case is the negative class.
Does the student select and use metrics relevant to the problem objective? 3
- Good work including and interpreting confusion matrices.
Does the student interpret the results of their model for purposes of inference? 3
- Great work here. If you are using logistic regression and interpreting the coefficients try to be a bit more explicit in your interpretations of them. Logistic and linear regression have great interpretability.
Is domain knowledge demonstrated when interpreting results? 3
- Yes
Does the student provide appropriate interpretation with regards to descriptive and inferential statistics? 3
- Yes

Conclusion and Recommendations 2

Does the student provide appropriate context to connect individual steps back to the overall project? 2
- Good work here. The one thing I would mention is that it wasn't always clear what part of your project was informing your conclusions.
Is it clear how the final recommendations were reached? 3
- You interpreted your models well in your modeling section so I knew how you reached your final recommendations. In the future it can be helpful to restate these in your conclusions. You did this well for some of your conclusions but not others. For instance you brought in your logistic regression coefficients when mentioning wholesome memes but not when talking about political posts.
Are the conclusions/recommendations clearly stated? 3
- Yes
Does the conclusion answer the original problem statement? 1
- The main issue here is that your problem statement is very brief and open ended. Once you edit your problem statement to be a bit more specific to your project this should be fixed.
Does the student address how findings of this research can be applied for the benefit of stakeholders? 2
- You talk a lot about what characteristics of a post on reddit are predictive of it's success but not as much about how your stakeholders could use this for their benefit.
Are future steps to move the project forward identified? 0
- No future steps are identified.

Project Organization 2

Are modules imported correctly (using appropriate aliases)? 3
- Yes
Are data imported/saved using relative paths? 3
- Yes
Does the README provide a good executive summary of the project? 3
- Yes. Good work here.
Is markdown formatting used appropriately to structure notebooks? 3
- Good work including markdown to help guide your reader through your logic.
Are there an appropriate amount of comments to support the code? 1
- You mostly used markdown instead of comments. If what you are writing in a markdown cell is only 1 line consider making it a comment.
Are files & directories organized correctly? 2
- You created a dataset folder to organize your data which is great. Try to create more directories to organize the rest of your files as well. This will become important as your projects become more complex.
Are there unnecessary files included? 3
- No unnecessary files
Do files and directories have well-structured, appropriate, consistent names? 3
- Yes

Visualizations 2

Are sufficient visualizations provided? 3
- Good work including a lot of visualizations as well as interpretations. I also liked the custom functions you created to make the easier for yourself. In addition to being easier it also helps to create a consistent look to your visualizations which adds cohesion to your overall project.
Do plots accurately demonstrate valid relationships? 3
- Yes
Are plots labeled properly? 3
- Yes
Are plots interpreted appropriately? 2
- For the most part yes. Be careful about interpreting correlations from scatter plots. They are a great way to get a general sense of the correlation of features but for actually making claims on correlation try to use something like the pearson correlation coefficients to get a more standardized and robust metric for your claims.
Are plots formatted and scaled appropriately for inclusion in a notebook-based technical report? 3
- Yes

Python Syntax and Control Flow 3

Is care taken to write human readable code? 3
- Great job using explicit names for your variables and columns.
Is the code syntactically correct (no runtime errors)? 3
- Yes
Does the code generate desired results (logically correct)? 3
- Great work, I couldn't find any part of your code that seemed to produce erroneous results.
Does the code follows general best practices and style guidelines? 3
- There were a couple of instances where you had long lines that got cut off on my screen but overall great work here.
Are Pandas functions used appropriately? 3
- Yes
Are sklearn and NLTK methods used appropriately? 3
- Yes
