# Banking_Domain_Data_Analysis_Project
### 1.	Banking Dashboard
Develop a basic understanding of risk analytics in banking and financial services and understand how data is used to minimise the risk of losing money while lending to customers.

### 2. Description/Purpose
With our dashboards which are created using Power BI latest tools helps the company to make a decision based on the applicant’s profile like if the applicant is likely to repay the loan then approving the loan otherwise not

### 3. Tech Stack
List the key technologies used to build the dashboard.
The dashboard was built using the following tools and technologies:

- 📊 Power BI Desktop – Main data visualization platform used for report creation.
- 📂 Panda – Used for data cleaning and data preaparing.
- 🧠 MySQL – Used for storing data from csv file into database.
- 📝 Matplotlib/Seaborn – Used to perform EDA(Exploratory Data Analysis) and find correlation between various columns.
- 📁 File Format – .pbix for development and .png for dashboard previews.

### 4. Data Source
This dataset basically contains information about bank details ,various client details which consists of multiple tables which are interlinked with each other through keys like primary key and foreign key.
The various tables are Banking Relationship, Client-Banking, Gender, Investment Advisor and Period.

### 5. Features / Highlights
• Data Cleaning – Creating a new column Engagement Timeframe in client-banking column which tells about the time line of the clients in banks
  KPI’S: 
  In which followings KPIS are present :
- Total Clients:
- Total Clients = DISTINCTCOUNT('Clients - Banking'[Client ID] )

• Total Loan :
- Total Loan gives you information about the bank loan + Business lending + credit cards balance of particular  investor , gender.
- Total Loan = [Bank Loan] + [Business Lending] + [Credit Cards Balance]

• Bank Loan :
- Bank Loan gives you information what is the loan amount of loan to be repaid by the client to bank.
- Bank Loan = SUM('Clients - Banking'[Bank Loans] )

• Business Lending :
- Business lending gives you information about the loan amount given to small business.
- Business Lending = SUM('Clients - Banking'[Business Lending] )

• Total Deposit 
- Total Deposit gives you information about the amount deposited by particular investors in bank
- Total Deposit = [Bank Deposit] + [Savings Account] + [Foreign Currency Account] + [Checking Accounts]

• Total Fees :
- Total Fees is nothing but the amount charged by the bank for account set-up , maintenance charges etc.
- Total Fees = SUMX('Clients - Banking' , [Total Loan] * 'Clients - Banking'[Processing Fees] )

• Bank Deposit :
- Bank deposit is the money put in the bank.
- Bank Deposit = SUM('Clients - Banking'[Bank Deposits] )

• Checking Account Amount :
- Checking account amount  is nothing but which offers easy access to your money for daily transactional needs.
- Checking Accounts = SUM('Clients - Banking'[Checking Accounts] )

• Total CC Amount :
- Total CC Amount is a short-term source of financing for a company by a bank.
- Total CC Amount = SUM('Clients - Banking'[Amount of Credit Cards] )

• Saving Account Amount :
- A savings account is an interest-bearing deposit account held at a bank.
- Savings Account = SUM('Clients - Banking'[Saving Accounts] ) 

• Foreign Currency Amount :
- Foreign Currency Account means an account held in a currency that is not the currency of India or Bhutan or Nepal.
- Foreign Currency Account = SUM('Clients - Banking'[Foreign Currency Account]) 

### 6. Screenshots / Demos
[Dashboard Preview]-(https://github.com/the-sweta-upadhyay/Banking_Domain_Data_Analysis_Project/blob/main/BANKING%20DASHBOARD%20(2).png)
