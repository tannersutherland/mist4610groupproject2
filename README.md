# mist4610groupproject2

Team Name and Members:

Audrey Staples\
Angela Ren\
Tanner Sutherland\
Sam Effron\
Tyler Schildkraut

Database Description:

We chose the data model title Real Estate Sales 2001-2023 GL. Specifically, our data was collected from the state of Connecticut and we have narrowed our focus more specifically on the past decade or so of housing prices. It included exactly 1,141,722 rows of values along with 14 columns in total so we really wanted to make sure we narrowed down our filters and the scope of our analysis. The reason we chose this data set was because we were curious about trends in recent years as the housing market is always a great indicator of market health. Additionally, our data set is rich in values that people can understand. Some of the most relevant data we were able to get plenty of information on were the following: Serial Number, List Year, Town, Address, Assessed Value, Sale Amount, Sales Ratio, Property Type, and Residential Type. Other data included in the database included Date Recorded, Non Use Code, Assessor Remarks, OPM Remarks, and Location. However, we made the decision to not include analysis of these values because they were redundant, not extremely intuitive, and we found we could provide better insights using other data points specified in the model. Serial Number (whole number data type) specifies the unique label placed on each individual house in the state of Connecticut. List Year (whole number data type) specifies the year the house was listed on the market and Data Recorded (date data type) is the specific date the property was registered under a specific mortgage/deed. Town (string data type) and Address (string data type) included information about where the house was located. Assessed Value (decimal number data type) and Sales Amount (decimal number data type) allowed us to examine the difference between what the value of the house was assessed to be by appraisers versus the amount the house actually sold for on the market. The Sales Ratio (decimal number data type) provides a specific ratio that details the discrepancies between Assessed Value and Sales Amount. For example, a ratio below 1.0 would be indicative of a property being under-assessed versus a ratio above 1.00 indicating the property is being over-assessed. Property Type (string data type) indicates the specific property type (Residential, Commercial, Vacant Land, etc.). Residential Type (string data type) specifies the specific residential property type given that the property is considered Residential (Single Family, Two Family, Condo, etc.). Non-Use Code (string data type) specifies information regarding a property if it was regarded as not conforming property contractual obligations. Assessor Remarks (string data type) specifies official remarks given by a property assessor for tax purposes, and OPM Remarks (string data type) includes information regarding if a property was financed by an outside source other than the purchaser’s own funds. Lastly, Location (string data type) provides the exact GPS coordinates of a specific property.

Question 1: How did average prices across Connecticut towns change from 2018–2023, especially during and after the COVID-19 housing surge?


Explanation: We wanted to examine the periods leading up to and after the COVID-19 pandemic to examine housing trends and if we could draw any insights given the data. It is known that during the pandemic, interest rates significantly decreased which aimed to stimulate economic growth overall, subsequently spurring growth in the housing market in the process. We want to see if this would be reflected in the data we measured in Connecticut.

Manipulations:\
<img width="492" height="402" alt="Screenshot 2025-11-21 at 1 56 41 PM" src="https://github.com/user-attachments/assets/0fa6d633-2ca3-4044-a1eb-544495e2498d" />

Visualizes the full spread of price growth across all 169 Connecticut towns, providing statewide context for our analysis.\
The median CT town grew ~45%, indicating broad but moderate appreciation between 2018–2023.\
The interquartile range (IQR) shows most towns clustered between ~20% and ~70% growth, reflecting common market conditions.\
We chose the top 10 because they’re the towns with the strongest growth trends — and the statewide distribution validates that these towns truly behaved differently.”\
Several top-performing towns (highlighted in blue) stand far above the statewide distribution, with growth between 150%–325%, confirming how uneven the COVID-era surge was.\
Highlights that the top 10 fastest-growing towns experienced 3–6× the typical growth, driving much of the statewide housing boom.


<img width="538" height="474" alt="Screenshot 2025-11-21 at 1 59 53 PM" src="https://github.com/user-attachments/assets/5d6e3269-8153-4bee-9ca5-3f293b1cde79" />

Focuses on the top 10 CT towns with the highest property price growth from 2018–2023, filtered from a full dataset of 169 towns for clearer interpretation/
Reveals strong variation across high-growth towns, indicating an uneven and shifting housing landscape/
High-growth areas (e.g., Windsor, Franklin) suggest strong demand, limited inventory, or intensified COVID-era in-migration/
Helps identify which local markets experienced the sharpest heating-up trends during the 2018–2023 period

<img width="282" height="263" alt="Screenshot 2025-11-21 at 2 01 19 PM" src="https://github.com/user-attachments/assets/957eccc0-e77d-4516-878c-ca3c0c50c423" />

Visualizes year-over-year changes in average sale prices (2018–2023) for the top 10 fastest-growing CT towns, filtered from all 169 towns for clarity\
Complements the previous bar chart by revealing how and when each top-growth town experienced its appreciation\
Highlights differences in momentum: some towns show sustained multi-year acceleration, while others spike later in the period\
Helps distinguish market behavior patterns across high-growth towns (e.g., rapid post-COVID run-ups vs. steady long-term appreciation)

<img width="323" height="204" alt="Screenshot 2025-11-21 at 2 02 20 PM" src="https://github.com/user-attachments/assets/6d2c8e94-2f07-43fc-843a-a32de28bf0fd" />

Shows average sale prices in each town before COVID (2018–early 2020).\
Prices more consistent across towns.\
Only a few gaps exist between higher-value and lower-value towns.\
This period represents the baseline before the major COVID-era market surge.\

<img width="336" height="230" alt="Screenshot 2025-11-21 at 2 02 46 PM" src="https://github.com/user-attachments/assets/b657081b-70a5-480c-b72e-315226c5ce20" />

Displays average sale prices in each town after COVID began (2020–2023).\
Nearly all towns show some price increases compared to pre-COVID.\
Differences between towns become more pronounced, with some markets accelerating faster.\
Highlights the pandemic-driven demand spike that in Connecticut’s housing market.


Analysis:

Home prices rose statewide from 2018–2023, with the sharpest increases during the COVID surge (2020–2022).\
Growth was uneven, with some towns appreciating far more rapidly than others.\
Lower-priced towns (e.g., Windsor, Canaan) saw the biggest percent gains, driven by low starting prices and strong COVID-era demand.\
Higher-priced towns (e.g., Washington, Salisbury) saw large dollar gains, but smaller percent increases due to the base effect.\
Most price jumps occurred between 2020–2022, while 2023 shows mixed cooling or continued growth depending on the town.\
Overall trends reflect COVID migration, remote work, and limited inventory—especially boosting rural and mid-market towns.


Question 2: On average, have assessed values kept pace with actual sale prices from 2018–2023, and which property types show the largest valuation gaps?

Explanation: This question narrowed in on the discrepancies between sale prices and assessed values during this time. It is important to understand this question because valuation gaps can effect tax assessment, housing affordability, and local revenue planning.

Manipulations:

<img width="286" height="256" alt="Screenshot 2025-11-21 at 2 04 56 PM" src="https://github.com/user-attachments/assets/0bf390a8-f1d6-4be3-afcf-c5f16c61b811" />


This graph shows the median assessed value of real estate property based on different property types from 2018 to 2023 in Connecticut\
The property types that are included in the graph are:\
Apartment (Blue)\
Commercial (Light Blue)\
Condo (Orange)\
Four Family (Peach)\
Industrial (Green)\
Public Utility (Light Green)\
Residential (Gold)\
Single Family (Yellow)\
Three Family (Turquoise)\
Two Family (Blue-Green)\
Vacant Land (Red)


<img width="288" height="251" alt="Screenshot 2025-11-21 at 2 05 59 PM" src="https://github.com/user-attachments/assets/b24c1e4d-2bd5-4017-a997-7b9f864a5546" />

Compared to the last slide, the actual sale prices are generally higher than the assessed prices of each property\
The median assessed price for apartments is $269,613, while the actual median sale price is nearly double at $538,000\
This shows how the majority of properties are vastly undervalued from assessment date to sale date\
The only outlier within the data is in the public utility property type\
The assessed price is $69,775 while the sale price $44,500\
This is the only property that was overvalued\
The largest gap between assessed price and sale price is in the industrial property type\
The assessed price is $426,230 while the sale price is $725,000\
That’s nearly a $300,000 undervaluation\

<img width="343" height="209" alt="Screenshot 2025-11-21 at 2 06 33 PM" src="https://github.com/user-attachments/assets/4d480c2e-e5c2-48db-916f-07d7af5d7c39" />


This map plots average sales ratios for commercial sales across CT towns.\
Sales Ratio = (Assessed Value / Sale Price) — values below 1 (red) mean the town under-assessed properties.\
Most towns appear light to deep red, indicating commercial properties typically sell for more than their assessed values.\
Under-assessment is strongest in suburban and rural areas, where sale prices rose faster than assessor updates.

<img width="348" height="219" alt="Screenshot 2025-11-21 at 2 07 02 PM" src="https://github.com/user-attachments/assets/a5f8ce53-4b00-4212-b904-599e1981a66b" />


Most towns appear deep red, meaning sales ratios are well below 1 meaning residential homes are significantly under-assessed relative to their sale prices.\
Under-assessment is widespread because residential market values surged during COVID, while assessor updates lagged behind.\
Indicates strong market demand pushed residential prices far above official assessed values from 2018–2023.


Analysis:

Aside from the public utility outlier, it is safe to say that the assessed values of the real estate properties have not kept pace with the actual sale prices of those properties.\
This is likely due to the increased interest rates from the Federal Reserve which increased prices in the real estate market.\
As shown in the bar charts, the majority of average assessed prices for real estate in Connecticut from 2018-2023 were lower for property types then the actual sales price with the \public utility property type being the exception.



