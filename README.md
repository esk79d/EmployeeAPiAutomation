# EmployeeAPiAutomation
This is sample solution in C# .net. It validates various Rest API methods of Employee APi (i.e https://dummy.restapiexample.com/)

#Brief Description of the Solution

1.  I've used BDD approach to create the Test scenarios and implemented the logic in Step definitions.
2. I've tried to keep the code generic by creating Helper and Model classes.


#packages used in this Solution

"NUnit" Version="3.13.2"
"SpecFlow" Version="3.9.22"
"SpecFlow.NUnit" Version="3.9.22"
"SpecFlow.Tools.MsBuild.Generation" Version="3.9.22"


#Steps to import and run the solution

Step 1: Un-zip the file and Import the given Solution. 
Step 2: Open Test Explorer in visual studio by Test->Windows->Test Explorer 
Step 3: Install the relevant packages mentioned above via Tools -> NuGet package manager -> Manage NuGet packages
Step 4: Run the Tests from Test Explorer
Step 5: Once the Test execution is completed, a detailed Test Report will be generated under "Test results" folder 

Notes:

1. I've noticed that this Test API (i.e https://dummy.restapiexample.com/) is inconsistent.
While sending the requests, It gives the below error intermittently instead of a valid response
{StatusCode: 429, ReasonPhrase: 'Too Many Requests', Version: 1.1, Content: 
Sometimes it gives 500 (Internal Server error)

2. The solution can also be implemented usig RestSharp to handle the Http Requests and Responses more easily.
I've intentionally avoided using RestSharp just to showcase a different way of handling the Http Requests and Responses

3. This solution can be enhanced further by providing a config file to feed in the urls and other input data rather than having them in Code. Also an external logger file can also be added to produce more meaningful logs which can help to debug any test issues / failures
