# Data Analysis of Kickstarter Project’s Success Rates of 2015 to Today
Using numpy, pandas, matplotlib, and Counter libraries, I make analysis of Kickstarter projects and its succes rates overall.

First let’s start off with knowing what exactly a Kickstart project is. A Kickstarter is a funding platform for creative projects. Any ideas a creator has will try to persuade funders by displaying a clear goal, or showing a prototype of the idea, to chip in to the project. Projects range from technology to a piece of art to even video games. There’s a wide range of categories of projects of Kickstarter.

This article is an overview of the statistical analysis of data collected by https://www.kickstarter.com/ and is primarily focused on the success rates of these Kickstarter projects that creators try to get funding for. This data was formatted into a csv by user Kemical from https://www.kaggle.com/. This data will cover a total of 370,454 Kickstarter projects in 2015 to today and all the currency has been converted to USD.

# Success Rates
I should mention that failing a Kickstarter project is not as big as a risk as starting a business; according to the website, if a project does not reach its funding goal, creators will not be expected to complete their project without the funds necessary to do so. I just want to provide some statistical information, so creators will see this and decide to see if their project is worth putting their time in it or not.

: I made four groups of projects: overall success rate, success rate with project’s goal of $5,000 USD or less, success rate with project’s goal of $5,000 USD to $20,000 USD, and success rate with project’s goal of $20,000 USD or more. Then these groups had two side by side comparisons of success rate with cancellation and without cancellation. The reason for this is if I am looking for the true success rate, I should include all states of goals, but if a creator just wanted to view success to failure rate, then that’s possible, too.

Now on to the analysis. Overall, there was a total of 133,956 successful projects, 197,719 failed projects and 38,779 canceled projects (35.38% with cancellations and 40.39% without). With projects whose goal is to pledge $5,000 USD or less, 82,250 were successful, 85,669 failed and 18,863 canceled (44.04% with cancellations and 48.98% without). Projects whose goal is to pledge $5,000 USD to $20,000 USD, 35,615 were successful, 57,558 failed and 13,269 canceled (33.46% with cancellations and 38.22% without). With projects whose goal is to pledge $20,000 or more, only 16,091 were successful, 54,492 failed and 14,854 canceled (18.83% with cancellations and 22.8% without). As you can see, more projects are failing as the goals get larger. You would have a better chance at success focusing on a project that is inexpensive as it is quicker to achieve and isn’t farfetched. Even though projects with goals of $5,000 USD have the highest success rate, it still is not high; you pretty much have a less than 50% chance of having your project be successful. The stats showed interesting results, and makes you question further in depth when trying to get funding to your project. Some examples include which category has the best success rate or why are large goals failing. Read on to find answers to these questions.

![alt text](https://raw.githubusercontent.com/mikeyyg96/data-analysis-kickstarter/master/success_rate_graph.JPG)

# Which category has the best success rate?
You’ve read the success rates and weren’t really excited about the results of success rates. So maybe there’s some project decisions to make that will increase the chance of your Kickstarter project being successful. The main categories that Kickstarter groups are as follows: Film & Video, Food, Design, Games, Art, Technology, Fashion, Publishing, Music, Photography, Comics, Theater, Journalism, Dance, and Crafts. The graph below shows which group has the highest success rate without any cancellations, as it was just focused on success to failure.

![alt text](https://raw.githubusercontent.com/mikeyyg96/data-analysis-kickstarter/master/categoy_success_rate.JPG)

# Why are large goals failing
Aside from the large goal demand, there are other factors that could potentially cause the success rate to be so low. A thing I looked at when working with the data was the success rates of just projects with large goals ($20,000 USD or more). The list were all low values, with the minimum value 0.7% and the maximum value being 35%. The mean was 0.21 with a standard deviation of 0.7, so most of the success rates lied between 14% to 28%. I wanted to see the impact the low values had on the high values, so I counted the number of projects total below the mean and counted the number of projects above the mean. I found interesting results and came up with 49,994 for the first half compared to 25,322! This makes a lot more sense now. A potential reason that the rates are lower, along with the large goal demand, is that there are many Kickstarter projects that fall into the unpopular categories. Over 30% of projects in the first half is technology, which is reasonable since technology does require a lot of money to fund, but does not gain enough trust from funders, or probably not enough detail about the project. Taking out the first half increases the success rate overall by 4.5%, which is still low.

# Conclusion
Don’t let this statistical analysis stop you from working on a project and needing funds for it. The objective of this analysis is to guide creators to proceed with caution and make the best decision to help you. I do advise to start with projects that have low goals to pledge and one of the top categories as you will have a better success rate than average. Good luck!
