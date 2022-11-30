# [Netlogo's Global Community](https://easy.quarto.pub/netlogos-global-community/) 
## Before you go any further, check out the final product [here!](https://easy.quarto.pub/netlogos-global-community/) 

Thank you for stopping by and checking out my project! I had a lot of fun putting it together-- while I'm sure there's a lot of
room for improvement, I always learn the most when I actually get to apply the skills I practice with homework. 
This was my thought process as I this whole thing together, as well as an explanation of everything in this repo.

### The Raw Data 
This probably needs little explanation, but in the [raw-data folder](https://github.com/emzou/cclcontribdatavis/tree/main/raw-data), 
you'll find a json file with the CCL's historical contribution data. 

### Preprocessing 
[Here](https://github.com/emzou/cclcontribdatavis/tree/main/preprocessing), you can see how I cleaned up the json file with some very
basic Python. Because I wanted to tell a story about Netlogo's global userbase, I needed locational data, but that wasn't included with 
the raw data. I turned the raw json file into dataframes easier to use with R. I did some additional minor cleaning up in R later.

### The Data Visualizations 
This project contains five different visualizations, which were all built using R and viewable in the qmd file [here](https://github.com/emzou/cclcontribdatavis/tree/main/data-visualization).
#### 1: The Interactive Map 
This visualization allows the reader to get an idea of NetLogo's global spread at a glance. For those unfamiliar with NetLogo,
it's hard to otherwise illustrate the breadth of its influence. However, I suspect that this tool may be more useful to members of the
NetLogo team, as they are intimately familiar with their own product. Would this spread confirm their existing ideas of who is 
using NetLogo, or are there areas that unexpectedly do or do not contribute their models? The detail of this visualization is also helpful
in that regard, as users can zoom in a lot. 

#### 2: The Animated Map 
I used the gganimate and gifski packages to put this visualization together. Besides an overall increase in models, 
I didn't find any particular trends over time by location, other than a slight increase in contributions from the Global South. 
Because I myself am not on the NetLogo team, I'm not able to extrapolate as much from a visualization showing change over time, but this visualization
would be helpful to understand the impact of specific updates and campaigns. I also just think its a cute animation, with all these models lighting up 
around the world. 

#### 3: Country Bar Chart 
This bar chart concisely shows which countries have contributed the most over time. To me, there are two key insights from this. The first is that it 
very nicely demonstrates the overall theme of this project, NetLogo's diverse user base. Though the maps are fun to look at, the roster of countries adds more 
clarity. Secondly, for the NetLogo team, the distribution of the countries provides insight into which specific countries-- and maybe which universities/programs-- 
are using NetLogo. 

#### 4: Continent Contributions by Time 
This line graph allows users to further explore what the animated map shows. The Americas and Europe are the only regions that consistently output
contributions, which would be an important insight for the NetLogo team. 

#### 5: Reactable 
While it is a lot of data, I thought it was important to add the entire data set for the sake of transparency. It also allows readers to page through 
variables I did not depict in the visualizations-- organization names and occupations. 
