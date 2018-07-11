# Describe the project will you be conducting and how your App will address the client’s needs.

Back2Bikes buy all their bicycle parts from one particular supplier. 

During customer's bicycle assesment the mechanic comes up with a list of parts that will be required to conduct the repairs. The qualification/sale process is most succesfull with being able to present the prices and details right there on the spot so the customer can make the decision, whether they would like to get the repairs done. At the moment, Back2Bikes exposeses their nett, wholesale pricing to the customers , which allows them to convert the sale on spot , however they are unable to introduce Retail Recommended Pricing which will increase the revenue of the foundation.

The solution is to create a full stack application that will pull the data from the supplier and render it on Back2Bikes own app in workshop. This way mechanics/volunteers can follow their known sale/consulting process with improving on margins that come from parts sales. 

The application will allow for searching via part number ( volunteers use in house, pysical catalogue for parts' number), name and description.

The solution includes creating Backend that will organise the data from the supplier and algorythms for rendering RRP on the Frontend. 



# Explain the different high-level components (abstractions) in your App.

The application will consist of backend which will pull the data from the supplier and serve it to the meteor's Frontend. 

### Front end will consist of: 
1. COMPONENT: List of parts (name, part number, description, image ... )
    1. COMPONENT: A card with for each individual part 

2. COMPONENT: search bar 
    1. COMPONENT: input field 
    2. COMPONENT: advanced filtering options 


# Provide an overview and description of your Testing process.

Test Driven Development (TDD) is essential. We write tests first. Testing can (and should be) done manually

Writing tests means the need for manual testing reduces (but never disappears completely).

We consider testing a bit like designing before you start coding. The test is like the design, or even a 'definition of done'. 

Once you have written some code, the test starts to be useful, because while it is failing, it tells you that you are not finished yet.

We write immutable (or stateless) code that is easier to test.

Write small components that do well defined things. It makes testing more powerful and useful. Complex components are a lot harder to test for which exposes you to unpredictable bugs in the future.

We use Jest for testing as well as we write stories using Storybook which covers a lot of testing as well. 

# Discuss methods you will use to protect information and data. 

Firstly we are using environment variables to store our keys securely.  Any sensitive data(supplier parts details) has not been included in the project on Github to make sure this information is not misused. Any members/volunteers are already using seceret pin number to check in for days work.
