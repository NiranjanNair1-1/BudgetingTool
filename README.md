# Budgeting Tool - Budgeting App for University Students (Console)


## Analysis


### 1. Problem Statement and Target User 


**Target User** 

University Student who look after their own day-to-day expenditure and are funded through a combination of part-time work and family support. Throughout this, README, these users are referred to as *university students*


**The Problem**

University students get their money from several sources, often at different times during the month. They spend it on many small, frequent purchases such as groceries, transport, rents etc. Without some kind of record, they can't see where their money is going or how much is left for the rest of the month. 


**Why it Matters**

If student lose sight of their expense or their spending, they are likely to overspend at the start of the month and end up with very little left for essential i.e. rent, food, transport etc. This can lead to financial stress, more dependency on family or borrowing and it makes it much harder to plan ahead. 


**The Need**

University students need a simply way to: 
- record income from different sources
- record everyday expenses by category
- understand how their money is being spent
- monitor their remaining balance for the current month

Our budget app (Python) provides all these functions in one place.

---


### 2. Scenario, User Roles and Project Scope 

#### Scenario

Mia is a second year university student. She works part time at a cafe and earns an income of CHF 900 per month. Her parents send her CHF 600 at the beginning of each month. Her wages come into two payments i.e. mid-month and at the end of the month. 

Mia pays rent, buys groceries several times a week, tops her public transport pass and occasionally goes out with friends. Because her income arrives at different times and her expenses are small and frequent, she often has no idea how much balance she has left. Last month she spent quite a lot on leisure in the first two weeks and had to ask her parents for extra money to cover groceries before her next wage.  

Mia wants a simple way to keep an eyer on her money. Using the budgeting app, she: 
1. records her family support and each wage payment as income, noting the source
2. records each expense as it happens, choosing a category such as groceries, transport, rent or leisure.
3. check a monthly summary showing her total income, total expenses and remaining balance.
4. looks at her spending by category and sees that leisure takes a larger share that she expected.
5. reduces her leisure spending for the rest of the month so that she has enough left for essentials.

 #### User Roles 

 The app has a single user role: the **university student**. There are no admin or shared-access roles, because each student uses the app to manage their own personal budget. In this README, "the user" means university student using the app. 

 - **Who they are:** A university student managing their own monthly budget (see section 1)
 - **Responsibilities:** Enter income and expenses accurately and promptly, assign each expense to the correct category, correct or delete wrong entries, and regularly review the monthly summary.
 - **Goals:** Know how much money is left for the month, see which categories they spend the most on, and avoid running short of money for essentials before the end of month.
 - **How they interact with the app:** Start the app on their own computer and use the menu to add income, add expense, view transactions edit or delete entries, and view the monthly summary and spending by category. Data is saved locally and reloaded the next time the app is opened.

#### Project Scope

**In Scope**
- recording an income with an amount, date and source (part time employment, family support or other)
- recording expenses with an amount, date, category and short description
- predefined expense categories: groceries, transport, rent, leisure, other
- viewing list of all transaction, filtered by month
- editing and deleting existing entries
- a monthly summary showing a total income, total expense and remaining balance
- a breakdown of spending by category for selected month
- saving data to local file and loading it when app starts
- input validation - no negative amounts, valid dates, valid categories
  

**Out of Scope**
- connecting to bank accounts or importing bank statements
- multiple user account, login or password protection
- cloud storage or syncing across devices
- a mobile app or web version
- shared or group budgets for example with flatmates
- multiple currencies (all amounts are in one currency)
- Automatic reminders or notifications
- saving goals, investment tracking, loans or tax calculations
- predictions or automated financial advise

These boundaries help keep the project achievable within th ecourse timeframe while sttill addressing the core need identified in SECTION 1.

---

  ### 3. User Stories 
  
**Niranjan User Stories:**
1. **US-01:** As a user, I want to add an expense with amount so that I can track my spending.
2. **US-02:** As a user, I want to add income (e.g. salary), so that I can see the money coming in.
3. **US-03:** As a user, I want to add an expense with category and description, so that I can track my spending.
  

**Andras User Stories:**

4. **US-04:** As a user, I want to add an expense with a date so that I can track my spending.
5. **US-05:** As a user, I want to edit a wrong entry, so that my data stays correct.
6. **US-06:** As a user, I want to delete a wrong entry, so that my data stays correct.


**Alpha User Stories:**

  7. **US-07:** As a user, I want to choose a category from a fixed list and see how much I spent per category, so that I know where my money goes.
  8. **US-08:** As a user, I want to set a monthly budget per category and get a warning when I go over it, so that I don't overspend.
  9. **US-09:** As a user, I want to set a savings goal and see my progress, so that I stay motivated.


**Stefano User Stories:**

  10. **US-10:** As a user, I want to see all my transactions, sorted by date, so that I have an overview.
  11. **US-11:** As a user, I want to filter the list (only expenses, only income, one category), so that I find things quickly.
  12. **US-12:** As a user, I want a dashboard with income, expenses and balance for a month I choose, so that I know where I stand.
