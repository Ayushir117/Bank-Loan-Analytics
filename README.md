# Bank Loan Analysis Dashboard

A comprehensive data analysis project examining bank loan performance using PostgreSQL, Excel, and Power BI to derive actionable insights for financial decision-making.

## 📊 Project Overview

This project analyzes bank loan data to provide insights into loan performance, risk assessment, and business metrics. The dashboard tracks key performance indicators (KPIs) including loan applications, funding amounts, repayment rates, and borrower characteristics.

## 🎯 Key Features

### Dashboard Components
- **Summary Page**: High-level KPIs and loan performance overview
- **Overview Page**: Detailed breakdowns by various dimensions
- **Details Page**: Granular loan-level information

### Key Performance Indicators (KPIs)
- Total Loan Applications: 38.6K
- Total Funded Amount: $435.8M
- Total Amount Received: $473.1M
- Average Interest Rate: 12.0%
- Average DTI Ratio: 13.3%
- Good Loan Rate: 86.2%
- Bad Loan Rate: 13.8%

## 📈 Analytics Insights

### Loan Performance
- **Good Loans**: 33K applications (86.2%) with $370.2M funded
- **Bad Loans**: 5K applications (13.8%) with $65.5M funded
- **Recovery Rate**: 108.6% ($473.1M received vs $435.8M funded)

### Loan Distribution Analysis
- **By Term**: 36 months (73.2%) vs 60 months (26.8%)
- **By Purpose**: Debt consolidation leads with 18K applications
- **By Home Ownership**: Rent and Mortgage categories dominate
- **By Employment Length**: 10+ years experience shows highest volume
- **By State**: Geographic distribution across all US states

## 🛠 Technical Stack

- **Database**: PostgreSQL
- **Data Visualization**: Power BI, Microsoft Excel
- **Query Language**: SQL
- **Data Processing**: ETL processes for data cleaning and transformation

## 📋 Database Schema

The analysis is based on the `Financial_loan` table with key fields:
- `id`: Unique loan identifier
- `loan_amount`: Principal loan amount
- `total_payment`: Total amount paid by borrower
- `loan_status`: Current status (Fully Paid, Current, Charged Off)
- `int_rate`: Interest rate
- `dti`: Debt-to-Income ratio
- `issue_date`: Loan origination date
- `address_state`: Borrower's state
- `purpose`: Loan purpose
- `term`: Loan term (36/60 months)
- `home_ownership`: Housing status
- `emp_length`: Employment length

## 🔍 SQL Analysis Features

### Time-Based Analysis
```sql
-- Month-to-Date (MTD) calculations
-- Previous Month-to-Date (PMTD) comparisons
-- Month-over-Month (MoM) growth analysis
```

### Loan Quality Metrics
```sql
-- Good Loan: 'Fully Paid' OR 'Current' status
-- Bad Loan: 'Charged Off' status
-- Performance ratios and percentages
```

### Dimensional Analysis
- Geographic distribution by state
- Temporal trends by issue month
- Borrower segmentation by employment length
- Loan purpose categorization
- Term-based analysis

## 📊 Dashboard Features

### Interactive Elements
- **State Filter**: Geographic drill-down capability
- **Grade Filter**: Risk grade segmentation
- **Good/Bad Loan Filter**: Performance-based filtering
- **Purpose Filter**: Loan purpose analysis

### Visualizations
- **Donut Charts**: Loan status distribution
- **Bar Charts**: Volume analysis by categories
- **Line Charts**: Temporal trend analysis
- **Maps**: Geographic distribution
- **KPI Cards**: Key metric highlights
- **Data Tables**: Detailed loan listings

## 📈 Business Impact

### Risk Assessment
- Identify high-risk loan categories
- Monitor default rates by segment
- Optimize approval criteria

### Performance Monitoring
- Track monthly loan origination trends
- Monitor collection efficiency
- Assess portfolio health

### Strategic Planning
- Geographic expansion opportunities
- Product mix optimization
- Risk-adjusted pricing strategies

## 🚀 Getting Started

### Prerequisites
- PostgreSQL database
- Power BI Desktop
- Microsoft Excel
- Basic SQL knowledge

### Setup Instructions
1. Clone the repository
2. Import the SQL schema and data
3. Execute the provided SQL queries
4. Open Power BI file (.pbix)
5. Refresh data connections
6. Explore the interactive dashboard

## 🔧 SQL Query Highlights

The project includes 25+ optimized SQL queries covering:
- **KPI Calculations**: Total applications, funding amounts, collection metrics
- **Time Intelligence**: MTD, PMTD, and MoM calculations
- **Risk Analytics**: Good vs bad loan classifications
- **Dimensional Analysis**: Breakdowns by state, purpose, term, etc.

## 📋 Usage

### For Business Analysts
- Use filters to drill down into specific segments
- Monitor KPIs for performance tracking
- Generate insights for stakeholder reporting

### For Data Scientists
- Leverage SQL queries for advanced analytics
- Extend analysis with machine learning models
- Perform statistical analysis on loan performance

### For Executives
- Review summary dashboard for high-level insights
- Track business performance against targets
- Make data-driven strategic decisions
