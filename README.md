# moovee_insights

Analysis of TMDb Films to discover insights and make recommendations for original movie studio business segment

---

# BIG QUESTION: 

### What strategy is best for Microsoft to employ in order to successfully launch an online streaming service?

---

<ul>
    <li>Which production companies have been involved with the most recent top-earning films?</li>
    <li>Is there a positive correlation between popularity and income?</li>
    <li>Which non-English films (films where English isn't the original language) are the most popular?</li>
    <li>How do films apart of collections compare to films that aren't apart of collections?</li>
</ul>


# Process & Tools Used

---

<ol>
    <li>Researched the length of time it takes to go from a flim's first announcement to the release date</li>
    <li>Scraped TMDb using TMDb Wrapper API to gather data</li>
    <li>Retrieved 1000/3000 movie IDs by querying the <i>popular</i> filter of the TMDb wrapper</li>
    <li>Used these IDs to query <i>Movie.info()</i> via the TMDb wrapper which gave me a fuller set of information for each film</li>
    <li>Leveraged Budget and Revenue to create a new column for Gross Income, which was used for multiple questions</li>
    <li>Created visualizations using Seaborn to discover interesting insights</li>
</ol>


# Findings

---

## Which production companies serve as the best benchmarks for Microsoft?

I decided to gain insights on production companies first and foremost because I saw this as the position Microsoft would be taking by starting this new business segment, and ultimately, wanted to discover the companies which had picked the "winners" so to speak. To this end, I used the Budget and Revenue columns to create a new column for Gross Income. I also focused on films released in the last 36 months to account for market changes. What I found is that Walt Disney Pictures stands head and shoulders above the rest, at more than $11.5B USD.
    

![Top 20 Production Companies](https://github.com/emel333/moovee_insights/production_companies_top_20.png)

