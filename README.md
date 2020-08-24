# Exploratory Data Analysis of Movies Via TMDb
Completed by: Marvin Lee


# Big Question: Should Microsoft create a new movie studio, and if so what is the recommended film production strategy?

<ul>
    <li>Which production companies have been the most successful of recent?</li>
    <li>What's the correlation between popularity score and gross income for films?</li>
    <li>How can the global economy / a global potential user base be well-incorporated into Microsoft's plans?</li>
    <li>Is there data to support a new movie studio launch in a particular niche?</li>
</ul>


# Process & (Data Science) Tools Used:

<ul>
    <li>Scraped data solely from TMDb via API, using TMDb Wrapper</li>
    <li>Researched the length of time it takes to go from movie announcement to release date</li>
    <li>Queried the <i>movies.Popular</i> filter to obtain 1000/3000 movie IDs that were then used to pull data from the <i>movies.Info</i> database</li>
    <li>Created dataframes specific to the questions I posed</li>
    <li>Leveraged the following tools: Pandas, FuncFormatter, Matplotlib, Seaborn, and Squarify</li>
    <li>Used <b>Budget</b> and <b>Revenue</b> to create a new column: Gross Income</li>
    <li>Created visualizations to gain insights into the data</li>
    <li><b>Focused largely on films released from 01-2017 to 12-2019</b></li>
</ul>


# Findings:


### Which production companies have been the most successful of recent?

From the beginning of 2017 to the end of 2019, Walt Disney Pictures has consistently proven to be number 1 in gross earnings, via the random selection of 1000 movie titles from TMDb's <b>Popular</b> filter (conducted 7 random selections until now). What's more, a Genre Dominance query among these films showed that Action, Drama, Thriller and Adventure are consistently the top genres. I recommend using the top 20 production companies as a benchmark for movie studio film production while focusing on any of the 4 mentioned genres.

![alt text](https://github.com/emel333/moovee_insights/blob/master/production%20companies%20top%2020.png "Top 20 Top-Earning Production Companies")

![alt text](https://github.com/emel333/moovee_insights/blob/master/genre%20dominance%20top%20earners.png "Genre Dominance Among Top 20 Production Companies By Earnings")


### How seriously should popularity score be taken?

It's been discovered that there is, indeed, a positive correlation between popularity score and gross income. However, what's interesting is that this doesn't necessarily translate to <i>high</i> popularity scores. It is very much possible to have a high-earning film receive a seemingly mediocre or low popularity score. The Boxplot portion of the chart below shows that the majority of popularity scores for top-earning films falls within the range of 20-40. So, I don't recommend producing films according to <i>high</i> popularity scores.

![alt text](https://github.com/emel333/moovee_insights/blob/master/popularity%20score%20all%20films%2036%20months.png "Income Popularity Relationship: All Films")

![alt text](https://github.com/emel333/moovee_insights/blob/master/popularity%20score%20boxplot.png "Popularity Score Distribution")


### How do films where the original language is not English fare, and what's their comparison to films whose original language is English?

Japanese films consistently proved to bring in the second-most earnings of films based on the film's original language (English was consistently the first). Moreover, it was discovered that films which have English as their original language bring in considerably more earnings when there are addiitonal languages spoken in the film. I recommend producing films which have at least 4 spoken languages.

![alt text](https://github.com/emel333/moovee_insights/blob/master/gross%20income%20per%20original%20language.png "Gross Income Per Film's Original Language")

![alt text](https://github.com/emel333/moovee_insights/blob/master/number%20of%20languages%20spoken%20gross%20income.png "Gross Income Per Original Language of Films")


### How significant is it for a film to be apart of a collection?

It turned out that films apart of collections accounted for more than 65% of gross income for each selection of 1000 random titles via TMDb. Particularly, films which had English as their original language <b>AND</b> were apart of collections brought in nearly $350 Million USD in gross earnings, while the gross income for all films combined whose original language was English amounted to less than $200 Million USD, showing that films both apart of collections and with English as their original language are, altogether, better for the bottom line. I recommend analyzing the conceptual linkages between film collections and series (those with multiple seasons, i.e. GOT), as this could represent a viable direction.

![alt text](https://github.com/emel333/moovee_insights/blob/master/gross%20income%20per%20language%20films%20apart%20of%20collections.png "Gross Income Per Language: Films Apart of Collections")


# Final Recommendations + Further Research:
Overall, I recommend the following:

<ol>
    <li>Produce films within Action, Adventure, Drama or Thriller genres with the plan or flexibility to build out <i>collections</i> unique to Microsoft's online movie studio platform.</li>
    <li>Produce films which have at least 4 different spoken languages.</li>
    <li>Produce films whose original language is either English or Japanese.</li>
    <li>Consider an exclusive partnership with one or more of the top 20 production companies listed above.</li>
    <li>Explore the common thread (to viewers) between movies apart of collections and productions apart of series.</li>
</ol>