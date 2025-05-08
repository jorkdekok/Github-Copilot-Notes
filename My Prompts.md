# My Copilot prompts

- What are the team's coding preferences?
- What is this application doing, how is it built, and what are the key components?


----
Task: Create a new HrmData model, HrmEntity functions, and a corresponding service.
Requirements:
1.	The HrmData model should be based on the structure of HrmEmployeeContract.cs.
2.	Implement HrmEntity functions for both Bouw and Infra divisions, modeled after the existing HrmEmployeeContractFunction implementations.
3.	Create a new HrmEntityService to handle operations related to HrmData.
4.	Add unit tests for the new HrmEntity functions and service, following the patterns in HrmEmployeeContractFunctionTests.
5.	Update Program.cs to register the new HrmEntityService for dependency injection.
6.	Add any missing usings and constants required for the new implementations.
Context:
•	The HrmEmployeeContract.cs file provides the structure for the HrmData model.
•	The HrmEmployeeContractFunction implementations in Bouw and Infra directories serve as references for the new HrmEntity functions.
•	The Program.cs file contains the dependency injection setup for services.
Question: How can I ensure the new HrmEntity functions and service align with the existing patterns and integrate seamlessly with the current setup?
![image](https://github.com/user-attachments/assets/f5d19535-fef4-493b-8b1e-9eacf6cb2b7a)
----


----
"I need to create a new HrmDate model based on the structure of HrmEmployeeContract.cs. This model should include properties for EmployeeId, StartDateOfEmployment, EndDateOfEmployment, OrganizationalChartLayer3, and OrganizationalChartLayer4.
Additionally, I need to implement HrmDateFunction for both Bouw and Infra divisions, following the pattern of HrmEmployeeCompetenceFunction. These functions should handle Service Bus triggers and timer triggers for processing HrmDate data.
Please also create a new HrmDateService to handle the business logic for upserting HrmDate data, and include unit tests for both the service and the functions. Ensure all necessary constants, configurations, and usings are added to the appropriate files.
Let me know if there are any improvements or optimizations I can make to this approach."
----
