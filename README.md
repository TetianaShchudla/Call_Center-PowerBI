# Call Center Analysis Project

![image](https://github.com/TetianaShchudla/Call_Center-PowerBI/blob/main/Images/callcenter.png)

# Overview
This project focuses on analyzing call center data for _ServiceSpot_, an IT company. __The goal__ is to provide insights through visually appealing reports using Power BI. The data, sourced from multiple files, includes call details, employee information, call types, U.S. states, and call charges.

# Data Dictionary
## CSV Files (Data YYYY)
These files contain call data for each year, with _the following columns_:

- _CallTimestamp:_ Date and time of the call
- _Call Type:_ Type of call
- _EmployeeID:_ Unique ID for the employee
- _CallDuration:_ Duration of the call in seconds
- _WaitTime:_ Wait time in seconds
- _CallAbandoned:_ Indicates if the call was abandoned (1 = Yes, 0 = No)

## Lookup Data

__Employees__
- _EmployeeID:_ Unique ID for the employee
- _EmployeeName:_ Full name of the employee
- _Site:_ Site name where the employee works
- _ManagerName:_ Employee's manager
  
__Call Types__
- _CallTypeID:_ Unique ID for the call type
- _CallTypeLabel:_ Label for the call type

__U.S. States__
- _StateCD:_ 2-letter state code
- _Name:_ Name of the state
- _Region:_ Name of the U.S. region (East, West, etc.)

__Call Charges__
- _Call Type Key:_ Unique ID for the call type
- _Call Type:_ Label for the call type
- _Call Charges / Min (YYYY):_ Amount charged per minute for each call type and year

# Report Findings

The data files run until the end of 2021. The last file (2021) had issues, including inconsistent timestamps and notable differences in wait times. The data appears to be an extract, as agents handle fewer than two calls per day, which is not realistic. Therefore, findings will focus on long-term trends rather than daily performance.

# Key Insights

## 1. Overview
Basic total numbers indicate all three regional centers are of similar size, with Washington showing slightly less revenue. SLA compliance stands at 86%.

![image](https://github.com/TetianaShchudla/Call_Center-PowerBI/blob/main/Images/overview.png)

## 2. Calls Performance
This operational dashboard allows filtering by date and state, showcasing total call numbers, wait times, abandoned calls, and SLA compliance.

![image](https://github.com/TetianaShchudla/Call_Center-PowerBI/blob/main/Images/calls_performance.png)

## 3. Time Trends
Patterns reveal average calls per day of the week with no significant differences and highlight seasonality, particularly a drop in calls at the year's end.

![image](https://github.com/TetianaShchudla/Call_Center-PowerBI/blob/main/Images/time_tends.png)

## 4. Agents Performance
Analyzes individual agent performance and team efficiency. Notably, SLA compliance dropped from 88% at the end of 2020 to 78% by the end of 2021. This decline correlates with an increase in average wait time.
Managers Jamar Prahl and Collin Tratman generate the most revenue due to the high volume of calls they handle.

![image](https://github.com/TetianaShchudla/Call_Center-PowerBI/blob/main/Images/agents_performance.png)

# Conclusion
This analysis provides valuable insights into call center operations, identifying areas for improvement and ensuring that ServiceSpot can enhance its customer service strategy.
