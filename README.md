# marketmindz campaign perfomance

## Project Overview

This documentation outlines the development of a Power BI reporting tool for MarketMindz, a market research firm collaborating with a small retail vendor in the food and beverage sector. The primary goal is to create a Business Intelligence (BI) solution that provides insights into marketing campaign performance, product performance, customer demographics, and the factors influencing campaign success.

## Problem Statement

The client is a small company that is still in the process of understanding its market and evaluating its customer base. They require a BI tool to gain insights from their marketing data, focusing on the following business requirements:

1. How are our six recent marketing campaigns performing?
2. How are our products performing?![Market minds campaign perfomance](https://github.com/user-attachments/assets/65eb8673-bc4e-49f0-a46d-34e990f7d2b4)

3. Who are our customers?![BUYER composition analysis](https://github.com/user-attachments/assets/a08c9aba-6270-40da-ae31-f8c013cff20b)

4. What drives campaign performance and buyer decision-making?![PURCHASE drivers analysis](https://github.com/user-attachments/assets/5712ef07-34b2-45d1-a699-f1b847b1484b)

### Insights on Purchase Drivers, Campaign Performance, and Buyer Composition

### Purchase Drivers

Based on the data analysis, several key factors have influenced purchase decisions among our customers:

1. **Demographic Characteristics**:
   - **Education Level**: Most of our customers are graduates, indicating that education may correlate with purchasing power and preferences for quality products.
   - **Marital Status**: The majority of customers are married, which often influences purchasing habits toward family-oriented products.
   - **Household Composition**: With no kids at home, this demographic may focus on premium products and convenience rather than bulk purchasing.

2. **Age Factor**:
   - Sales of wine have shown a positive correlation with customer age, suggesting that older customers are more inclined to purchase alcoholic beverages, potentially for social occasions or personal enjoyment.
   - Conversely, meat sales have decreased as customers age, possibly indicating a shift toward healthier or plant-based options.

### Campaign Performance

The analysis of the six recent marketing campaigns reveals the following insights:

1. **Top-Performing Campaigns**:
   - **Campaigns 5 and 6** have generated the most sales. This success could be attributed to targeted messaging that resonates with our customer demographics (graduates and married couples).

2. **Platform Influence**:
   - The primary platform for customer engagement has been the store itself, which suggests that in-store promotions and experiences play a critical role in driving sales.
   - Strategies that enhance the in-store shopping experience may further boost campaign efficacy.

3. **Marketing Tactics**:
   - Campaigns that emphasized premium wine offerings likely appealed to older customers, contributing to increased wine sales.
   - To replicate the success of Campaigns 5 and 6, analyzing the specific tactics used (e.g., promotions, product placements) will be crucial.

### Buyer Composition

Understanding the composition of our buyer base is essential for future marketing strategies:

1. **Customer Profile**:
   - The typical customer is a graduate, married, and without children at home, which shapes their purchasing preferences and behaviors.
   - This profile indicates a potential focus on products that cater to adults, such as gourmet foods and premium beverages.

2. **Sales Trends**:
   - The observed trends in wine and meat sales highlight the need for tailored marketing approaches. As customers age, they may show a preference for healthier options, prompting a potential pivot in product offerings.

### Strategic Recommendations

1. **Targeted Marketing**: Develop campaigns specifically aimed at older, married graduates, promoting products that align with their lifestyle and preferences.
2. **Product Diversification**: Consider expanding the product range to include more health-conscious options, especially as the customer base ages.
3. **Enhanced In-Store Experiences**: Invest in enhancing the in-store experience to leverage the primary platform for engagement, ensuring that customers have compelling reasons to visit the store.

By focusing on these insights and strategies, MarketMindz can optimize future marketing efforts and better meet the needs of their evolving customer base.

## Proposed Solution

To address these requirements, we propose developing a Power BI report that connects to a star schema database. This solution will enable the client to visualize and explore their data interactively.

### Key Features

1. **Data Visualizations**: 
   - Utilize a variety of Power BI visualizations such as charts, cards, and key influencers visuals to effectively display data insights.

2. **Interactive Filters**:
   - Implement visual filters including slicers and dropdowns to allow users to explore data by Campaign, Product, and Customer ID.

### Architectural Design - Star Schema![Star Schema](https://github.com/user-attachments/assets/3bf18b42-d65e-459f-850b-16194c30501f)


The star schema design will consist of the following components:

#### Fact Table

- **Fact Table**: This table will capture quantitative data points, including:
  - **Income**: Total revenue generated.
  - **Accepted Campaigns**: Number of campaigns that received positive responses.
  - **Age**: Age metrics of customers or campaign duration.

#### Dimension Tables

1. **Campaign Dimension**:
   - **Accepted_Ind**: Indicator of campaign acceptance.
   - **Campaign**: Name of the marketing campaign.
   - **ID**: Unique identifier for each campaign.

2. **Platform Dimension**:
   - **ID**: Unique identifier for the platform used.
   - **Platform**: Name of the platform (e.g., social media, email).
   - **Quantity**: Number of interactions or engagements per platform.

3. **Products Dimension**:
   - **ID**: Unique identifier for each product.
   - **Product**: Name of the product.
   - **Total Sales**: Total sales figures for each product.

## Business Metrics

To ensure the solution meets stakeholders' expectations, we will focus on the following key business metrics:

- **Campaign ROI**: Return on investment for each marketing campaign, calculated as (Revenue - Cost) / Cost.
- **Customer Acquisition Cost (CAC)**: Total marketing costs divided by the number of new customers acquired.
- **Sales Performance**: Total sales per product, highlighting top-performing items.
- **Customer Segmentation**: Analysis of customer demographics, including age groups, to tailor marketing strategies.

## Tools Used

- **Power BI Desktop**: This tool will be utilized for creating the Power BI report and establishing a connection with the star schema database. It offers robust features for data transformation, visualization, and sharing insights.

## Conclusion

This Power BI storytelling project aims to empower our client with actionable insights derived from their marketing data. By implementing an interactive reporting tool with a clear architectural design, we can help the client better understand their campaigns, products, and customer base, ultimately driving informed decision-making and strategic growth.
By leveraging these insights, MarketMindz can effectively guide their client toward a more data-driven marketing strategy.
