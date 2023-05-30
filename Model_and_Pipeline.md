## Data Models and Pipelines

#### Data Model
: Show how data is organized and related to each other

#### Dimentional model
Fact - Dimention : Provide details for the Fact
And <strong>Attribute</strong> provides details for a Dimention

#### Schema 
is a output product after the modeling
- Star schema
![ADOdTP8WRAKHyHKl2QS14A_997c1cb1b57e40969848c1ee1b0275f1_Screen-Shot-2022-12-21-at-12 43 34-PM](https://github.com/yinlongTh/Google_BI/assets/108507768/dacbf2fc-6618-459a-a8e0-0930c3bbe8d4)
- Snowflake schema
![9EHB99ggRZ-jcYUuR7TCrw_6bf720e4e1484544bba3c40294ccedf1_Screen-Shot-2022-12-21-at-12 45 32-PM](https://github.com/yinlongTh/Google_BI/assets/108507768/bd8836d7-7784-4408-a257-3b1ec41642c6)

And others, Unstructured, Flat, Doc, Key-value etc.

#### Database types
- OLTP 
- OLAP
- Row-based
- columnar
- Distributed
- Single-homed
- Separated storage and compute | combined

#### Database choosing Consider
- Business needs
- Seize and type of data
- Data model

Case Study with using GCP
<pre>
Previously, you started exploring Google Dataflow, a Google Cloud Platform (GCP) tool that reads data from the source, transforms it, and writes it in the destination location. In this lesson, you will begin working with another GCP data-processing tool: BigQuery. As you may recall from the Google Data Analytics Certificate, BigQuery is a data warehouse used to query and filter large datasets, aggregate results, and perform complex operations.

As a business intelligence (BI) professional, you will need to gather and organize data from stakeholders across multiple teams. BigQuery allows you to merge data from multiple sources into a target table. The target table can then be turned into a dashboard, which makes the data easier for stakeholders to understand and analyze. In this reading, you will review a scenario in which a BI professional uses BigQuery to merge data from multiple stakeholders in order to answer important business questions.

The problem : 
Consider a scenario in which a BI professional, Aviva, is working for a fictitious coffee shop chain. Each year, the cafes offer a variety of seasonal menu items. Company leaders are interested in identifying the most popular and profitable items on their seasonal menus so that they can make more confident decisions about pricing; strategic promotion; and retaining, expanding, or discontinuing menu items.

The solution :
- Data extraction
In order to obtain the information the stakeholders are interested in, Aviva begins extracting the data. The data extraction process includes locating and identifying relevant data, then preparing it to be transformed and loaded. To identify the necessary data, Aviva implements the following strategies:

- Meet with key stakeholders
Aviva leads a workshop with stakeholders to identify their objectives. During this workshop, she asks stakeholders questions to learn about their needs:

= What information needs to be obtained from the data (for instance, performance of different menu items at different restaurant locations)?

= What specific metrics should be measured (sales metrics, marketing metrics, product performance metrics)?

= What sources of data should be used (sales numbers, customer feedback, point of sales)?

= Who needs access to this data (management, market analysts)?

= How will key stakeholders use this data (for example, to determine which items to include on upcoming menus, make pricing decisions)?

Observe teams in action :
Aviva also spends time observing the stakeholders at work and asking them questions about what they’re doing and why. This helps her connect the goals of the project with the organization’s larger initiatives. During these observations, she asks questions about why certain information and activities are important for the organization.

Organize data in BigQuery :
Once Aviva has completed the data extraction process, she transforms the data she’s gathered from different stakeholders and loads it into BigQuery. Then she uses BigQuery to design a target table to organize the data. The target table helps Aviva unify the data. She then uses the target table to develop a final dashboard for stakeholders to review. 

The results :
When stakeholders review the dashboard, they are able to identify several key findings about the popularity and profitability of items on their seasonal menus. For example, the data indicates that many peppermint-based products on their menus have decreased in popularity over the past few years, while cinnamon-based products have increased in popularity. This finding leads stakeholders to decide to retire three of their peppermint-based drinks and bakery items. They also decide to add a selection of new cinnamon-based offerings and launch a campaign to promote these items. 

Key findings :
Organizing data from multiple sources in a tool like BigQuery allows BI professionals to find answers to business questions. Consolidating the data in a target table also makes it easier to develop a dashboard for stakeholders to review. When stakeholders can access and understand the data, they can make more informed decisions about how to improve services or products and take advantage of new opportunities. 
</pre>

Case study: Wayfair - Working with stakeholders to create a pipeline
<pre>
Working with stakeholders while designing and iterating on a pipeline system is an important strategy for ensuring that the BI systems you put in place answer their business needs. In this case study, you’ll discover how the BI team at e-commerce home retailer Wayfair, headquartered in Boston, Massachusetts, works with their stakeholders throughout a project to create a pipeline system that works for them.

Company background :
Longtime friends Niraj Shah and Steve Conine started the online-only company in 2002 after deciding they wanted to offer a larger selection of choices to customers—more than could fit in a brick-and-mortar space. They started the company as a collection of more than 200 e-commerce stores, each selling separate categories of products. In 2011, the company combined these sites to establish wayfair.com.

Wayfair founders, Niraj Shah and Steve Connie :
Wayfair is now one of the world’s largest home retailers. The company’s goal is to help everyone, anywhere, create their feeling of home. It empowers customers to create spaces that reflect who they are, what they need, and what they value.


The challenge :
The Wayfair pricing ecosystem includes thousands of different inputs and outputs across a full catalog of products, which change multiple times a day. All of these inputs and outputs are being generated in different ways from different sources. Because of this, the BI team and other data professionals who needed to access pricing data were having trouble locating, querying, and interpreting the complete dataset. This led to incomplete and often inaccurate insights that weren’t useful for decision makers. 

To address this, the BI team decided to design and implement a new pipeline system to consolidate all the data stakeholders needed. They also needed to consider a few additional challenges with their pipeline system:

- Monitoring and reporting around these processes would need to be included in the design to track and manage errors.

- Data would need to be clean before it could be shared with downstream users. 

- Due to the variety of data types being joined, the BI team also needed to better understand the data relationships so they could accurately consolidate the data. 

- Training sessions would be required to help educate users on how to best access and use the new datasets. 

- These unique challenges meant that it was especially important for the BI team to work closely with stakeholders while developing their new system to address their needs and create something that worked across multiple teams. 

The approach :
Given the massive amount of data within the system, it was important for the BI team to step back and work with stakeholders to really understand how they were using the data currently. That included understanding the business problems they were trying to solve, the data they were already using and how they were accessing it, and the data they wanted to use but couldn’t access yet. 

Once they had communicated with stakeholders, the team was able to design a pipeline that achieved three key goals:

All the required data could be made available and easy to understand and use

The system was more efficient and could make data available without delays

The system was designed to scale as the dataset expanded vertically and horizontally to support future growth

After this initial design was completed, the system was presented to stakeholders for review to ensure they understood the system and that it met all of their needs. This project required collaboration across a variety of stakeholders and teams:

Software engineers: The software engineer team were the primary owners and generators of data, so they were key to understanding the current state of the data and helped make it accessible for the BI team to work with.

Data architects: The BI team consulted with data architects to ensure that the pipeline design was all-encompassing, efficient, and scalable so the BI team could handle the amount of data being ingested by the system and ensure that downstream users would have access to the data as the system was being scaled. 

Data professionals: As the core users, these teams provided the use cases and requirements for the system so that the BI team could ensure that the pipeline addressed their needs. Because each of their respective teams’ needs were different, it was important to ensure the system design and data included was wide enough to account for allof those needs. 

Business stakeholders: As the end users of the insights generated by the entire pipeline, the business stakeholders ensured all development work and use cases were rooted with clear business problems to ensure what the BI team built could be immediately applied to their work. 

Communicating with all of the stakeholders throughout the design process ensured that the Wayfair BI team created something useful and long-lasting for their organization.

The results :
The final pipeline that the BI team implemented achieved a variety of key goals for the entire organization:

- It enabled software engineering teams to publish data in real-time for the BI team to use.

- It consolidated the different data components into one unified dataset for ease of access and use.

- It allowed the BI team to store different data components in their own individual staging layers.

- It included additional processes to monitor and report on the system’s performance to inform users where failures were occurring and enable quick fixes.

- It created a unified dataset that users could leverage to build metrics and report on data.

The greatest benefit of this pipeline solution was that Wayfair now had the ability to provide accurate information in one place for users, eliminating the need to join different sources themselves. This meant that the team could promote more accurate insights for stakeholders and get rid of costly ad-hoc processes. 

The response cross-team was very positive. The director of analytics at Wayfair said that this was revolutionary for their team’s daily work because they had information on retail price, cost inputs, and product status in the same place for the first time. This was a huge benefit for their processes and to help them handle their data in a more intelligent way. 

Conclusion :
A significant benefit that business intelligence provides an organization is that it makes the systems and processes more efficient and effective for users across the organization; basically, BI makes everyone’s jobs a little easier. Ensuring that the BI team is tightly aligned with the business stakeholders and other teams is critical to their success. Without great partnership, problems can’t be solved correctly. 
</pre>



