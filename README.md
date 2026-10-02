Salt-Corp-HR-Analytics-Workforce-Attrition-Analysis

An analysis of 1,000 employees at Salt Corporation to find out who is leaving and why, delivered as an Excel analysis workbook and a 10-slide presentation for decision-makers. A data-driven review of headcount, pay, satisfaction, and turnover across the organization to understand the organizational structure, the salaries across departments, job satisfaction among other factors and finally establish the attrition drivers and make recommendations to management to reduce the attrition rate.

Author: Joan Kamau

#	Finding	Evidence

1.	Job satisfaction is the strongest predictor of attrition.	Employees scoring satisfaction 1–2 leave at 56.0%, versus 26.4% for those scoring 3+. This group is 43% of headcount but accounts for about 62% of all departures (242 of 392).

2.	Finance combines low morale with high attrition - The lowest satisfaction score (2.72/5) sits alongside the second-highest attrition rate (40.4%).

3.	Marketing and the 3-5 year cohort turn over fastest- Marketing leads all departments at 42.8% attrition; the 3-5 year tenure band peaks at 40.9%.

4. Demographics are not the driver - Age, tenure, and employment type show only modest variation (roughly 37-41%), so broad policy changes targeting these alone are unlikely to help in retention. The 54–63 age group is lower (16.7%) but has only 12 people.

Overall attrition is 39.2% (392 of 1,000 employees). 

Average salary is $60,209 with only about a $1,300 spread between departments, so pay does not explain the differences.

<img width="1283" height="579" alt="image" src="https://github.com/user-attachments/assets/82e29c29-4b05-4a75-8c24-0164e314c1fc" />


Recommendations in the deck

1. Direct retention effort at employees scoring 1–2 on satisfaction, rather than broad salary increases.
2. Audit workload and tooling in Finance, paired with manager coaching.
3. Introduce a mid-tenure career path (year 3–5 milestone reviews and promotion tracks).
4. Institutionalise stay interviews, starting with Marketing.

WORKFORCE OVERVIEW

Metric	Value

Total employees	1,000

Average salary	$60,209

Female / Male	49.3% / 50.7%

Overall attrition rate	39.2%

Gender	Gender Distribution
Female	49.3%
Male	50.7%

<img width="485" height="117" alt="image" src="https://github.com/user-attachments/assets/bb745a22-dd5c-4b0d-ade8-73df5f6a073e" />


<img width="566" height="355" alt="image" src="https://github.com/user-attachments/assets/b15d6de3-af1f-49eb-9c18-2ab1f3dad991" />

Department	Average Salary per Department
Sales	 60,993 
HR	 60,236 
Marketing	 60,107 
Finance	 59,984 
IT	 59,713 
Grand Total	 60,209 


<img width="547" height="204" alt="image" src="https://github.com/user-attachments/assets/18da66ff-0c20-4efa-b86e-1078ff6b8707" />

<img width="821" height="450" alt="image" src="https://github.com/user-attachments/assets/5f627fc9-61e2-41bf-a090-b18a6c2cfb5e" />

Method summary

Cleaning: consistent department and employment-status labels, text salaries and ages converted to numbers, date formats standardised.

  - Cleaning Salary Column: IFS(TRIM(G2)="SIXTY THOUSAND",60000,TRIM(G2)="NAN",AVERAGEIFS(G:G,J:J,J2,L:L,L2),TRUE,G2)

  - Cleaning Department Column: IF(OR(J2="HR",J2="IT"),UPPER(J2),PROPER(J2))

  - Filled missing email addresses: =LOWER(CONCAT(B8,".",C8,"@saltcorp.com"))

Analysis: attrition rate (share of employees who left) compared across department, job satisfaction, age band, years-of-service band and employment status, in Excel pivot tables.

Attrition Per Department	

Total Attrition Rate 39.2%

<img width="632" height="273" alt="image" src="https://github.com/user-attachments/assets/df09d8df-8405-4b80-afb5-4d6f2e1aed5d" />


Attrition Vs Years of Service		
		
Years of Service	Attrition Rate	
0-2	36.8%	
3-5	40.9%	
6-8	39.1%	
Grand Total	39.2%	

<img width="461" height="207" alt="image" src="https://github.com/user-attachments/assets/a108c6ef-40a4-434d-b6e6-e6a491623a08" />

Age Group Analysis

Age Group	Total Employees	Employees Left	Attrition Rate (%)
24-33	410	164	40.0%
34-43	388	153	39.4%
44-53	190	73	38.4%
54-63	12	2	16.7%


<img width="735" height="146" alt="image" src="https://github.com/user-attachments/assets/530ff60c-8b2f-44d2-b814-076405986d7a" />

Attrition by Employment Status	
	
Employment Status	Attrition Rate (%)

Contract	40.0%
Full-Time	40.2%
Part-Time	36.9%
Grand Total	39.2%


<img width="468" height="213" alt="image" src="https://github.com/user-attachments/assets/3882f6bd-5748-476f-9943-db909b630839" />

Job Satisfaction

Department	Job_Satisfaction/Department
Marketing	3.01
HR	2.99
Sales	2.98
IT	2.91
Finance	2.72
Grand Total	2.92


<img width="519" height="204" alt="image" src="https://github.com/user-attachments/assets/1db2f680-d494-4faf-b892-ba9213df0e5b" />


Job Satisfaction vs Attrition Rate

Job Satisfaction Score	Employees	Employees Left	Attrition Rate

1	 218	128	59%
2	 214	114	53%
3 	182	50	27%
4	 206	54	26%
5	 180	46	26%
Grand Total	1000	392	39%

<img width="849" height="204" alt="image" src="https://github.com/user-attachments/assets/0656a8cd-58bd-4c42-8e08-ef4045eb5406" />



Bands: 

Age 24–33 / 34–43 / 44–53 / 54–63 

Years of service 0–2 / 3–5 / 6–8 

Job Satisfaction Low (1–2) vs Higher (3–5)
 


