# practical-application-5.1
## Description
Imagine driving through town and a coupon is delivered to your cell phone for a restaurant near where you are driving. Would you accept that coupon and take a short detour to the restaurant? Would you accept the coupon but use it on a subsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaurant? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day? Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

The data is from the UCI Machine Learning Repository and was collected via a survey on Amazon Mechanical Turk. The survey describes data different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. There are five different types of coupons -- less expensive restaurants (under 20), coffee houses, carry out & take away, bar, and more expensive restaurants.  The goal of is to distinguish between customers who accepted a driving coupon versus those that did not.

## Analysis Summary
The analysis show that:
- Only 56.84% of coupons were accepted
- The analysis looked deeper into the drivers who go to bars:
    - 41% of bar coupons were accepted.  Which is lower than the overall coupon acceptance rate of 56.8%. 
    - Those who go to bars 3 times or fewer have acceptance rate of 37.1%. However, those who go more than 3 times have higher acceptance rate of 76.9%.      Therefore the previous bar going behavior is a strong predictor of bar coupon acceptance.
    - Those drivers who go to bars more than once a month and are older than 25 years, have 69.5% acceptance rate.
    - Those drivers who go to bars more than once a month and don't have kids as passangers and have occupations other than farming, fishing, or forestry have acceptance rate of 71.3%. So this group accepts coupons at a lot higher rate than others.
- For the category of:
    - Those drivers who go to bars more than once a month, had passengers that were not a kid, and were not widowed have acceptance rate of 68.3%
    - Those drivers who go to bars more than once a month and are under the age of 30 have acceptance rate of 70.7%
    - Those drivers who go to cheap restaurants more than 4 times a month and income is less than 50K have acceptance rate of 45.3%
    - Others have accepatance rate of 29.8%

## Conclusion:
This analysis concludes factors such as:
- Age: Younger drivers (under 30) who frequently visit bars show a higher acceptance rate. This could be due to younger people generally being more socially active and more likely to visit bars
- Lifestyle: People who already go to bars more than once a month and don't have kids as passengers are more likely to accept bar coupons
- Income: Those who frequently visit cheaper restaurants and have lower income also show higher acceptance rates. This could be due to price sensitivity and deal-seeking behavior influences coupon acceptance
- Marital status: Non-widowed status combined with frequent bar visits correlates with higher acceptance. This could indicate that social factors and relationship status influence bar-going behavior

The strongest predictors of bar coupon acceptance appear to be: Existing bar-going frequency, Younger age, Social factors (no kids as passengers, not widowed), Price sensitivity.  Therefore targeting bar coupons to younger, socially active who already frequent bars and are price-conscious could yield the highest acceptance rate

