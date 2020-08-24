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

From the beginning of 2017 to the end of 2019, Walt Disney Pictures has consistently proven to be number 1 in gross earnings, via the random selection of 1000 movie titles from TMDb's <b>Popular</b> filter (conducted 7 random selections until now). What's more, a Genre Dominance query among these films showed that Action, Adventure and Drama are consistently the top genres. I recommend using the top 20 production companies as a benchmark for movie studio film production.

![alt text](https://github.com/emel333/moovee_insights/production companies top 20.png "Top 20 Top-Earning Production Companies")


### How seriously should popularity score be taken?

It's been discovered that there is, indeed, a positive correlation between popularity score and gross income. However, what's interesting is that this doesn't necessarily translate to <i>high</i> popularity scores. It is very much possible to have a high-earning film receive a seemingly mediocre or low popularity score. The Boxplot portion of the chart below shows that the majority of popularity scores for top-earning films falls within the range of 20-40. So, I don't recommend producing films according to popularity scores.


### How do films where the original language is not English fare, and what's their comparison to films whose original language is English?

Japanese films consistently proved to bring in the second-most earnings of films based on the film's original language (English was consistently the first). Moreover, it was discovered that films which have English as their original language bring in considerably more earnings when there are addiitonal languages spoken in the film. I recommend producing films which have at least 4 languages spoken.

### How significant is it for a film to be apart of a collection?

It turned out that films apart of collections accounted for more than 65% of gross income from the consistent random selection of 1000 titles via TMDb. Particularly, films which had English as their original language <b>AND</b> were apart of collections brought in nearly $350 Million USD in gross earnings, while the gross income for all films combined whose original language was English amounted to less than $200 Million USD, showing that films apart of collections are, altogether, better for the bottom line. I recommend investigating the linkages between film collection and Series with multiple seasons, as this could represent a viable direction.


# Final Recommendations + Further Research:
OVerall, I recommend the following:

<ol>
    <li>Produce films within Action, Adventure or Drama genres with the plan or flexibility to build out <i>collections</i> unique to Microsoft's online movie studio platform.</li>
    <li>Produce films which have at least 4 different languages spoken.</li>
    <li>Produce films whose original language is either English or Japanese.</li>
    <li>Consider an exclusive partnership with one or more of the top 20 production companies listed above.</li>
</ol>