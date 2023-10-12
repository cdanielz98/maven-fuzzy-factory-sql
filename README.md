<h1><a href="#">&#x200B;</a>SQL Project- Maven Fuzzy Factory</h1>
A course-based project split into two parts.

<h2><a href="#">&#x200B;</a>The Situation</h2>
You've just been hired as an eCommerce Database Analyst for Maven Fuzzy Factory, an online retailer which has just launched their first product.
<h2><a href="#">&#x200B;</a>The Brief</h2>
As a member of the startup team, you will work with the CEO, the Marketing Director, and the Website Manager to help steer the business.
You will analyse and optimise marketing channels, measure and test website conversion performance, and use data to understand the impact if new product launches.

<h2><a href="#">&#x200B;</a>Part 1</h2>

<h3><a href="#">&#x200B;</a>1. Gsearch seems to the the biggest driver of our business. Could you pull monthly trends for gsearch sessions and orders so that we can showcase the growth there?

![test](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/7ec26085-5c1e-43b5-af47-fa1557c52e2d)
>Both sessions and orders have been increasing monthly.
<br>
<br>
2. Next, it would be great to see a similar monthly trend for Gsearch, but this time splitting out nonbrand and brand campaigns separately. I am wondering if brand is picking up at all. If so, this is a good story to tell.

![2](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/fb1bb1be-485d-4f04-b246-7ea1dd217711)

>Nonbrand campaigns are bringing in significantly more sessions and orders than brand campaigns.
<br>
<br>

3. While we're on Gsearch, could you dive into nonbrand and pull monthly sessions and device type? I want to show the board we really know our traffic sources.

![3](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/a8307e9b-e420-4dee-ba61-b5413c5bda23)

>There were far more desktop sessions than mobile sessions, and number of sessions from both device types increased monthly.
<br>
<br>

4. I'm worried that one of our more pessimistic board members may be concerned about the large % traffic from Gsearch. Can you pull monthly trends for Gsearch, alongside monthly trends for each other channel?

![4](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/6527d2e7-342b-4a9c-9ef2-8defff6fd3b1)
<br>
<br>

5. I'd like to tell the story of our website performance improvements over the course of the first 8 months. Could you pull session to order conversion rates, by month?

![5](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/17759ffb-356e-4726-b15f-0355228fee8d)

>There is a steady increase in session to order conversion rates since it began 8 months ago.
<br>
<br>
6. For Gsearch lander test, please estimate the revenue that test earned us. lander test: (Jun 19-Jul 28).

![6](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/fd4efe9f-8708-4436-a0cb-3d80a5dd688e)

>* '/home' conversion rate = 0.0318<br>
>* '/lander-1' conversion rate = 0.0406<br>
>* a difference in conversion rate of 0.0088 (an additional 0.0088 orders per session with new lander page)

![6 2](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/fa792353-936a-41d1-b77d-ff6b976ce79f)


>* 22972 sessions since the test ended<br>
>* 22972 * 00.0088 = roughly 202 extra orders since the test ended on 2012-07-28<br>
>* which is almost a difference of 4 months so:<br>
>* 202/4 = about 50 extra orders a month since before test
<br>
<br>
7. For the landing page test you analyzed previously, it would be great to show a full conversion frunnel from each of the two pages to orders. You can use the same time period you analyzed last time (Jun 19 - Jul 28).

![7](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/1291ba14-8ab6-4828-8901-f815634afa15)

>* 'thankyou_clickthrough_rate' corresponds to the rate of users that clicked on to the 'thank-you-for-your-order-page' from the previous page (billing page).<br>
>* thankyou_clickthrough rate for:<br>
>* /home = 0.4286<br>
>* /lander-1 = 0.4772<br>
>* There were 5% more completed orders in the 'lander-1' condition compared to the '/home' condition.
<br>
<br>

8. Quantify the impact of our billing test. Analyze the lift generated from the test (Sep 10 - Nov 10), in terms of revenue per billing page session, and then pull the number of billing page sessions for the past month to understand monthly impact.

![8](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/581cee23-fb57-40b6-9b55-91b3a2a2ac44)

>* '/billing-2' refers to the new billing page being tested, and '/billing' refers to the original billing page<br>
>* revenue_per_session for billing = 22.826 USD<br>
>* revenue_per_session for billing-2 = 31.311 USD<br>
>* *LIFT= 8.486 USD per billing page view*

![8 2](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/4e50aec4-b50e-4c65-a4e1-d94025ed9ce1)

* >1193 sessions in last month<br>
* >LIFT= 8.486 USD per billing page view<br>
* >*IMPACT OF BILLING TEST IN LAST MONTH: $10123.80*



<h2><a href="#">&#x200B;</a>Part 2</h2>
<h2><a href="#">&#x200B;</a>The Situation</h2>
(Dated: 20.03.2015)
Cindy is close to securing Maven Fuzzy Factory's next round of funding, and she needs your help to tell a compelling story to investors. You'll need to pull the relevant data, and help your CEO craft a story about a data-driven company that has been producing rapid growth.
<br>
<br>
<h3><a href="#">&#x200B;</a>
1.Task 1:<br>
First, I'd like to show our volume growth. Can you pull overall session and order volume, trended by quarter for the life of the business? Since the most recent quarter is incomplete, you can decide how to handle it.
![T1](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/25aded98-d856-42e0-bd85-c981d51a6368)
> A steady increase in sessions and order volume by quarter for the life of the business.
<br>
<br>

Task 2:<br>
Next, let's showcase all of our efficiency improvements. I would love to show quarterly figures since we launched, for session-to-order conversion rate, revenue per order, and revenue per session.
![T2](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/3665d1a5-d718-41e1-ae0a-acfe1039f509)
>Improvements in all areas: session to order conversion rates, revenue per order, and revenue per session, quarterly for the life of the business.
<br>
<br>
Task 3:<br>
I'd like to show how we've grown specific channels. Could you pull a quarterly view of orders from Gsearch nonbrand, Bsearch nonbrand, brand search overall, organic search, and direct type-in?
![T3](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/57e7c82e-4b79-4fcd-b454-0392bea832b0)
>A steady increase in orders from all channels. Note: importantly, an increase in orders from direct type-ins and organic search as more people become aware of our brand.
<br>
<br>
Task 4:<br>
Next, let's show the overall session-to-order conversion rate trends for those same channels, by quarter. Please also make a note of any periods where we made major improvements or optimizations.
![T4](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/930d27f9-319d-4399-8036-741d50dbd78c)
> There has been an overall increase in conversion rate across all channels.
> We can also see a slight increase in conversion rates across all channels in the first quarter of 2013, which coincides with the launch of our second product.
<br>
<br>
Task 5:<br>
We've come a long way since the days of selling a single product. Let's pull monthly trending for revenue and margin by product, along with total revenue and margin. Note anything you notice about seasonality.
![T5](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/b9c791e9-8446-47d7-8904-4942c84f3c4e)
>Monthly, revenue and margin increases for all products, consequently there is also an increase in total revenue and margin.<br>
>Regarding seasonality, there is a distinct spike in revenue every November and December which could link to increases in sales during Black Friday and Christmas.
<br>
<br>
Task 6:<br>
Let's dive deeper into the impact of introducing new products. Please pull monthly sessions to the /products page, and show how the clickthrough rates to another page have changed over time, along with a view of how conversion from /products to placing an order has improved.
![T6](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/a90debe7-71d4-414b-b579-afdfb90c5178)
>There is a steady increase in sessions clicking through from the products page, and products to order conversion rates over the life of the business.
<br>
<br>
Task 7:<br>
We made our 4th product available as a primary product on December 05, 2014 (it was previously only a cross-sell item). Could you pull sales data since then, and show how well each product cross-sells from one another?
![T7](https://github.com/cdanielz98/maven-fuzzy-factory-sql/assets/135237144/968d5aee-e818-470e-aef3-984274d74ae4)
>Product 4 had the highest cross selling rate across all other primary products, upon further investigation this may be because it was cheaper than all other products making it an easy add-on.
<br>
<br>
Task 8:<br>
In addition to telling investors about what we've already achieved, let's show them that we still have plenty of gas in the tank. Based on all the analysis you've done, could you share some recommendations and opportunities for us going forward?
>As previously mentioned, many users added product 4 on to their orders and it was an effective cross-sell product.<br>
>It may be worth looking into adding similar products that also have lower price points and see if these are effective.<br>
<br>
>Also the 'gsearch_nonbrand' channel brings in a lot of traffic to the website, it may be worth looking into increasing the bids for this channel.
