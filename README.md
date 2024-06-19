# Car-Brand-Maps-
Using principal component analysis and regression to visualize brand competition 

## Data Overview 
Cars_Data.csv contains 10 car brand with raiting for attractiveness, quiet, poorly built, interesting, sporty, uncomfortable, roomy, easy service, prestige, common, economical, successful, avent garde, poor value, and overall preference. We will create a brand map to understand the competition in the market and how specifically infinity can improve their position in the market. 

## Build Brand Maps 
<img width="777" alt="Screenshot 2024-06-19 at 1 37 22 PM" src="https://github.com/lex910/Car-Brand-Maps-/assets/101606445/0c742890-c578-4d77-9889-bf9f2d991f1a">

## Determine how many factors to retain 
We will retain 2 factors. After calculating the component scores that show the coordination of brands in the map, we can create a preference regression to estimate how many benefits affect the overall performance score. The regression model shows that z1 and z3 are significant at the 0.05 significance level. Z3 appears to have a negative slope so all of the z variables will need to be multiplied by -1.

## Assign names to retained factors 
Z1(Luxury): attractive, quite, poorly built, prestige, successful (slope is positive so we don’t need to flip z-variables)
Z3 (Modest) : interesting, economical, poor.value (slope is negative so we need to flip the z variables by multiplying by -1)

## Iso preference line calculation 

Slope of iso preference line: 1.494

 Groups the list of all goods that provide the same level of satisfaction
● Built on customer preferences
● Interpretation :
  ○   Right side is more preferred
  ○   Left side is less preferred
  ○   Same line are equally preferred

## Regression line

 Used to estimate the relationship between the independent variables (X1 , X2 ..... Xn ) and the dependent variable Y
● Mainly used for predicting the values of the dependent variable when provided with the independent variables

## Ideal Vector

Slope of ideal vector: -0.669

The ideal vector is a line perpendicular to the iso-preference lines that points toward the location of higher consumer preference. The direction of the ideal vector shows where the attributes of brands increase in desirability.

## Angles of iso-preference line and ideal vector arrow 

Angle of iso preference line: 56.209
Angle of ideal vector: -33.791

## 95% CI fo the angle of the ideal vector using bootstrap methods 
2.5%          97.5%
-43.59        -22.503

## Recommendations for Infinity brand to improve product design 

From the 2 components that we honed in on, Luxury and Modest, it’s clear that Infinity is doing well on Luxury. This means their cars are viewed as both Attractive and Prestigious. However, they may have taken this angle too far, since they outpace even BMW in Luxury. This could be hurting sales as those who value Modesty are not interested since they are below market average. The highest weighted category in Modest is Economical. Our recommendation for Infinity is to focus more on improving their car’s reliability and gas mileage as these are the 2 factors that often affect consumer’s opinion of a car being Economical. A strategy that they should follow is the strategy of Lexus, who is both a Luxury brand but also widely seen as the Modest option. This will help them get greater general appeal and broaden their customer base.
