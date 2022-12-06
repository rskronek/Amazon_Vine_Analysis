In this project I used US Pet product reviews from Amazon. The goal was to analyze if it would be worth it to subscribe to a Vine program if we were to sell similar products through their platform. The vine review program is an incentive model in which customers are gifted free stuff when they write good reviews. I was able to use PySpark to extract, transform, and load (ETL) the data to a AWS RDS I created and connected to my PostgreSQL server to be able to query it and extract my finished tables from there. Part of the data transformation was made using pandas as well.

Results
Paid Vine Program

170 total reviews
65 5-star reviews
38.23% of vine reviews were 5-star

Unpaid reviews

37840 total reviews
20612 5-star reviews
54.47% of unpaid reviews were 5-star

Summary
In conclusion, the vine program might just not be worth it for the Pet Products category. As it can be seen, there were not many helpful reviews that made part of it (total of 170), and less than half of them were 5-star rated (38%), where as the unpaid reviews which was just more than half of them were 5 star rated (54%). Even though the percentages may be misleading as the volume of reviews in the vine and non-vine programs vary so much, this itself is a sign that the vine program is not very popular in this category. We might not want to pay for it as it is not incentivizing the people to write better reviews.

This allows us to conclude that customers don't feel a positivity bias for leaving good reviews in the paid program as there are so few and not so many well-rated. Nevertheless, if we were to further analyze we could calculate the mean of the star ratings on each programs' reviews to see if there's a significant incentive.

avg_star_rating.png

In fact, there is a slight 0.2 difference in the average review star-rating in favor of the vine program. However, there is still not enough information to enroll in it. A great recommendation would be to apply a NLP sentiment analysis to check for the words used in the majority of the reviews. This way we could see if vine reviews are more touching and detailed, that we can feel customers have an incentive to leave great reviews.