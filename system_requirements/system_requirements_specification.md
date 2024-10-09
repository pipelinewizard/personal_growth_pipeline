# Project Scope Document

## Project Title: Value Driven Pipeline (Azure End-to-End)

## Phase 1: Personal project (testing w/ personal data)

*Project Owner: Isaiah Donley*

### Purpose:
Build a fully automated data pipeline that aligns with my key values, managing data from multiple domains of my life such as finances, health, and family media. This pipeline will deliver insights, analysis, and predictions to support those "key values", all running end-to-end on Azure.
____________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

### Key Values and Mapped Data Domains:

**Value 1: Health & Well-being Report**
- Objective 1: Sleep [X hours] per night
- Objective 2: Workout [X minutes] per day
- Objective 3: Write in journal [X times] per week

*Mapped Domains:* Health data (e.g., Apple Watch, fitness apps), sleep data, medical records, and activity metrics.

**Value 2: Family and Relationships Report**
- Objective: Allocate Quality Time
- Objective: Capture and preserve annual family milestones and traditions

*Mapped Domains:* Media data (pictures and videos), household schedules, family event tracking, travel data, and family memory archiving.

**Value 3: Financial Stability Report**
- Objective 1: Enhance Financial Discipline and Control
    - Key Result 1: Achieve [X %] budget compliance
- Objective 2: Increase financial security and savings
    - Key Result 1: Achieve [X %] savings rate
- Objective 3: Build and grow personal wealth
    - Key Result 1: Achieve [X $] networth
- Objective 4: Improve financial literacy and investment knowledge
    - Key Results 1: Read [X #] personal finance/investment books/articles per year

*Mapped Domains:* Financial transactions, investment portfolios, online purchases, tax data, and budgeting.

**Value 4: Personal Growth Report**
Objective 1: Enhance data engineering skillset and knowledge - (Ongoing)
    - Key Result 1: Build and Complete [X #] Personal Data Engineering Projects
    - Key Result 2: Read [X #] of data engineering books/articles
    - Key Result 3: Complete [X #] certifications or courses
    - Key Result 4: Lead [X #] of organizational data engineering projects
    - Key Result 5: Build and Complete [X #] of organizational data engineering projets
    - Key Result 6: Contribute [X %] or [X $] to organizational revenue or cost savings through data engineering projects.
    - Key Result 7: Build and complete [X #] of contract data engineering projects
    - Key Result 8: Achieve a revenue of [X $] from contract data engineering projects
    - Key Result 9: Publish [X #] data engineering articles, blogs, case studies.
    - Key Result 10: Publish [X #] of data engineering podcasts.
    - Key Result 11: Publish [X #] of post on Linkedin
    - Key Result 12: Publish [X #] of comments on Linkedin
    - Key Result 13: Publish [X #] of article contributions on Linkedin 

Objective 2: Contribute meaningfully to the data engineering community (Ongoing)
    - Key Result 1: Gain [X #] readers on Substack
    - Key Result 2: Gain [X #] followers on Linkedin
    - Key Result 3: Get [X #] on impressions on Linkedin (Discovery)
    - Key Result 4: Get [X #] of members reached per post on Linkedin (Discovery)
    - Key Result 5: Get [X #] of reactions per post on Linkedin (Engagement)
    - Key Result 6: Get [X #] of comments per post on Linkedin (Engagement)
    - Key Result 7: Get [X #] of repost per post on Linkedin (Engagement)
    - Key Result 8: get [X #] of Profile viewers in Past 90 days
    - Key Result 9: get [X #] of search appearances in previous week
    - Key Result 3: Gain [X #] followers on Threads
    - Key Result 3: Contribute to [X #] of data conferences, podcasts, webinars etc.

- Objective 2: Secure a Job as a Data Engineer - 9 to 18 months
    - Key Result 1: Apply to [X #] relevant data engineering roles
    - Key Result 2: Attend [X #] of networking events.
    - Key Result 3: Recieve Feedback on [X #] job interviews.
    - Key Result #4 Make [X #] of new connections

- Objective 3: Run a Data Engineering Consulting Firm - 3 to 5 years
    - Key Result 1: Secure [X #] of clients
    - Key Result 2: Deliver [X #] of data engineering projects
    - Key Result 3: Achieve a client satisfaction rate of [X %]

- Objective 4: Becoming Data Engineering Manager or Team Lead - 8 to 12 years
    - Key Result 1: Lead [X #] successful data engineering projects
    - Key Result 2: Complete [X #] of leadership or management development courses
    - Key Result 3: Present or contribute to [X #] data engineering conferences, podcasts, blogs.
    - Key Result 4: Implement [X #] of data engineering best practices across teams or departments
    - Key Result 5: Publish [X #] of data engineering articles
    - Key Result 6:  Contribute [X %] or [X $] to company revenue or cost savings through data engineering projects.

*Mapped Domains:* Education and learning data (courses, coding platforms, books), goal tracking, certrifications, career advancement initiatives, and personal projects.
____________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

### Scope:

**Inside Scope**:
1. Develop a Fully Operational Data Pipeline:
    - Build a data pipeline using Azure that integrates multiple data sources (financial, health, media, educational growth) and includes processes for extraction, storage, orchestration, transformation, and serving.

2. Ensure Data Security and Privacy:
    - Implement robust security measures to protect sensitive data throughout the pipeline, including access control and encryption.

3. Generate Analytical Reports:
    - Create Power BI dashboards and reports that provide actionable insights across key value domains such as well-being, financial stability, educational growth, and family relationships.

4. Apply Machine Learning:
    - Develop predictive machine learning models for insights on financial trends, health metrics, and media categorization.

5. Document Project Lifecycle:
    - Produce detailed project documentation, including project scope, phase updates, and a final review of challenges, insights, and alignment with family values and objectives.

**Outside Scope**:
1. Real Personal Data:
    - Real personal data will not be used. All demonstrations and development will rely on mock datasets created using the Python faker module.

2. Advanced AI or Deep Learning Models:
    - The project will focus on basic machine learning models for predictions, excluding advanced AI or deep learning models.

3. Non-Core Domains:
    - The project will primarily focus on financial, health, media, and educational growth data, with potential future expansions into other domains like communication or personal growth outside the current scope.
_______________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

### Flow of Data in the ELT Pipeline:

**Extract:**
- Azure Data Factory (ADF) extracts raw data from multiple sources, such as financial institutions, health apps, and media libraries.

**Load:**
- The extracted data is loaded directly into Azure Data Lake Storage Gen2, creating a centralized Raw Data Store.
- Raw data remains in the data lake until it is transformed for analysis.

**Transform:**
- Azure Databricks is used for transformation after the data has been loaded into the data lake.
- Transformations include data cleaning, standardization, and preparing data for analysis and machine learning.
- Processed data is then stored back in Azure Data Lake Storage Gen2 and moved to Azure Synapse Analytics for data warehousing and reporting.

**Data Warehousing and Analysis:**
- Data is moved to Azure Synapse Analytics for querying, analysis, and advanced reporting.
- Synapse enables complex data analysis across different domains (financial, health, media, and personal growth).

**Visualization and Reporting:**
- Power BI is used to create dashboards that provide insights into well-being, financial stability, family relationships, and personal growth.

**Machine Learning:**
- Machine learning models are applied to generate predictions, such as financial forecasts, health trend predictions, and media categorization using tools like Azure Cognitive Services.
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

### Key Deliverables:

1. **Stable and Functioning Data Pipeline with Security**:
    - Deliver a fully operational pipeline that automates data extraction, storage, orchestration, transformation, and serving
    - Ensure the pipeline integrates data from multiple domains (financial, health, media, and educational growth) using Azure Data Factory and Azure Data Lake Storage Gen2.
    - Implement robust security and privacy controls, including encryption and access management, to ensure sensitive data is protected at all stages.
    
2. **Comprehensive Analytical Reports**:
    - Generate detailed reports and dashboards using Power BI that provide actionable insights across key value domains, including:
        - Well-being: Health metrics (e.g., fitness tracking, sleep analysis).
        - Financial Stability: Income and expense tracking, investment performance.
        - Educational Growth: Progress in learning and personal development.
        - Family Relationships: Tracking family events and organizing media.
    - Ensure all reports are aligned with the key values and provide clear, useful insights to inform decision-making.
    
3. **Predicitve Machine Learning Models**:
    - Develop machine learning models to deliver predictive insights in areas such as:
        - Financial Trends: Forecast income, expenses, and investments.
        - Health Metrics: Predict health outcomes or fitness trends.
        - Media Categorization: Organize and label family media using models like Azure Cognitive Services.
    - Ensure all models are designed to align with and support key values and domains, offering reliable insights and forecasting.
    
4. **Detailed Project Scope Document**:
    - Deliver a project scope document that clearly outlines project objectives, key milestones, deliverables, timelines, and resources.
    - Ensure the scope document aligns with the overall goals of managing personal data across multiple domains while adhering to key values.

5. **Phase-Based Project Update Documents**:
    - Create comprehensive project update documents at the conclusion of each phase, summarizing:
        - Progress made and milestones achieved.
        - Challenges faced and how they were addressed.
        - Insights gained and how the work aligns with key values.
    - These updates will provide ongoing reflection and ensure continuous alignment with project goals.

6. **Final Project Review Document**:
    - Deliver a finalized project review document that serves as the culmination of the entire project.
    - Include a full write-covering:
        - The entire project lifecycle.
        - Key challenges encountered and solutions.
        - Major insights gained and lessons learned.
        - Alignment with key values and objectives.
    - This document will serve as a reflective guide for future projects, ensuring the work aligns with both personal and technical goals.
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

### Assumptions and Risk

**Assumptions:**
- Data ingestion will start manually for initial testing, followed by automation.
- Azure services will be utilized for all production-level operations (storage, transformation, analysis).
- The faker module will be used to generate mock datasets for development.

**Risks:**
- Risk: Accidental exposure of real personal data during live streaming.
    - Mitigation: Use of mock datasets and encryption for all sensitive data.
- Risk: Data corruption or loss due to system failure.
    - Mitigation: Implementation of robust backup and recovery strategies.
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

### Timeline, Success Criteria, and Tools & Technologies

**Timeline:**
- Phase 1: Financial Stability Pipeline (x)
- Phase 2: Educational & Career Growth Pipeline (x)
- Phase 3: Health & Well-Being Pipeline (x)
- Phase 4: Family & Relationships Pipeline (x)

**Success Criteria:**
- Phase 1: Fiancial Stability Pipeline
    - Successful extraction and loading of mock data from all target sources.
    - Cleaned and transformed data stored in Azure Synapse for analysis.
    - Power BI dashboards providing insights into financial stability.
    - Machine learning models generating accurate predictions for financial stability.

- Phase 2: Educational & Career Growth Pipeline
    - Successful extraction and loading of mock data from all target sources.
    - Cleaned and transformed data stored in Azure Synapse for analysis.
    - Power BI dashboards providing insights into educational growth.
    - Machine learning models generating accurate predictions for educational growth.

- Phase 3: Health & Well Being Pipeline
    - Successful extraction and loading of mock data from all target sources.
    - Cleaned and transformed data stored in Azure Synapse for analysis.
    - Power BI dashboards providing insights into well-being.
    - Machine learning models generating accurate predictions for well-being.

- Phase 4: Family & Relationships Pipeline
    - Successful extraction and loading of mock data from all target sources.
    - Cleaned and transformed data stored in Azure Datalake & Azure Synapse Analytics for analysis.
    - Power BI dashboards providing insights into well-being.
    - Machine learning models generating accurate predictions for well-being.

**Tools & Technologies:**
- Data Ingestion: Python, Azure Data Factory
- Storage: Azure Data Lake Storage Gen2, Azure Synapse Analytics
- Transformation: Azure Databricks, Python (pandas), Azure Cognitive Services (for media)
- Reporting: Power BI, Python (matplotlib, seaborn)
- Machine Learning: Python (scikit-learn, TensorFlow), Azure Machine Learning
- Mock Data: Python faker
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________
