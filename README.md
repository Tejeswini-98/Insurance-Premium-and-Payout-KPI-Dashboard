# Insurance-Premium-and-Payout-KPI-Dashboard
## Insurance Premium and Payout KPI Dashboard Project in PowerBI
<img width="1361" height="720" alt="image" src="https://github.com/user-attachments/assets/83a6d31a-1360-42d3-8efe-e3721b0832db" />
<img width="1366" height="678" alt="image" src="https://github.com/user-attachments/assets/2340d2db-047c-40e1-8f29-f513cd8faa0a" />


### Overview 🎯
This video introduces a comprehensive finance-focused data analytics project designed to teach how to build an interactive PowerBI dashboard for an insurance company. The core content centers on creating a premium and payout KPI dashboard for True Secure Credit Insurance, covering data acquisition, cleaning, modeling, and visualization. The instructor explains detailed financial metrics, data relationships, and DAX calculations using real client requirements. The teaching method combines hands-on PowerBI steps, theoretical explanations of insurance data, and practical examples to prepare learners for finance domain analytics and job interviews.

### Summary of Core Knowledge Points ⏱️

- **00:00-01:05 Introduction to Project & Business Scope**  
  - The project focuses on building a KPI dashboard for insurance premium management and payout analysis in PowerBI.  
  - Learners will track premiums, claims, maturity amounts, and key metrics like revenue growth and customer retention in an interactive report.

- **01:06-04:45 Client Requirements & Insurance Business Overview**  
  - Data from 2015-2025 includes policy lifecycle, customer info, claims, loans, maturity calculations.  
  - True Secure Credit Insurance focuses on credit/debit linked insurance covering individuals and businesses.  
  - Business goals include policy performance tracking, segmentation analysis by state and customer, claim settlement monitoring, and report automation.

- **04:46-17:00 Dataset Structure & Tables**  
  - Key tables include customer details, policy types, policy names, sales agents, insurance policies (fact table), regional and zonal managers.  
  - Variables explained: customer demographics, premium amounts, policy tenure, claim eligibility, underwriting expenses, loan eligibility criteria.  
  - Distinction between fact (transactional) and dimension (categorical) tables to form a star schema.

- **17:01-22:45 Example Policy Walk-through & Calculation Concepts**  
  - Sample term policy illustration with premium amount, tenure, start date.  
  - Calculations for total premium paid, premium payable (remaining), maturity amount based on premium, tenure, and return rates.  
  - Explanation of financial terms: ROI and CAGR with investment examples.

- **22:46-29:00 PowerBI Data Import & Cleaning**  
  - Data loading from CSV files, use of Power Query Editor for cleaning: removing blanks, removing header rows, setting column headers, choosing relevant columns.  
  - Methods to ensure data type consistency for numerical calculations.

- **29:01-43:00 Data Modeling & Relationships**  
  - Importance of star schema for performance: fact table in the center with dimension tables linked by keys.  
  - Relationship creation between tables using primary and foreign keys.  
  - Cross filter directions (single vs bi-directional) explained with practical filtering examples.  
  - Modeling enables efficient data filtering and drill-down in reports.

- **43:01-58:00 Calculated Columns & Measures (DAX)**  
  - Introduction to implicit vs explicit measures.  
  - Stepwise creation of key calculated columns: total annual premium (aligned by payment frequency), total premium amount, premium payment duration, total premium paid, premium payable.  
  - Use of PowerBI DAX functions like SWITCH, IF, and variables (VAR) with RETURN for complex conditional calculations.

- **58:01-01:34:00 Advanced Financial Calculations**  
  - Maturity amount calculated using premium, tenure, policy type, and return rate conditions with nested DAX logic.  
  - Calculation of annualized ROI using DAX power and divide functions with safeguards against divide-by-zero errors.  
  - CAGR measure calculated to reflect compound growth over investment period.  
  - Profit and gain calculated as difference between maturity amount and total premium paid.

- **01:34:01-02:01:00 Buckets, Flags & Segmentation**  
  - Creation of payment buckets (e.g., mature in next 5, 10, 15, 20 years) using date difference and SWITCH statements as flags.  
  - These help segment data for focused reports on premium due in future periods.  
  - User filters data via slicers linked to buckets for customized views.

- **02:01:01-03:04:00 Visualization Setup & KPI Cards**  
  - Dashboard design principles: first page as summary with key performance indicators (KPIs) in card visuals (number of policies, total premium amount, annual premium, underwriting expenses).  
  - Styling techniques: rounded corners, background colors, font sizes for clarity.  
  - Creation of detailed data tables and slicers for filtering by policy type, name, sales agent, state, occupation, and year.  
  - Use of bar charts, pie charts, tree maps for visual comparison among categories.

- **03:05:00-03:59:00 Dynamic Visuals & Field Parameters**  
  - Utilization of PowerBI field parameters to switch measures dynamically in visuals based on user selection.  
  - Creation of explicit sum measures for aggregation compatible with field parameters.  
  - Setting up slicers for selecting different metrics like total premium paid, payable, underwriting expense for interactive exploration.

- **04:00:00-04:30:00 Advanced Visualizations & Comparison Charts**  
  - Investment value vs maturity value displayed with line and clustered column charts.  
  - Annual premium vs sum assured protection values compared over tenure years.  
  - Use of funnels, stacked bar charts, and area charts with conditional formatting for better insight.  
  - Slicers allow breakdown by tenure buckets and detailed filters.

- **04:31:00-04:56:00 Sales Hierarchy Performance & Role-Based Views**  
  - Construction of dynamic sales hierarchy matrix showing zonal managers, regional managers, sales agents, and policy holders.  
  - Implementation of field parameters for flexible data rows selection.  
  - Sync slicers and bookmarks to swap between matrix and chart views for hierarchical data analysis.  
  - Visual border, gridlines, drill-down enabled for user-friendly navigation.

- **04:57:00-End Role Level Security (RLS) Implementation**  
  - Explanation of RLS concept: restricting data visibility based on user roles (owner/user), regions managed, and login email (User Principal Name).  
  - Creating DAX expressions using LOOKUPVALUE, USERPRINCIPALNAME, and IF to enforce security logic for sales agents, regional and zonal managers.  
  - Managing roles within PowerBI Desktop and viewing report as different users to validate security.  
  - Handling hierarchy with split state-region data to map security filters correctly.  
  - Publishing report and assigning user role permissions on PowerBI Service.

### Key Terms and Definitions 📚

- **Premium Amount:** The periodic payment made by the policyholder for the insurance coverage.  
- **Maturity Amount:** The sum payable to the policyholder at the end of the policy tenure.  
- **Claim Settlement:** The process of paying out insurance claims to the policyholders.  
- **ROI (Return on Investment):** Percentage gain on the invested premiums over the investment period.  
- **CAGR (Compound Annual Growth Rate):** Average annual growth rate of an investment assuming compounding interest.  
- **Star Schema:** Data modeling technique with a central fact table linked to dimension tables.  
- **Fact Table:** Table containing transactional or measurable data.  
- **Dimension Table:** Table containing descriptive attributes related to facts.  
- **Power Query Editor:** A PowerBI tool for data cleaning and transformation.  
- **DAX (Data Analysis Expressions):** Formula language used in PowerBI for creating calculated columns and measures.  
- **Switch Statement:** Conditional DAX function returning values based on expressions.  
- **UserPrincipalName:** DAX function returning the email ID of the logged-in user.  
- **Role Level Security (RLS):** Feature in PowerBI to limit data access based on user roles.  
- **LookupValue:** DAX function similar to Excel VLOOKUP to fetch related data based on matching criteria.  
- **Field Parameters:** PowerBI feature allowing dynamic selection of measures or dimensions in visuals.  
- **Slicer:** Visual filter control in PowerBI to slice data based on selected values.  
- **Bookmark:** Saved view state in PowerBI used to toggle visibility of visuals or pages.

### Reasoning Structure 🔍

1. **Project Requirement to Data Model Setup**  
   Premise: Client sends insurance data and business KPIs → Reasoning: Import diverse tables, define keys → Conclusion: Create star schema to link fact table with dimensions.

2. **Calculation Flow for Premium & Maturity**  
   Premise: Premium payments come in different frequencies → Reasoning: Convert all to annual amounts → Calculate total premiums paid and payable → Use policy type and tenure to compute maturity amount.

3. **Returning Financial Metrics with DAX**  
   Premise: Complex conditional logic needed → Reasoning: Use variables and SWITCH to implement different return rates → Calculate ROI and CAGR → Return key financial insights.

4. **Visual and Interactive Functionality**  
   Premise: Users want dynamic views → Reasoning: Implement slicers for dimensions and field parameters for measures → Build charts that respond to user selection → Enhanced exploration of data.

5. **Security Implementation Logic**  
   Premise: Sensitive data requires access control → Reasoning: Use USERPRINCIPALNAME and LOOKUPVALUE to map logged users to roles → Define conditions for owners vs users → RLS filters data accordingly.

### Examples 🎓

- **Policy Calculation Example:**  
  A term policy with a 20-year tenure paying 100,000 annually started in 2020. Total premium paid by 2025 = 100,000 x 5 = 500,000; remaining payable = 100,000 x 15 = 1,500,000. Maturity amount calculated based on return rate tiers.

- **ROI Calculation Example:**  
  Investment of 100,000 over 3 years yields 133,100 total. Total ROI = 33.1%, Annualized ROI = 10%, demonstrating compounding effect.

- **Role Level Security Demo:**  
  Sales agent Ana logs in; using USERPRINCIPALNAME, PowerBI filters data just for Ana's clients. Regional manager sees data only for their assigned region, zonal manager sees entire zone.

- **Dynamic Visual Parameter Use:**  
  User selects Total Premium Paid or Underwriting Expense via slicer; dashboard visuals update instantly without multiple report pages.

### Error-prone Points ⚠️

- **Payment Frequency Handling:** Misaligning monthly, quarterly, yearly premiums leads to incorrect annual premium calculation. Correct use of SWITCH and multiplication factors is essential.

- **Data Modeling Direction:** Improper cross filter direction setting leads to broken filters between tables. Dim -> Fact should filter; bidirectional may cause unintended context propagation.

- **RLS Implementation:** Confusing owner and user roles can lead to overexposed or restricted data. Ensuring correct security level and email matching is vital.

- **DAX Syntax Errors:** Missing commas, wrong variable scopes or improper use of RELATED function can cause calculation failure.

- **Visual Parameter Compatibility:** Calculated columns cannot be easily used in field parameters; they require explicit measures for dynamic visuals.

### Quick Review Tips / Self-Test Exercises 🎓

**Tips (No Answers):**  
- Explain the difference between fact and dimension tables in star schema.  
- Describe how premium payment frequency affects total premium calculations.  
- What is the purpose of cross filter direction in PowerBI data modeling?  
- Name two DAX functions essential for implementing role-level security.  
- How do field parameters improve report interactivity?

**Exercises (With Answers):**  
1. What DAX function converts a user’s login email to be used in RLS filters?  
   - **Answer:** USERPRINCIPALNAME()

2. If a policy has quarterly premium payments of 20,000, how is the total annual premium calculated?  
   - **Answer:** 20,000 × 4 = 80,000 (Annualized premium)

3. Which visual type is best to compare investment value vs maturity over time?  
   - **Answer:** Line and clustered column chart

4. What is the core logic behind setting up star schema relationships in PowerBI?  
   - **Answer:** Fact table contains foreign keys to dimension tables, connected by primary keys to enable efficient querying.

5. How do you create a maturity bucket flag for payments due in 10 years or less?  
   - **Answer:** Use a DAX SWITCH statement checking date difference from current date to tenure date ≤ 10 years, then assign flag.

### Summary and Review 📚
This tutorial comprehensively guides through building a finance domain PowerBI dashboard for insurance premium and payout analysis. Beginning with understanding client requirements and insurance data structure, it proceeds through diligent data cleaning and star schema modeling. The video covers detailed DAX calculations for premium alignment, maturity, ROI, and growth metrics. Visual design principles are applied to craft intuitive KPIs, filters, and comparison charts. Advanced features like dynamic field parameters enhance interactivity. Finally, robust role-level security implementation ensures sensitive data access is controlled by user roles aligned with organizational hierarchy. This structured approach teaches not only technical skills but also domain-specific insights vital for real-world data analyst roles in finance.
