# Will a customer accept the coupon? 

This project analyzes factors that influence whether a customer accepts a coupon. The project explores the dataset using 
visualizations and basic probability and statistics to characterize customers who accepted a coupon.

## Overview

This repository contains a Jupyter Notebook and a dataset for exploratory data analysis (EDA) of a coupons dataset. 

The analysis focuses on:
- Cleaning and understanding the data
- Visualizing distributions and relationships
- Comparing groups of accepting coupons
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

When I look at all the data, the acceptance rate is 56.93% across all coupon types. But for bar coupons specifically, 
it is much lower at only 41.19%. This tells me that acceptance of bar coupons depends more on personal habits and lifestyle 
compared to other coupons like "Carry out" or "Restaurant (<$20)", which more people use.

### 2. The Role of Regular Habits

**How Often People Visit Matters:**

Drivers who go to bars at least once per month accept the coupon much more often.

**The "Regular Customer" Pattern:** In Question 3, I saw that most acceptances (33.51% of all bar coupons) come from 
people who visit bars 3 times or less per month. But this is probably because there are more people in this group. 
However, when I looked at Question 6, I concluded that people who frequent bars are the main group accepting these coupons.

### 3. Who Accepts and Social Situations

**Age and How People Live:**

The drivers over 25 years old who regularly go to bars (Question 4) are only 14.53% of acceptances. This means younger 
drivers who are under 25, or people who do not visit bars often, they make up bigger portion of people accepting the bar coupons.

**Traveling with Children is Important:** When drivers have children with them, they do not want bar coupons. The data 
shows that drivers accept bar coupons much more when kids are not in the car (Question 5).

**What Job People Have:** The lifestyle and work background also matter. Drivers who work in jobs that are not farming, 
fishing, or forestry showed a different pattern for accepting coupons.


### 4. Finding the Best Target Groups

When I analyzed Question 6, I found a specific "profile" that represents 65.23% of all accepted bar coupons. This high 
success group has these characteristics:

- **Social and Regular Visitors:** These are people who go to bars frequently, and they are either younger than 25 or they are not widowed.
- **People Looking for Good Deals:** These individuals often go to cheap restaurants and earn less than $50,000 per year.

**Conclusion:** The best target customers for bar coupons are young people and those who like cheap dining and frequent 
cheap restaurant visits. The marketing should focus on these groups and avoid sending coupons when drivers have children in the car.

# Independent Investigation

Based on the analysis of the data, the top performing coupons are "Coffee House", "Restaurant(<20)", and "Carry out & Take away". Below are the key findings:

### Problem Statement

Understanding which factors influence the acceptance of the top 3 coupons to optimize targeting and maximize redemption rates.

### Key Insights

**1. Time of Day Impact**
The acceptance patterns show that time matters. Around 2 PM is when people accept most coupons, probably because it's 
lunchtime or an afternoon break. Morning time, 7 AM, is also good, people going to work want coffee or breakfast. 
Evening time after 6 PM is not so strong for acceptance.

**2. Social Context is Very Important**
When people travel with friends, they accept coupons more than when alone or with kids. Having kids in the car lowers 
the acceptance rate, parents probably want to get home fast without stopping. Partners also show moderate acceptance, 
but the friends group is the best target.

**3. Age Demographics**
Younger people, aged 21-31,  accept coupons more than older groups. The heatmap shows that people aged 21-26 have the 
highest acceptance rates across all coupon types. Maybe younger people are more price sensitive or more open to try new things.

**4. Weather Effects**
Sunny weather shows the best acceptance rates. When the weather is rainy or snowy, people don't want to make extra stops. 
This makes sense because nobody wants to get out of the car in bad weather just for a coupon discount.

**5. Destination Matters**
People with "No Urgent Place" accept coupons the most. When going to work or home, acceptance is lower, they probably 
already have specific plans. This suggests that coupons work better for relaxed trips than commute trips.

### Actionable Recommendations

**For Marketing Teams:**
- Send coupons during lunch hours, 2 PM, and morning commute, 7 AM to 10 AM, for best results
- Target people who are traveling with friends, this is your best customer segment
- Focus on sunny days for coupon campaigns, and avoid sending coupons during bad weather
- Don't waste resources sending to drivers with kids
- Young adults from 21 to 30 should be the priority demographic group

**For Business Strategy:**
- Coffee House coupons work very well across all segments. Consider increasing coffee promotions
- Restaurant(<20) coupons perform better when people are not in a hurry
- Cheap dining options (under \$20) attract budget-conscious customers earning less than $50K

**Next Steps:**
1. Test campaigns comparing morning vs. lunch time distribution
2. Create special "friends group" promotions with higher value to promote acceptance
3. Develop a weather based coupon system that pauses campaigns during rain

These findings suggest that a successful coupon strategy needs to consider not just the product but the entire context 
of the customer journey, including where they are traveling, who they are with, where they are going, and what the weather is like.