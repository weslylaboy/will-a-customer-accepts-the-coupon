# Will a customer accepts the coupon? 

This project analyze factors that influence whether a customer accepts a coupon. The project explores the dataset using 
visualizations and basic probability and statistics to distinguish between customers who accepted a coupon versus those who did not.

## Overview

This repository contains a Jupyter Notebook and a dataset for exploratory data analysis (EDA) of a coupons dataset. 

The analysis focuses on:
- Cleaning and understanding the data
- Visualizing distributions and relationships
- Comparing groups (accepted vs. not accepted)
- Drawing insights about features that may correlate with coupon acceptance


## Dataset

- Source file: `data/coupons.csv`
- Format: CSV
- Note: The dataset is provided in this repo for convenience. If the dataset is updated or moved, adjust the notebook path accordingly.


## Project Structure

```
.
├── README.md                     # Project documentation (this file)
├── prompt.ipynb                  # Main analysis notebook (EDA and insights)
├── data/
│   └── coupons.csv               # Dataset used by the notebook
```


## Key Findings: Bar Coupon Acceptance


### 1. General Acceptance Patterns

**Overall versus Specific Coupons:**

When I look at all the data, the acceptance rate is 56.93% for all types of coupons. But for bar coupons specifically, it is much lower at only 41.19%. This tells me that bar coupons are depending more on the personal habits and lifestyle of people compared to other coupons like "Carry out" or "Restaurant (<$20)" which more people can use.

### 2. The Role of Regular Habits

**How Often People Visit Matters:**

The drivers who go to bars at least once per month, they accept the coupon much more.

**The "Regular Customer" Pattern:** In Question 3, I saw that most acceptances (33.51% of all bar coupons) come from people who visit bars 3 times or less per month. But this is probably because there are more people in this group. However, when I looked at Question 6, the people who go frequently to bars, they are the main group accepting these coupons.

### 3. Who Accepts and Social Situations

**Age and How People Live:**

The drivers over 25 years old who regularly go to bars (Question 4) are only 14.53% of acceptances. This means younger drivers who are under 25, or people who do not visit bars often, they make up bigger portion of people accepting bar coupons.

**Traveling with Children is Important:** When drivers have children with them, they do not want bar coupons. The data shows very clearly that drivers accept bar coupons much more when kids are not in the car (Question 5).

**What Job People Have:** The lifestyle and work background also matters. Drivers who work in jobs that are not agricultural (I mean not farming, fishing, or forestry) showed different pattern for accepting coupons.

### 4. Finding the Best Target Groups

When I analyzed Question 6, I found a specific "profile" that represents 65.23% of all accepted bar coupons. This high success group has these characteristics:

- **Social and Regular Visitors:** These are people who go to bars frequently, and they are either younger than 30 or they are not widowed.
- **People Looking for Good Deals:** These individuals go often to cheap restaurants and they earn less than $50,000 per year.

**My Conclusion:** The best target customers for bar coupons are young people and people who like budget friendly dining and eat frequently at cheap restaurants. The marketing should focus on these groups, and should avoid sending coupons when drivers have children in car.


# Independent Investigation

Based on analysis of the data, the top performing coupons are "Coffee House", "Restaurant(<20)", and "Carry out & Take away". Below are the key findings:

### Problem Statement
Understanding which factors most strongly influence acceptance of top 3 coupons to optimize targeting and maximize redemption rates.

### Key Insights

**1. Time of Day Impact**
The acceptance patterns show that time matters a lot. Around 2PM (14h) is when people accept most coupons, probably because is lunch time or afternoon break. Morning time (7AM) also good, maybe people going to work want coffee or breakfast. Evening time (6PM-10PM) is not so strong for acceptance.

**2. Social Context is Very Important**
When people travel with friends, they accept coupons more than when alone or with kids. Having kids in the car makes acceptance much lower, parents probably want to go home fast and not stop. Partners also show moderate acceptance, but friends group is the best target.

**3. Age Demographics**
Younger people (around 21-31 years) accept coupons more than older groups. The heatmap shows that people aged 21-26 have the highest acceptance rates across all coupon types. Maybe younger people are more price sensitive or more open to try new things.

**4. Weather Effects**
Sunny weather shows the best acceptance rates. When the weather is rainy or snowy, people don't want to make extra stops. This makes sense because nobody wants to get out of the car in bad weather just for a small discount.

**5. Destination Matters**
People with "No Urgent Place" accept coupons the most. When going to work or home, acceptance is lower, they probably already have specific plans. This suggests that coupons work better for leisure trips than commute trips.

### Actionable Recommendations

**For Marketing Teams:**
- Send coupons during lunch hours (2PM) and morning commute (7AM-10AM) for best results
- Target people who are traveling with friends, this is your best customer segment
- Focus on sunny days for coupon campaigns, avoid sending during bad weather
- Don't waste resources sending to drivers with kids unless it's a family restaurant
- Young adults (21-30) should be the priority demographic group

**For Business Strategy:**
- Coffee House coupons work very well across all segments. Consider increasing coffee promotions
- Restaurant(<20) coupons perform better when people are not in a hurry
- Cheap dining options (under \$20) attract budget-conscious customers earning less than $50K

**Next Steps:**
1. Test campaigns comparing lunch time vs. dinner time distribution
2. Create special "friends group" promotions with higher value
3. Develop a weather based dynamic coupon system that pauses campaigns during rain

These findings suggest that a successful coupon strategy needs to consider not just the product, but the entire context of the customer journey, when they travel, who they are with, where they are going, and what the weather is like.