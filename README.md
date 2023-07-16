# Assignment 1: Protests

During the past few years in the United States, there has been a surge of protests in support of the Black Lives Matter movement, women's rights, trans rights, immigration reform, gun control, the environment, and many other social and political issues.

In this assignment, you will work with data from [CountLove](https://countlove.org/), a group that collects data about protests from across the United States, including information about the purpose of the protests, the location of the protests, as well as how many people attended the protests. This data has often been [cited by the *New York Times*](https://www.nytimes.com/2020/08/28/us/black-lives-matter-protest.html), among other major outlets.

Through this assignment, you will be able to answer questions including:
- What were the most attended and least attended protests in the US in the last 5 years?
- How many protests occurred in Washington state?
- How did the number of protests in 2019 compare to 2020, and why?
- Why are people protesting in the US? What are the biggest motivators?


This assignment is divided into 2 parts. You will complete your coding work in the `analysis.R` file, and you will write short answer responses related to critical analysis and reflection of the data in this `README.md` file. Before getting started on your coding work, you should complete the section **"Critical Analysis & Reflection: Before You Code"** below.

When you are finished with the assignment, be sure to push all changes to your GitHub repository and then submit the link on Canvas.

## Before You Code: Critical Analysis & Reflection

Before diving into this (or any) dataset, it's important to know where the data came from, and it's important to have or to seek out _domain familiarity_ — in other words, knowledge about the subject/topic of the dataset. (We don't want to be "strangers in the dataset," as Catherine D'Ignazio and Lauren Klein describe it.)

To get more familiar, we are going to begin by doing some background reading.

- First, please read [this FAQ](https://countlove.org/faq.html) from the CountLove website and the opening of [this blog post](https://www.tommyleung.com/countLove/index.htm). Based on the information in these pieces, why did the creators start collecting the CountLove data? Please answer in 2-3 sentences (3 points)
**The authors decided to start collecting data on protests and demonstrations because they are a good way to commmunicate with elected leaders. They hope to keep a record of this data in order to support a "diverse, empathetic, and kind country" (*Leung & Perkins*). This is also being done because there is barely any data being gathered on this topic despite being commonly and widely reported in news articles.**

- Next, we would like you to read this [*New York Times* piece, which uses CountLove data](https://www.nytimes.com/interactive/2020/06/13/us/george-floyd-protests-cities-photos.html) (here's a [Google Doc version for anyone who gets paywalled](https://docs.google.com/document/d/1sdjFsA5csYuH4plNEEk7WXT77K5h5ZuyW05CBwYdk6A/edit?usp=sharing)), and which describes the Black Lives Matter protests that occurred in the summer of 2020. Please summarize the main point or argument of this article in 2-3 sentences (3 points)
**The main point of the article is to show the widespread response to the response to the death of George Floyd. This is done by showing the reader visualizations of where protests are happening and by showing how participants from multiple diverse communities came together to support black lives. The story is told in chronological order showing the progression of the movement.**

Next, we're going to reflect about who collected this data, and what's actually inside it.

- Who collected and shared the CountLove data, and what do they do for a living? Please answer in 1-2 sentences(2 points)
**One of the authors of the CountLove data is Tommy Leung was a student at MIT who enjoys cooking, coding, and drinking coffee. The other author, Nathan Perkins, was also an MIT graduate student, studies brains, and participated in multiple projects in the last several years.**

- As Klein and D'Ignazio remind us, when it comes to data, "what gets counted counts." What types of demonstrations does CountLove include in their data, and what types do they exclude? (3 points)
**As mentioned on the CountLove website, they do not count protests that are not out of the ordinary. This means they do not include awareness events, celebrations, reenactments, fundraising, and political rallies**

- How and where does CountLove get their data about the protests? Please answer in 2-3 sentences (2 points)
**CountLove gets its data from news articles. They automate most of the process but the two authors have to manually read through the articles to create descriptions for each protest and decide on other metrics such as attendance count.**

- How does CountLove make their estimates about the number of people who attended a protest? What potential problems might arise from this method of estimation? Please answer in 3-4 sentences (4 points)
**They estimate the number of attendees through primary sources such as news reports or videos. The exact number is recorded very conservatively with a dozen being translated to 10 or hundreds being translated to 100. While this obviously can lead to data that underrepresents the true scale of the protest or demonstration, it could also lead other consequences in during data analysis such as underrepresent the amount of partcipation in protests and demonstrations nationwide.**

## While You Code: Critical Analysis & Reflection

- Reflection 1: Why do you think the mean is higher than the median? Which metric would you use in a report about this data, and why? Please answer in 2-3 sentences (2 points)
**The mean is different from the median because the mean is influenced by outliers and skew of the data distribution more. The mean being significantly higher than the median means that the data is either skewed left, there are protests with an extremely high amount of attendees (outliers), or both. If I were to report on the data, I would use the median since it is a better representation of typical values in the data**

- Reflection 2: Before actually calculating the number of protests that occurred in 2018, 2019, 2020, record your guesses for the following questions. (1 point)

  Guess: Do you think there were more protests in 2019 than in 2018? Why or why not? Please answer in 1 or 2 sentences
  **I think that there were more protests in 2019. I believe that due to the increased polarization of values and increased connectivity through social media every year, it would lead to more demonstrations and protests.**

  Guess: Do you think there were more protests in 2020 than in 2019? Why or why not? Please answer in 1 or 2 sentences
  **I think that there were more protests in 2020. Despite the COVID19 outbreak, I believe that there was more awareness and participation in protests and demonstrations especially involving social justice issues.**

- Reflection 3: Does the change in the number of protests from 2018 to 2019 to 2020 surprise you? Why or why not? What do you think explains the fluctuation? Please answer in 1 or 2 sentences (2 points)
**The decrease in the number of protests from 2018 to 2019 does suprise me.However, a reason for the large number of protests in 2018 might be because of the ongoing trade war at the time. The increase in protests in 2020 didn't suprise me, especially given in the increased concern with social justice issues and BLM movement gaining a significant amount of traction.**

- Reflection 4: What is the first and fourth most frequent category of protest? Do these frequencies align with your sense of the major protest movements in the U.S. in the last few years? Why or why not? (3 points)
**The first most frequent category of protest is Racial Injustice at 10620 and the fourth most frequient category of protest is Immigration at 3496. These frequencies do align with the topics of major interest that have been trending in the news in recent years. We can often see debate over immigration and alot of support for BLM as these topics appear in social media, Presidential debates, and television.**

## After You Code: Critical Analysis & Reflection

In the second chapter of *Data Feminism*, Klein and D'Ignazio describe 4 ways that data scientists can challenge power and take action:
> Taking action can itself take many forms, and in this chapter we offer four starting points:  
> (1) Collect: Compiling counterdata—in the face of missing data or institutional neglect—offers a powerful starting point as we see in the example of the DGEI, or in María Salguero’s femicide maps discussed in chapter 1.  
> (2) Analyze: Challenging power often requires demonstrating inequitable outcomes across groups, and new computational methods are being developed to audit opaque algorithms and hold institutions accountable.  
> (3) Imagine: We cannot only focus on inequitable outcomes, because then we will never get to the root cause of injustice. In order to truly dismantle power, we have to imagine our end point not as “fairness,” but as co-liberation.  
> (4) Teach: The identities of data scientists matter, so how might we engage and empower newcomers to the field in order to shift the demographics and cultivate the next generation of data feminists?  

- How does the CountLove project embody one or more of these 4 forms of challenging power? Please answer in at least 3-4 sentences (3 points)
**The CountLove project embodies the first way of challenging power through collecting and compiling counterdata in the face of missing data. It was mentioned in the CountLove FAQ that there were no other databases like this before, despite protests and demonstrations being an important tool for driving social change. This can also been seen as a way of challenging power since a large institution would not willingly create open source database on critcism they received throughout the years despite it being a very important piece of information for people to know and understand.**

- What is the most interesting or surprising thing you learned from this analysis? Please answer in at least 2-3 sentences (2 points)
**The most suprising thing that I learned from the analysis is that there was a decrease in the number of protests that don't count as regular business in 2019 compared to 2018. It was also interesting to see that despite the COVID19 outbreak, the number of protests and demonstrations in 2020 nearly doubled that of 2019.**

- What is a kind of analysis that you would like to do or that would be interesting to do with the CountLove data that you don't have the time or skills to accomplish at this moment? Please answer in at least 2-3 sentences (2 points)
**I would like to have created some data visualizations. For example, I believe that creating a visualization of the number of protests by state, the most common types of protests by state, or a graph of the number of protests over time would grant us additional insights on the data that we did not have before.**
