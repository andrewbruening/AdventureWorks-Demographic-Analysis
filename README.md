### Hey! I'm Andrew. Welcome to my [Github] 👋

- 📊 Data visualization is my forte. See my [Tableau] page! 
- 🚀 Most of what you see here is Tableau, Python, SQL, and Figma
- 🧠 I'm interested in how our social climate and media trends influence BI decisions
- ⛳ A nice quote: "If it's worth doing, it's worth doing well"

## Adventure Works Cycles: Demographic Analysis
**AdventureWorks is a Microsoft product sample for an online transaction processing (OLTP) [database].**
 
![](Dashboard_Screenshots/dash.png)
 
This readme includes various screenshots, but you can view the actual dashboard [here]


## Approach
1. The pyodbc package was used to connect to the AdventureWorks database and query in python. 
2. Since we'll be importing our data to Tableau, it's in our best interests to work from one large dataframe. This isn't always possible, but we can take advantage of the opportunity here with **'custdf'**
3. There wasn't much cleaning to be done, but I did need to convert the **BirthDate** column to a brand new **Age** column. I wrote a custom function and used the difference between today's date and BirthDate to make Age.
4. A few dashboard elements were designed in Figma, then everything was imported to Tableau for dashboard creation. 
5. The complete [dashboard] features hover tooltips on most graphics and text boxes.
 
![](Dashboard_Screenshots/tooltip_gif.gif)


## Data Insights
**Demographics:** Our analysis points to a predominantly family-focused, upper middle class population who are likely to have multiple children and live in the Pacific Northwest. Genders are equally represented, slightly favoring married couples, and strongly favoring a college education.

**Location:** Destination-specific content can be A/B tested on the creative level.

    1. Imagery featuring recognizable locations may pique the interest of top-of-funnel colder customers (Crissy Field, Mount Rainier, etc.)

    2. PNW cities like San Francisco, Portland, and Vancouver are known to be well-traveled by commuters riding bikes to-and-from work, which surely makes up a considerable portion of Road Bike and Touring Bike purchases.

    3. The Seattle to Portland (STP) Bicycle Classic is one of the largest recreational bike rides in the country. Each year, thousands of riders participate in this multi-day event. With 77% of our customers in the PNW, the STP poses a potential partnership opportunity, or at the very least, viable inspiration for advertisements.

**Age:** The age range of 40-65 is particularly responsive to Facebook Ads but is most likely not using TikTok or Instagram. In order to target this population properly via Facebook:

    1. Create 1-2% lookalike audiences via Facebook Ads from an email list, or from the followers of competitors like REI, MEC, and Cannondale. 

    2. These audiences should match at least 1000 people in the market, and be combined with detailed targeting on the ad set level for use in Messages or Lead Generation campaigns.

    3. A/B test on the creative level with casual family-oriented biking imagery and copy. 

    4. These will be top-of-funnel campaigns, so cost will be measured based on CPM.

**Sales History:** While 77% own cars, car ownership and bike ownership are not mutually exclusive, and many customers may ride bikes recreationally or for short-distance commutes.

**Income:** We know that our clientele is largely represented by individuals in the upper middle class. They make purchases not only for themselves, but for their family members as well.

• Marketing content can be primarily geared toward biking imagery with a mention of time-sensitive promotions on additional accessories, or promo codes for "afterthought" products. 

• Families may be interested in deals that include travel bike racks and group purchases.

## In Hindsight

This was an earlier project of mine. If I were to approach this project with the experience that I have now, the main difference I'd make in my actions is with the dashboard design. There are a number of ways I could go about making it more intuitive, organized, and aesthetically pleasing. For example, it would be beneficial to add separate dashboard pages or show/hide buttons to reduce clutter. This is a lot of information to squeeze into a 1600x900px space.

I've noticed that the most successful dashboards are the easiest to digest. Overall, I enjoy the monochrome color palette and the variety of graphs/charts that I included.  Marketing/BI analysts should have no problems using my dashboard. But looking back, I've realized that I've gained plenty of experience since working on this. It's been a refreshing way to take note of what I should do differently next time around.

I may revisit this in the future! If I do, I'll include before and after images.

## See the complete interactive dashboard [here]

</details>

[Tableau]: https://public.tableau.com/app/profile/andrew.bruening
[Github]: https://github.com/andrewbruening
[here]: https://public.tableau.com/views/AdventureWorks2019/NADB?:language=en-US&:display_count=n&:origin=viz_share_link
[dashboard]: https://public.tableau.com/views/AdventureWorks2019/NADB?:language=en-US&:display_count=n&:origin=viz_share_link
[database]: https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15&tabs=ssms
