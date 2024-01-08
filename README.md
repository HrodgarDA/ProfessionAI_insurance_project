# ML: Credit Evaluation
The goal of this project is to develop a machine learning model capable of evaluate the creditworthiness of people based on the following set of parameters:

application_record.csv
FEATURE                    NAME                	          {EXPLANATION} 
ID 	                       Client number	
CODE_GENDER 	             Gender	
FLAG_OWN_CAR	             Is there a car	
FLAG_OWN_REALTY         	 Is there a property	
CNT_CHILDREN	             Number of children	
AMT_INCOME_TOTAL	         Annual income	
NAME_INCOME_TYPE	         Income category	
NAME_EDUCATION_TYPE        Education level	
NAME_FAMILY_STATUS         Marital status	
NAME_HOUSING_TYPE 	       Way of living	
DAYS_BIRTH 	               Birthday	                      {Count backwards from current day (0), -1 means yesterday}
DAYS_EMPLOYED 	           Start date of employment	      {Count backwards from current day(0). If positive, it means the person currently unemployed}
FLAG_MOBIL                 Is there a mobile phone	
FLAG_WORK_PHONE 	         Is there a work phone	
FLAG_PHONE 	               Is there a phone	
FLAG_EMAIL                 Is there an email	
OCCUPATION_TYPE         	 Occupation	
CNT_FAM_MEMBERS 	         Family size

credit_record.csv		
FEATURE                    NAME                	          {EXPLANATION}
ID	                       Client number	
MONTHS_BALANCE	           Record month	                   {The month of the extracted data is the starting point, backwards, 0 is the current month, -1 is the previous month, and so on}
STATUS	                   Status	                         {0: 1-29 days past due 1: 30-59 days past due 2: 60-89 days overdue 3: 90-119 days overdue 4: 120-149 days overdue 5: Overdue or bad                                                                debts, write-offs for more than 150 days C: paid off that month X: No loan for the month}
