Requirements

When the app is started, the user is presented with the main menu, which allows the user to (1) enter or edit current job details, (2) enter job offers, (3) adjust the comparison settings, or (4) compare job offers (disabled if no job offers were entered yet). 

When choosing to enter current job details, a user will:
Be shown a user interface to enter (if it is the first time) or edit all the details of their current job, which consist of:
Title
Company
Location (entered as city and state)
Cost of living in the location (expressed as an index)
Yearly salary 
Yearly bonus 
Number of stock option shares offered
Home Buying Program fund (one-time dollar amount up to 15% of Yearly Salary)
Personal Choice Holidays (A single overall number of days from 0 to 20)
Monthly Internet Stipend ($0 to $75 inclusive)
Be able to either save the job details or cancel and exit without saving, returning in both cases to the main menu.
When choosing to enter job offers, a user will:
Be shown a user interface to enter all the details of the offer, which are the same ones listed above for the current job.
Be able to either save the job offer details or cancel.
Be able to (1) enter another offer, (2) return to the main menu, or (3) compare the offer (if they saved it) with the current job details (if present).
When adjusting the comparison settings, the user can assign integer weights to:
Yearly salary
Yearly bonus
Number of Stock Option Shares Offered
Home Buying Program Fund
Personal Choice Holidays
Monthly Internet Stipend
If no weights are assigned, all factors are considered equal.
When choosing to compare job offers, a user will:
Be shown a list of job offers, displayed as Title and Company, ranked from best to worst (see below for details), and including the current job (if present), clearly indicated.
Select two jobs to compare and trigger the comparison.
Be shown a table comparing the two jobs, displaying, for each job:
Title
Company
Location 
Yearly salary adjusted for cost of living
Yearly bonus adjusted for cost of living
Number of Stock Option Shares Offered
Home Buying Program fund (one-time up to 15% of Yearly Salary)
Personal Choice Holidays (A single overall number of days from 0 to 20) 
Monthly Internet Stipend ($0 to $75 inclusive monthly)

Be offered to perform another comparison or go back to the main menu.
When ranking jobs, a job’s score is computed as the weighted average of:

AYS + AYB + (CSO/3) + HBP + (PCH * AYS / 260) + (MIS*12)

where:
AYS = yearly salary adjusted for cost of living
AYB = yearly bonus adjusted for cost of living
CSO = Company shares offered (assuming a 3-year vesting schedule and a price-per-share of $1)
HBP = Home Buying Program
PCH = Personal Choice Holidays 
MIS= Monthly Internet Stipend 

For example, if the weights are 2 for the yearly salary, 2 for the yearly bonus, 2 for Internet Stipend, and 1 for all other factors, the score would be computed as:


2/9 * AYS + 2/9 * AYB + 1/9 * (CSO/3) + 1/9 * HBP + 1/9 * (PCH * AYS / 260) + 2/9 * (MIS*12)

The user interface must be intuitive and responsive.
For simplicity, you may assume there is a single system running the app (no communication or saving between devices is necessary).
