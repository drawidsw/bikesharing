# Overview

In this exercise, bike rental data from a company in New York city is analyzed in Tableau to answer questions such as:
* Who are the main subscribers
* What times are bikes rented out the most
* What locations are bikes rented out the most
* Which bikes are rented out the used the most
* How many times on average are bikes rented out
* What is the average trip duration of the bike rental
* What is the breakdown of the subscribers based upon gender and age

This data will be analyzed and presented to the investors for an investment opportunity in the bike rental company. The company must prove it can operationalize and analyze this data to make bikes efficiently available where and when they are needed, and that the bikes are routinely maintained and repaired. This way, the company can maximize its revenue and thereby its profit while increasing the scale of bike rentals even more.

# Results

The following seven results are presented to the investors.

| Number | Description | Link | 
| ------ | ----------- |------|
| 1 | There are 1.9M subscribers and only 443K one-off customers. This bodes well for the company as an overwhelming majority (78%) of its base is that of regular subscribers.  | [Subscribers vs Customers](https://public.tableau.com/app/profile/swapna.drawid/viz/bikesharing6/Sheet2) |
| 2 | The company can accurately keep track of number of bikes rented out at each location. For example, the top rental location is 195 Broadway (40.7115, -74.0132). | [Start Times](https://public.tableau.com/app/profile/swapna.drawid/viz/bikesharing7/Sheet3) |
| 3 | The company can accurately measure checkout times for bikes. Most bikes are checked out in the first few mins. after midnight - this shows an automated system is in place to check the bikes out for users and reserve specific bikes for them. This bodes well for the company.  | [Checkout Times](https://public.tableau.com/app/profile/swapna.drawid/viz/bikesharing1_16272673287700/CheckoutTimesforUsers) |
| 4 | An overwhelming majority of customers are males. This data is important to mine so that the company can make bikes available proportionately for each gender. | [Checkout Times by Gender](https://public.tableau.com/app/profile/swapna.drawid/viz/bikesharing2_16272673736050/CheckoutTimesbyGender) |
| 5 | Popular checkout times during weekdays are 8 AM in the morning and 5-6 PM in the evenings. Thursday evenings are peak checkout times for the week. For Saturdays, checkouts are evenly distributed most of the day. This kind of data is important to analyze so bikes can be provisioned accordingly to meet peak checkout demand. | [Checkout Times by Hour](https://public.tableau.com/app/profile/swapna.drawid/viz/bikesharing3/Sheet3) |
| 6 | Among the genders, the checkout patterns hold. The peak checkout times are the same for all genders. | [Checkout Times by Hour by Gender](https://public.tableau.com/app/profile/swapna.drawid/viz/bikesharing4/Sheet4) |
| 7 | Male subscribers by far outnumber all other user types. Their demand peaks at Thursdays. | [User Trips by Gender](https://public.tableau.com/app/profile/swapna.drawid/viz/bikesharing4/Sheet4) |


# Conclusions and Future Work

The company looks promosing to the investors.
* An overwhelming majority of its users are that of subscribers. The company also has an automated system in place to check bikes out for its subscribers are reserve them.
* The company has the ability to track where and when most bikes are rented out and who rents them out. This helps them in provision enough bikes to meet peak demand.
* Overall for the month of August, over 2.4M bikes are rented out. Assuming $5 per rental, this translates to $12M revenue for the month of August.

There is some future work that needs to be done.

* We expect bike rentals will peak in August as it is the last month of summer. We need bike rental data for all 12 months, expecially in the winter months to get a true picture of annual revenues. We expect bike rentals will dip in the peak winter months of December - February.
  * A simple visualization here is to show bike rentals per month - this can be done by adding the **month as a measure**, bike rentals in **size** of the **marks** sections and showing the data as a **bar chart**.
* We would also like to get an estimate of average trip duration breakdown by gender to see if the bike usage pattern differs among genders. For this, we would like to get average measure of trip broken down by genders. A possible visualization for this is to select the **Tripduration (avegare)** as the measure and the **gender** as a **label mark**. Since we will get only three values, any visualization will work; the circle visualization will work better where the size of the circle corresponds to the average of each gender. In fact, this visualization is [here](https://public.tableau.com/app/profile/swapna.drawid/viz/bikesharing8/Sheet1).
