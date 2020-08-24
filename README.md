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

I decided to gain insights on production companies first and foremost because I saw this as the position Microsoft would be taking by starting this new business segment, and ultimately, wanted to discover the companies which had picked the "winners" so to speak. To this end, I used the Budget and Revenue columns to create a new column for Gross Income. I also focused on films released in the last 36 months to account for market changes. What I found is that Walt Disney Pictures stands head and shoulders above the rest, at more than $11.5B USD. The recommendation is to focus significantly on the top 20 production companies' film choices.
    


## Is there a positive correlation between popularity and income?

With films released in the last 36 months, and whether for the "bottom-earners" or all earners, there is a positive correlation. However, an interesting insight is that the majority of films did <b>not</b> have a high popularity score, as shown by the chart below with the boxplot. Nevertheless, it's quite possible to have a successful film income-wise without achieving a high popularity score. When benchmarking films, I recommend focusing on films that have a populariry score between 20-40.



## Is there a significance to the number of languages spoken in films?

Films whose original language is English brought in the most gross income among films released in the last 36 months. An interesting insight found is that films which have English as the original languages and have more than 3 languages spoken in the film provded to bring in more gross income than those with 1 or 2 total languages spoken. I recommend focusing on films where more than 4 languages are spoken.



## Which non-English films are the most popular?

Among the non-English films that brought in the most gross-income, it was films with their original language as Japanese that performed the best. I recommend focusing on films with original language in either Japanese or Korean.



## How do films apart of collections fare?

Gross income performance for films with original language as English proved much better than gross income for all films. Films apart of collections accounted for more than 65% of gross income for all films. 



## Final Recommendations

Overall, I recommend focusing largely on films whose original language is English but are potentially appealing to a wider market by having at least 4 other languages spoken in the film. I'd also recommend sourcing for scripts / movie ideas that have sequels or more future films in serious mind. Focusing on the Drama, Action and Adventure genres generally is recommended as well, and benchmarking movie streaming production according to the top 20 production companies is advised as well. Further research into how film popularity, vote counts and more are valuable as they relate to time viewers remain with a streaming platform would be a solid angle to investigate further.