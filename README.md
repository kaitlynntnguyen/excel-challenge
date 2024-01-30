# Excel Challenge

1. First, I used conditional formatting in Excel to fill cells with a different color based on `Outcome`, depending on whether the associated campaign was successful (green), failed (red), canceled (yellow), or is currently live (blue).
2. Then, I created a column called `Percent Funded` that uses formula to find how much money a campaign made relative to its initial funding goal and used conditional formatting to fill cells in `Percent Funded` in a three-color scale. Cells with a value equal to or more than 0 and less than 100 are dark red, cells with a value equal to or greater than 100 and below 200 are green, and cells with a value equal to or greater than 200 are blue.
3. I created a column called `Average Donation` to find how much each project backer paid on average. To obtain this, I looked at the acquired funding and divided it by the number of backers.


4. I created a column called `Parent Category` and another one called `Sub-category` to split the contents of the `Category and Sub-Category` column into two separate columns.

5. In another sheet, I created a pivot table to look at the number of campaigns that were failed, successful, canceled or live based on category. I created a stacked-column pivot chart that filtered the results by country based on the pivot table I created.

6. I created another sheet with a pivot table to analyze the outcome of campaigns per sub-category. Then, I created a stacked-column pivot chart that can be filtered by country and parent category based on the pivot table I created.

7. On the initial sheet I converted the `launched_at` and `deadline` columns from Unix timestamps to date format into two new columns `Date Created Conversion` and `Date Ended Conversion`. On another sheet, I created a pivot table that looked at outcome of campaigns and the date created, and filtered based on parent category and Years. I created a pivot-chart line graph to visualize the results.

8. I created a new sheet that looked at the outcome of campaigns based on the crowdfunding goals. I created a table with a `Goal` column that specified the crowdfunding goal in ranges going from `Less than 1000` to `Greater than or equal to 50000`. The table showed the number of campaigns that were successful, failed, canceled, and the total number of campaigns in each crowdfunding goal range, and calculated the percentage of campaigns with each outcome. Then, I created a line graph based on that table to visualize the results.

9. I created a new sheet that showed the successful campaigns and the number of backers, and on another column showed the failed campaigns and the number of backers. 
    - For successful campaigns, the `mean` number of backers was 851, the `median` was 201, the `minimum` was 16, the `maximum` was 7295, the `variance` was 1603374, and the `standard deviation` was 1266.
    - For failed campaigns, the `mean` number of backers was 586, the `median` was 115, the `minimum` was 0, the `maximum` was 6080, the `variance` was 921575, and the `standard deviation` was 960.
    - I concluded that the median summarizes the data better than the mean because outliers heavily skew the mean.
    - I also noted that there is more variability with successful campaigns, failed campaigns have a lower number of backers because these were campaigns that did not reach their crowdfunding goal, while successful campaigns exceeded their goal, increasing variability in the number of backers.
