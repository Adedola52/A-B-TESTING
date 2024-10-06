# A-B TESTING
**INTRODUCTION:**
A fintech company aims to increase the average transaction value of its users by 10% per month. To achieve this, the marketing team proposed sending a tutorial video to customers, 
explaining how to make easy and stress-free transfers. They believe that this initiative will result in an increase in the average transaction value per user each month.

However, the head of sales argued that the tutorial video would not lead to any significant change in transaction behavior. To validate both claims, it was decided to conduct an A/B test. 

In other to conduct this test, users will be splitted into two groups:
- **Test group:** The users in this group will be shown a tutorial video 
- **Control group:** The users in this group will not be shown a tutorial video
  
**Defining Hypotheses:**
- **Null Hypothesis (H0):** The tutorial video will not lead to any significant change in transaction behavior among customers.

- **Alternative Hypothesis (H1):** The tutorial video will help customers navigate the process of making seamless transfers, ultimately leading to an increase in average transaction values.

Before performing the test or analysis, it is important to determine an appropriate sample size for each group. This ensures that we have enough data to detect any potential change in average transaction value if such a change exists.
To achieve this, we perform **power analysis**.

**DATA SOURCE**

The dataset used was generated using numpy library funnctionalities in python

**DATA STRUCTURE**

There are *10,000 rows* in the DataFrame, each representing a cummulative of a user total engagement, as well as *6 columns*

- **user_id** - The user ID is the unique identifier
- **group** - The group the user belong to
- **transfers_completed** - Number of completed transfers through out the session
- **signup_date** - The date when the user signed up
- **age** - Age of users
- **gender** - Gender of users
- **signup_method** - How the user signed up

After conducting the test using the appropriate hypothesis testing method, here are the results:

The control group has an average transaction value of 6.031, while the test group has an average of 5.962. This indicates that the control group performed better than the test group in terms of average transaction value.

To determine whether this difference is statistically significant, we evaluated the following statistics:

- t_stat : -0.874
- p_value : 0.382
- critical value: ±1.96

**What the results interprets:**

**P-value:** Since the p-value (0.382) is greater than α (0.05), we fail to reject the null hypothesis. 

**T-statistic:** A t-statistic of -0.874 indicates that the test group's performance is not significantly different from the control group's performance, and in fact, it suggests that the test group performed worse, but this difference is not significant.

**Critical Value:** The critical value of ±1.96 sets the boundary for statistical significance. For a significant result, 
the t-statistic would need to fall outside this range (i.e., less than -1.96 or greater than +1.96). Since -0.874 is well within this range, this further supports failing to reject the null hypothesis.

**Conclusion:** We do not accept the alternative hypothesis (H1) because the evidence does not support that the test group improved significantly.
The result indicates that the control group performed better than the test group, but this difference is not statistically significant. 
Therefore, we can conclude that the performance difference could likely be due to chance, rather than a true effect of the tutorial.



**RECOMMENDATION**

Since the test did not show significant improvement, we might want to explore:

- **Reasons for the lack of improvement:** We should figure whether the tutorial was effective, engaging, or necessary.
- **Adjustments:** Perhaps improve the tutorial content or delivery and conduct further testing to gather more data.
- **User Feedback:** Conduct interviews or focus groups to understand user experiences and gather insights for improvement.
- **A/B Testing Formats:** Experiment with different tutorial formats (e.g., video vs. written) to find the most effective one.
- **Segmented Targeting:** Tailor tutorials based on user demographics or experience levels for personalized learning.
- **Follow-Up Support:** Implement reminders and additional support post-tutorial to reinforce learning.
- **Influencer Collaboration:** Partner with trusted figures for webinars or live sessions to increase credibility.
- **Social Proof:** Showcase testimonials or success stories from users who benefited from the tutorial.
- **Iterative Testing:** Continuously gather data and refine the tutorial based on user feedback.

**If you would like to read extensively on A/B testing with hypothesis testing, you can check out my blog post here;**
https://medium.com/@abowabat/a-b-testing-in-data-science-8abcd53e43b9
