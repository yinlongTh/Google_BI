## Foundations of Business Intelligence

#### Describe
<pre>
- What drives BIs bring for changes? 
</pre>

#### Example Scenarios
Scenario 1
<pre>
Topic : Restuarants reducing waste
-----------------------------------
Problems -> How to ensure the restaurants’ numerous locations have enough ingredients to meet customer demand
         -> How to reduce food waste
-----------------------------------
Data -> Customer transactions
     -> Marketing data related to promotions
     -> Customer satisfaction
     -> Employee information
-----------------------------------
Solution 
1) Set matrics 
   - How many ingredients are dilivered to each location
   - How much of each menu item is made / day
   - How much of each menu item ordered / day
2) Comparing matrices to answer the questions
3) Organize this data within database and deliver
</pre>

Scenario 2
<pre>
Topic : Hospitals promoting patient care
-----------------------------------
Problem -> Doctors outside of the system can’t access test results from the hospital
        -> Patients are being tested multiple times
-----------------------------------
Solution 
1) Multiple source systems needs to be consolidated (Prev. visit, Tests, Patients info)
2) Develop the Db system and pipeline
</pre>

#### Data Life Cycle
1. Plan
2. Capture
3. Manage
4. Analyze
5. Archive
6. Destroy

#### Data Analysis Process
1. Ask
2. Prepare
3. Process
4. Analyze
5. Share
6. Act

#### Business Intelligence Stages 
Goal : Increase <strong>Data Maturity Level</strong> 
1. Capture : What happen? - Description
2. Analyze : Why did it happen? - Diagnostic
3. Monitor : What's happening now? - Prescription & Prediction
<br>

![maturity_model](https://github.com/yinlongTh/Google_BI/assets/108507768/a28be2da-ab83-4ec0-b3f8-2b451c95b68e)

<br>

#### Key BI docs
1. Stakeholder Requirements Doc
   - Business problem
   - Stakeholder
   - Stakeholder usage details
   - Primary requirements
2. Project Requirements Doc
   - Purpose
   - Key dependencies
   - Stakeholder requirements
   - Success criteria
   - User journey <br>
   [And more](https://docs.google.com/document/d/1Vq9G_MAQRz4V6iZF_Z-v_u0AcwloB96lc6wwYzz9EDg/template/preview?pli=1)
3. [Strategy Doc](https://docs.google.com/document/d/13v9_pOAHbcv2dhEMZtPFJ6sgvZaY-9tVp1op32owAdE/template/preview)

#### Data Availability Factors
- Data integrity
- Data visibility
- Update frequency
- Change update

#### Vanity metrics
<pre>
Data points are intended to impress others, but cannot reveal any meaningful insights like the number of Twitter follower of Amazon
</pre>

#### Case Study : USDM - Selecting key project metrics
<pre> 
Company background :
USDM, headquartered in Santa Barbara, California, collaborates with life science companies across a variety of industries, including biotechnology, pharmaceutical, medical device technology, and clinical. USDM helps its customers, from large-scale companies to small businesses, ensure that their database systems are compliant with industry standards and regulations, and work effectively to meet their needs. USDM’s vision is to bring life sciences and healthcare solutions to the world better and faster—starting with its own company values: customer delight, accountability, integrity, respect, collaboration, and innovation. 

The challenge :
In this case study, you’re going to explore an example of USDM’s work with one of their clients. The client for this project researches and develops antibody treatments for cancer patients. The client needs analytics that measure the effectiveness and efficiency of their products. However, with the client’s existing database, to get the types of reports they need, they have to access many systems, including facility data, licensing information, and sales and marketing data. All of this data exists in various places, and as a result, developing analysis reports creates issues for the client’s stakeholders. Also, it makes it harder to compare key metrics because so many KPIs needed to be brought together in one place. 

To help better understand how effective their product is and forecast demand, the client asked USDM to help architect a data storage system that could address their specific needs. They needed a system that could bring the data their team needs together, follow industry regulations, and allow them to easily create reports based on key metrics that can be used to measure product effectiveness and market trends. A significant part of this initiative started with the basics: what were the actual key metrics for the client’s team and what data systems did they come from? 

The approach :
To identify which metrics were most important for the client’s business needs, the USDM team needed to get input from a variety of different people from across the organization. For example, they needed to know what charts the sales and marketing teams who used this data for their reports needed, what their existing processes were, and how to address these needs in the new system. But, they also needed to know what data the product development team used in order to measure efficacy. 

USDM worked closely with different teams to determine what charts they needed for reports, how they were accessing and using the database system currently, and what they were hoping to achieve with the new system. As a result, the team was able to determine a selection of key metrics that represented their client’s business needs. These metrics included:

- Sales performance
- Product performance
- Insurance claims
- Physician information
- Facility data

To enact a business intelligence solution there must be both the business interaction with stakeholders and the technical interaction with the architects of other team’s systems. Once these metrics were identified by the client, the USDM team collaborated with other members of the client’s team to begin building a new solution that could capture these measurements. 

But, almost every project comes with unexpected challenges; the database tool the team was using to develop the new system didn’t have all of the features the team needed to capture their must-have metrics. In this case, the USDM team collaborated with leadership to develop a list of requests from the tool vendor, who was able to address their team’s unique needs. 

The results :
By the end of the project, the USDM BI team architected a data storage system that consolidated all of the data their team needed from across a variety of sources. The system captured the key metrics the client needed to understand their product’s effectiveness, forecast sales demand, and evaluate marketing strategies. The reporting dashboards created with this data storage system included everything the stakeholders needed. By consolidating all of the KPIs in one place, the system could provide faster insights and save the client time and improve efficiency without having to run reports from every individual system. The solution was more automated and efficient—and importantly, designed specifically with their team’s most useful metrics in mind.

Conclusion :
Collaborating with users and stakeholders to select metrics early on can help determine the long-term direction of a project, the specific needs stakeholders have, and how to design BI tools to best address unique business needs. As a BI professional, a key part of your role will be considering key metrics and how to tailor the tools and systems you create to capture those measurements efficiently for reporting use.
</pre>






