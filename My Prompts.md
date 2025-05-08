# My Copilot prompts

- What are the team's coding preferences?
- What is this application doing, how is it built, and what are the key components?


## Prompt 1
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


## Prompt 2
"I need to create a new HrmDate model based on the structure of HrmEmployeeContract.cs. This model should include properties for EmployeeId, StartDateOfEmployment, EndDateOfEmployment, OrganizationalChartLayer3, and OrganizationalChartLayer4.
Additionally, I need to implement HrmDateFunction for both Bouw and Infra divisions, following the pattern of HrmEmployeeCompetenceFunction. These functions should handle Service Bus triggers and timer triggers for processing HrmDate data.
Please also create a new HrmDateService to handle the business logic for upserting HrmDate data, and include unit tests for both the service and the functions. Ensure all necessary constants, configurations, and usings are added to the appropriate files.
Let me know if there are any improvements or optimizations I can make to this approach."

## Prompt 3
Task: Create a new HrmDate record based on the structure of HrmEmployeeContract. Implement corresponding functions and services for HrmDate in both the Bouw and Infra folders, following the patterns of HrmEmployeeContractFunction. Ensure the following:
1.	Record Definition:
-	The HrmDate record should include properties for Date, Description, and Type.
-	Add appropriate JSON property annotations and ensure it is marked as [ExcludeFromCodeCoverage].
2.	Functions:
-	Create HrmDateFunction in both Bouw and Infra folders.-
-	Functions should handle Service Bus triggers and timer triggers, similar to HrmEmployeeContractFunction.
3.	Service:
- Implement HrmDateService in the Services folder.
- The service should include an UpsertAsync method for handling HrmDate objects.
4.	Testing:
- Add unit tests for the HrmDate functions and service.
- Ensure tests cover success and failure scenarios, as well as feature flag behavior for Infra.
5.	Configuration:
- Update Program.cs to register the new HrmDate service and retry session-based service.
- Add any missing constants to FunctionsConstants.cs (e.g., Service Bus topics and subscription names).
6.	Usings:
- Ensure all necessary namespaces are included in the new files.
7.	Output:
- Provide a detailed implementation plan, including file paths, class definitions, and method signatures.
- Highlight any assumptions or additional considerations.


