# AdventureWorks-Demographic-Analysis



### Hey! I'm Andrew. Welcome to my [Github] 👋

- 📊 Data visualization is my forte. See my [Tableau] page! 
- 🚀 Most of what you see here is Tableau, Python, and Figma
- 🧠 I'm interested in how our social climate and media trends influence marketing needs
- ⛳ A nice quote: "If it's worth doing, it's worth doing well"

## Wide World Importers
**WWI is a wholesale novelty goods importer and distributor operating from the San Francisco bay area**
 
![](Dashboard_Screenshots/dash.png)
 Here's a link to the SQL [database] from Microsoft

This readme includes various screenshots, but you can view the actual dashboard [here]


## Approach
1. The pyodbc package was used to connect to the AdventureWorks database and query in python. 
2. Since we'll be importing our data to Tableau, it's in our best interests to work from one large dataframe. This isn't always possible, but we can take advantage of the opportunity here with **'custdf'**
3. There wasn't much cleaning to be done, but I did need to convert the **BirthDate** column to a brand new **Age** column. I wrote a custom function and used the difference between today's date and BirthDate to make Age.
4. Regex was implemented to standardize StockItemName in **'productdf'**, and to categorize it in **'timedf'**.
5. The two dataframes were exported from Python, a few dashboard elements were designed in Figma, then everything was imported to Tableau. 
6. The complete [dashboard] features hover tooltips on most graphics and text boxes.
 
![](Dashboard_Screenshots/tooltip_gif.gif)


## Data Insights
**Demographics**
Our analysis points to a predominantly family-focused, upper middle class population who are likely to have multiple children and live in the Pacific Northwest. Genders are equally represented, slightly favoring married couples, and strongly favoring a college education.

**Age**
The age range of 40-65 is particularly responsive to Facebook Ads but is most likely not using TikTok or Instagram. In order to target this population properly via Facebook:

    1. Create 1-2% lookalike audiences via Facebook Ads from an email list, or from the followers of competitors like REI, MEC, and Cannondale. 

    2. These audiences should match at least 1000 people in the market, and be combined with detailed targeting on the ad set level for use in Messages or Lead Generation campaigns.

    3. A/B test on the creative level with casual family-oriented biking imagery and copy. 

    4. These will be top-of-funnel campaigns, so cost will be measured based on CPM.


Sales History
While 77% own cars, car ownership and bike ownership are not mutually exclusive, and many customers may ride bikes recreationally or for short-distance commutes.
     
![](Dashboard_Screenshots/line_with_i_bubble.png)

**Income** 
We know that our clientele is largely represented by individuals in the upper middle class. They make purchases not only for themselves, but for their family members as well.

• Marketing content can be primarily geared toward biking imagery with a mention of time-sensitive promotions on additional accessories, or promo codes for "afterthought" products. 

• Families may be interested in deals that include travel bike racks and group purchases.


**Location**
Destination-specific content can be A/B tested on the creative level, for both weekend adventures and casual city commutes.

• Imagery featuring recognizable locations may pique the interest of top-of-funnel colder customers (Crissy Field, Mount Rainier, etc.)

• PNW cities like San Francisco, Portland, and Vancouver are known to be well-traveled by commuters riding bikes to-and-from work, which surely makes up a considerable portion of Road Bike and Touring Bike purchases.

• The Seattle to Portland (STP) Bicycle Classic is one of the largest recreational bike rides in the country. Each year, thousands of riders participate in this multi-day event. With 77% of our customers in the PNW, the STP poses a potential partnership opportunity, or at the very least, viable inspiration for advertisements.




- **Our contribution margins aren't contributing enough:**
    The standard markup for individual retail products is 50%. In previous years, we've exceeded that number at an average margin of 54%. In 2016, we averaged a troublesome 25%. 

    One identifiable weak point is our USB category. *(see **i bubble** on Scatter Plot Sidebar)*
    
    This raises a few questions: 
	- What was the logic behind the price point of USB products? 
	- Were they part of a promotion?
	- Was this part of a loss leader strategy?
     
![](Dashboard_Screenshots/scatter_with_i_bubble.png)
## See the complete interactive dashboard [here]

</details>

[Tableau]: https://public.tableau.com/app/profile/andrew.bruening
[Github]: https://github.com/andrewbruening
[here]: https://public.tableau.com/views/AdventureWorks2019/NADB?:language=en-US&:display_count=n&:origin=viz_share_link
[dashboard]: https://public.tableau.com/views/AdventureWorks2019/NADB?:language=en-US&:display_count=n&:origin=viz_share_link
[database]: https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15&tabs=ssms
