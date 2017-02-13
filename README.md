# Kickstarter_from_Kaggle
Crowdfunding has become one of the main sources of initial capital for small businesses and start-up companies that are looking to launch their first products. Websites like Kickstarter and Indiegogo provide a platform for millions of creators to present their innovative ideas to the public. This is a win-win situation where creators could accumulate initial fund while the public get access to cutting-edge prototypical products that are not available in the market yet.

At any given point, Indiegogo has around 10,000 live campaigns while Kickstarter has 6,000. It has become increasingly difficult for projects to stand out of the crowd. Of course, advertisements via various channels are by far the most important factor to a successful campaign. However, for creators with a smaller budget, this leaves them wonder,
~by Cathie So on Kaggle, see more at https://www.kaggle.com/socathie/kickstarter-project-statistics

## Data Sources

All of raw data are scraped from Kickstarter.com.

<li> First 4000 live projects that are currently campaigning on Kickstarter (live.csv) </li>

* Last updated: 2016-10-29 5pm PDT
* amt.pledged: amount pledged (float)
* blurb: project blurb (string)
* by: project creator (string)
* country: abbreviated country code (string of length 2)
* currency: currency type of amt.pledged (string of length 3)
* end.time: campaign end time (string "YYYY-MM-DDThh:mm:ss-TZD")
* location: mostly city (string)
* pecentage.funded: unit % (int)
* state: mostly US states (string of length 2) and others (string)
* title: project title (string)
* type: type of location (string: County/Island/LocalAdmin/Suburb/Town/Zip)
* url: project url after domain (string)

<li> Top 4000 most backed projects ever on Kickstarter (most_backed.csv) </li>

* Last updated: 2016-10-30 10pm PDT
* amt.pledged
* blurb
* by
* category: project category (string)
* currency
* goal: original pledge goal (float)
* location
* num.backers: total number of backers (int)
* num.backers.tier: number of backers corresponds to the pledge amount in pledge.tier (int[len(pledge.tier)])
* pledge.tier: pledge tiers in USD (float[])
* title
* url

See more at http://datapolymath.paperplane.io/

## This project
**I try to figure out the relation between tier structure and amount of pledged.**

## Conclusion
* These projects on Kickstarter have about 10 tiers is very popular.
* We found that second to seventh price in "pledge.tier_num" is really important, they make a huge contribution to the funding cases.
* The "median price" in the project is very important.
* The contribution of crowd maybe meets the "long tail theory", so the big part of contribution is at the lower price.
