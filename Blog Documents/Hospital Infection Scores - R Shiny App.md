---
title: "Hospital Infection Scores - R Shiny App"
author: "Scott Stoltzman"
date: "May 14, 2017"
output: html_document
---

## Hospital Infection Scores - R Shiny App

About two weeks ago I created an extremely rough version of an R Shiny Application surrounding Medicare data. Right after publishing the blog post, I received a lot of input for improvement and help from others. 

Here's a look a look at the latest version of the [Medicare Shiny App](https://stoltzmaniac.shinyapps.io/medicare_data/). This utilizes data.gov [found here](https://catalog.data.gov/dataset/healthcare-associated-infections-hospital-3ca5e).

I was traveling for two weeks and had very little time to do any work on it. After creating a [GitHub Repository](https://github.com/stoltzmaniac/Medicare/tree/master/shinyApp) for it, the user [Ginsberg](https://github.com/ginberg) played a huge role in cleaning it up and adding a lot more functionality. I found it incredible that a complete stranger to me would put in such effort to something like this. In fact, he isn't even a resident of the USA - so Medicare probably isn't on his radar as often as it is for some of us. Fantastic generosity! 

Ultimately, I will be looking to keep this project alive and grow it to fully utilize a lot more of the Medicare data available. The infections data set was very simple and easy to use, so I started off with it but there are a lot more tables listed on data.gov. The purpose of this application is to allow people who don't want to spend time digging through tables to utilize the information available. This isn't necessarily just for people seeking care to make a decision but this could perhaps be utilized for others doing research regarding hospitals in the US.

The R Shiny App allows you to filter by location and infection information. These are important in helping to actually find information on what you care about.

Three key tabs were created by (@Ginsberg):  

  * Sorting hospitals by infection score
  * Maps of hospitals in the area
  * Data table of hospital data
  
---------  

#### Sorting hospital data by score:  

  * This is a tricky plot because "score" is different for each type of metric
  * Higher "scores" aren't necessarily bad because they can be swayed by more heavily populated areas (or density)
  * Notice the use of plotly and its interactivity
  
  
![](https://www.stoltzmaniac.com/content/images/2017/05/blog_2_01.png)
  
  
---------    
  
#### Map of the data:  

  * Location of the hospitals is incredibly important if you happen to live in a certain area
  * The radius of the circle allows for easy identification of places with larger "scores"
  * Hovering and clicking the circle will display more information
  
  
![](https://www.stoltzmaniac.com/content/images/2017/05/blog_2_02.png)
  
---------    
  
#### Displaying the data in table format:  

  * This allows for visibility into the raw data that is populating the other tabs
  * It provides the ability to download a CSV or PDF file containing the relevant information
  * More information may be added such as the address and telephone number of the hospital - depending on the direction of the app
  
  
![](https://www.stoltzmaniac.com/content/images/2017/05/blog_2_03.png)


Again, I want to give a big thanks to [Ginsberg](https://github.com/ginberg) for essentially creating 95% of what makes this app great!

Here's the link to the [Medicare Shiny App](https://stoltzmaniac.shinyapps.io/medicare_data/).  

You can find the code on my [GitHub](https://github.com/stoltzmaniac/Medicare).
