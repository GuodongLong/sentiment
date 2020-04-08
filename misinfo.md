[Policy analysis](https://guodonglong.github.io/sentiment) | [Misinformation analysis](https://guodonglong.github.io/misinfo)


## Misinformation analytics

The spreading of misinformation will cause some unpredictable issues to the national healthcare system. 

## Case 1: Chloroquine has been approved to be used to treat COVID-19

In tragic news a man is dead and his wife is making a recovery in the US after they ingested a version of chloroquine, a substance Donald Trump falsely claimed had been approved to treat coronavirus.

President Trump claimed at a press conference on March 19 that the US would be making chloroquine, used to treat malaria, "available almost immediately" and that it had been approved by the Food and Drug Administration.


### Misinformation propgation on social networks

We compare the social impact of misinformation and the opponents who are fighting to the misinformation. The social impact will be calculated by counting # of tweets, # of retweets, # of likes, and # of audiences. If a person received the misinformation at earlier stage, we will count him/her as Believed group (Label 1). If this person received the message against misinformation, we will categorise him/her to the Against group (Label 2).

The influenced count comaprison will be visualised by a race bar chart. 
<img src="https://guodonglong.github.io/sentiment/bar-chart-race.png" height="60%" width="60%">

- [Bar chart race](https://observablehq.com/@d3/bar-chart-race)<<<click it to see the interactive demo
- **Figure 1. Comparison of social impact between misinformation and its opponents.**
- Description: ...


The below figure display the spreading of misinformation over geo locations.
<img src="https://guodonglong.github.io/sentiment/map-interactive-spread.png" height="60%" width="60%">

- [Interactive map](https://bl.ocks.org/GerardoFurtado/02aa65e5522104cb692e)<<<click it to see the interactive demo
- **Figure 1: An interactive map to demonstrate the influence of misinformation and its components.** 
- Descriptions: ...



### Data acquistion
- Hashtags: #chloroquine
- Related keywords: Donald Trump, Coronavirus.
- Time: Since 19 Mar 2020
- The data will be collected through a depth-first search. We search the tweets using the Hashtags, and then searched who retweet or like this message. Once we get all tweets related to this topic, we also need to acquire the involved accounts and their followers who can see the message but never take any actions on social media. 



### Labelling tweets
- Label 1: Believed/Positive/Supportive comments to the misinformation. The people who retweet the misinformation will aslo belong to the support of spreading misinformation.

https://twitter.com/realDonaldTrump/status/1241367239900778501

https://twitter.com/kakape/status/1247628714864771072

- Label 2: Against/Negative/Fighting to the misinformation.

https://twitter.com/NafdacAgency/status/1247459498031304704

- Label 3: Unrelated messages.


Notice: There is no neural comments for the misinformation. If you spread the misinformation, you will be part of the believed poputaion. The labelling process could be an active learning process.

