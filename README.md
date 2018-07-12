
# 3. Describe the client’s current setup and data.


### React JS 
Used in the front-end. This front-end framework will allow us to segregate all of our on-screen components letting us combine them into a well-designed UI for the user. Manipulation of component props and state will be updated in real-time so load times are much less.

### MongoDB
 Used as the Database. Mike from Back2bikes has already set up his existing web-app with mongo and for consistency we will do the same. MongoDB is a table-less database and stores data in JSON-like documents.

### Meteor
A full-stack javascript platform. It includes different libraries for building connected-client reactive applications. It allows us to develop in javascript across all environments, i.e. application server and web-browser.

### Semantic UI 
A modern front-end development framework that provides a sleek, subtle, and flat design look that provides a lightweight user experience. It uses minimal and neutral styling which allows ample room for customization.

### Story Book
A development environment for UI components. It Helps visualize the states of UI components and develop them interactively. Storybook runs independantly, it is does not have specific dependancies and requirements.

### Docker
A containerize platform that is designed to make it easier to create, deploy and run applications. By packaging up the parts needed such as libraries and other dependancies which is then deploys everything as one container.

# 8. Describe the architecture of your App.

The architecture of our app consist of a front-end and a backend. 

### Back-end
In the backend we are using MongoDB Database. Although MongoDB is schema-less database and is document orientated, it is good practice to constrain the contents of the collections to conform to a known format. 

That way we do not need to write defensive code to check and confirm the structure of the data as it _comes out_ of the database, instead of when it _goes into_ the database. The logic behind creating a schema in a document-orientated database is because we tend to _read data_ more often you _write it_.


*Parts schema and Order schema*

![b2b_db_design](./assets/b2b_db_design.png)

### Front-end
We are using React on the front end to render components on the client side.  
We use _Minimongo_ library which creates a local cache in the front-end allowing that allows us make live-updating database queries.

### App Architecture

Meteor initializes code from the _Client and Server_ directory. Both _Client and Server_ will point to the configuration files in the _startup_ directory and load all the code.

*The app's main architecture is made up client, server and imports .*
```
server/
client/
imports/
    startup/ 
        server/ 
        client/
    api/ 
    ui/
```

*App Flow*

![App Flow](./assets/app_flow.png)


### Deployment 

** Heroku?? Discuss with team **


# 10. Detail any third party services that your App will use.

There are no direct or obvious third party services used. However we are using: 
* React by Facebook
* Heroku ( Deployment ) ????

# 16. Describe the way Tasks are being allocated and tracked in your project.
### Agile
Agile methodology is used in many software development environment, we have stand ups every morning and record them into our trello board. 

#### Trello 
We used Trello, a project management tool to allocate and track key milestones in our project and Nuclino, a workflow management tool.

### Internal Team Trello Board
- Tasks filled on cards are required for planning phase.
- List down all tasks that needs to be completed.
- Use trello color labels to allocate task to each team member.
- Dedicated columns (swim lanes) for completed tasks.
- Summaries of Agile standups.

![Team Trello Board](./assets/teamtrello.png)

### Back2Bikes (Client) Trello Board
- Collaborative board with client.
- Consist of tasks of the development phase. 
- Tasks include features that are inspired from user stories and user pains.
- Columns (swin lanes): Backlog, Ready, In-progress, Dev Done, QA, Done

![Team Trello Board](./assets/b2bparttrello.png)

## Nuclino
Each member should reflect, track and manage the workflow to ensure that we are maintaining consistency with the standards provided by the client. Using all the dev tools will be important for collaboration and achieving efficiency.

Stndards
* Filenaming
* Component names
* Collection names
* Coding style

Workflow
* Git
* Test Driven Development
* Agile
* Trello Board
* Git- Branching strategy

![Team Trello Board](./assets/nuclino.png)

### THIS IS README ME ###
---

### 5. Identify and describe the software (including databases) to be used in your App.

* **React**
  * React is a front-end framework to help build websites through segregated components. We can then combine these components to create a UI that is fast, reactive and functional. We will be using react to create Back2Bikes Parts ordering system alongside Meteor.
* **Meteor**
  * Meteor is a full-stack JavaScript platform, which allows development in one language (JavaScript) across all environments. There are a few key components that make meteor unique, such as:
    * Meteor doesn't send HTML over the network. The server sends data and lets the client render it.
    * The database methods are available everywhere. You can   use these within the client and the server.
    * Meteor prefetches data and simulates models to make it seem like server method calls are returned instantly.<br/>
* **Visual Studio Code**
  * Visual Studio Code is a source code editor. It includes support for debugging, embedded Git control, syntax highlighting, intelligent code completion, snippets, and code refactoring. This is our standard text editor, but some may opt to not use it.
* **Storybook**
  * Storybook is a development environment for UI components. It allows you to browse a component library, view the different states of each component, and interactively develop and test components. We will be using this throughout our testing phases before pushed to production.
* **Figma**
  * Our standard for designing and will be used to create our wireframes. Figma is a free software that makes wireframing very easy with the ability to create components and reuse them in our design however we like.
* **Nuclino**
  * Nuclino is a cloud-based team collaboration software which allows teams to collaborate and share information in real-time. We will be using this to share information that will stay the same throughout the length of the project, such as coding standards and git workflow practices.
* **Trello**
  * Trello is a collaboration tool that organizes your projects into boards. In one glance, Trello tells you what's being worked on, who's working on what, and where something is in a process. We will be using this throughout the project to track who is working on what and what is being worked on, so there is no overlap.

* **MongoDB** is the database used in our application. Our client already uses this so we will continue to do the same for consistency.
---

### 11. Identify the database to be used in your app and provide a justification for your choice.

**MongoDB** is the database used in our application. Our client already uses this so we will continue to do the same for consistency.

Using a MongoDB data model lets us represent hierachical relationships, data arrays and other complex structures we may need to take advantage of during development.

---

### 17. Discuss how Agile methodology is being implemented in your App.

We will work as an agile team. This means:
* Sprints (1 week)
* Aim for Minimal Viable Product (MVP)
* From the Agile Manifesto:
  * Working code over documentation 
  * Individuals and Interactions Over Processes and Tools
  * Customer Collaboration Over Contract Negotiation
  * Responding to Change Over Following a Plan

Other agile gems:
* Frequent delivery of working software 
* Fail quickly (or don't be afraid to fail and change course)

How do we do this? 
* Use Trello as our Kanban board for the sprint
* Work on one thing at a time
* Talk about what it is, and how to do it
* Challenge the story

---

### 22. Research what your legal obligations are in relation to handling user data.

The GDPR is the most official guidelines regarding handling of personal information.
The GDPR states: if we are to store personal data we are to disclose the fact that we are doing so, or not do so at all. No personal data may be processed unless it is done under a lawful basis. Users of the application may request a copy of the personal information collected in a common format, and may have the right to delete any data upon request.

Because we are only creating an application based on making orders and will only be used by staff of the company, we will not have to worry about the GDPR guidelines.


## 4. Describe the project will you be conducting and how your App will address the client’s needs.

Back2Bikes buy all their bicycle parts from one particular supplier - Bicycle Wholesale Australia. 

During customer's bicycle assesment the mechanic comes up with a list of parts that will be required to conduct the repairs. The qualification/sale process is most succesfull with being able to present the prices and details right there on the spot so the customer can make the decision, whether they would like to get the repairs done. At the moment Back2Bikes exposeses their nett, wholesale pricing to the customers , which allows them to convert the sale on spot , however they are unable to introduce Retail Recommended Pricing which will increase the revenue of the foundation. They usually try to explain to the customer additional costs (GST, freight etc) however it is a timeconsuming and awkward process.

The solution is to create a full stack application that will pull the data from the supplier and render it on Back2Bikes own app in workshop. This way mechanics/volunteers can follow their known sale/consulting process with improving on margins that come from parts sales. 

The application will allow for searching via part number ( volunteers use in house, pysical catalogue for parts' number), name and description.

The solution includes creating Backend that will organise the data from the supplier and algorythms for rendering RRP on the Frontend. 



## 9 Explain the different high-level components (abstractions) in your App.

The application will consist of backend which will pull the data from the supplier and serve it to the Meteor's Frontend. 

### Front end will consist of: 
1. COMPONENT: List of parts (name, part number, description, image ... )
    1. COMPONENT: A card with for each individual part 

2. COMPONENT: search bar 
    1. COMPONENT: input field 
    2. COMPONENT: advanced filtering options 


## 19. Provide an overview and description of your Testing process.

Test Driven Development (TDD) is essential. We write tests first. Testing can (and should be) done manually

Writing tests means the need for manual testing reduces (but never disappears completely).

We consider testing a bit like designing before you start coding. The test is like the design or even a 'definition of done'. 

Once you have written some code, the test starts to be useful, because while it is failing, it tells you that you are not finished yet.

We write immutable (or stateless) code that is easier to test.

Write small components that do well defined things. It makes testing more powerful and useful. Complex components are a lot harder to test for which exposes you to unpredictable bugs in the future.

We use Jest for testing as well as we write stories using Storybook which covers a lot of testing as well. 

## 21 Discuss methods you will use to protect information and data. 

Firstly we are using environment variables to store our keys securely.  Any sensitive data(supplier parts details) has not been included in the project on Github to make sure this information is not misused. Any members/volunteers are already using seceret pin number to check in for days work.


## 1. Who is your client?

back2bikes is a social enterprise, providing bicycle training, repair and recycling services for the local community, asylum seekers and refugees.

back2bikes is run by volunteers, and is supported by Port Phillip Council.

They are looking for:

*  New volunteer mechanics (no skills required)
*  New volunteers to promote them
*  Donations of usable bikes and parts
*  Bike servicing

They offer:

* Quality secondhand bikes for sales
* Cheap servicing and parts
* (Paid) Maintenance courses
* Free training for volunteers
* Bikes for refugees and asylum seekers

We are happy to be involved with an organisation that helps the community and is not for profit.

## 2. What is your client’s need (i.e. challenge) that you will be addressing in yourproject?

Back2bikes buy all of their parts from one supplier, Bicycle Parts Wholesale and they do not provide RRP (Recommended Retail Price) to them.
At present they can't hide the trade price from the customer when looking at their web site. 

http://www.bicyclepartswholesale.com.au/page/10/product-catalogues

Bicycle Parts Wholesale (BPW) publish a glossy colour catalogue, which is essential when placing orders, as the photos on the web site and the descriptions are not always adequate to work out which part to order.

Back2bikes have a XLSX file of their database. It is simply a list of a part number, a short description and a bar code number. No category or sub-category information is available.

So we need to do the following:

* Import the parts list and prices to our (Mongo) database
* Provide a simple page (within their existing Meteor app) to allow searching of the database, either by name or part no
* Write an algorithm to calculate a RRP
* Display the price of the part(s) found as a list
* Provide an advanced search option

### Possible extension: 

* Allow part to be added to a draft order, with a quantity
* Review draft order, add/remove parts
* Send order to supplier (via email)
* BPW will send them updates to the price list regurarly. An update process should allow an import of the new XLSX file, but it should be checked to make sure that 1) The number of items should be +/- 10%, average prices should also be +/- 10%

All to be done using React, Storybook, TDD

### Pricing algorithm

* The first calculation is to double the wholesale price to make RRP. 
* This helps to cover GST and shipping costs.
* Anything over $60, the margin is 50%
* Anything over $100 the margin is 30%

## 7. Identify and describe the infrastructure (i.e. hardware) that your App will run on.

Even though our app will be deployed online, it will primarily be accessed from just one computer in the back2bikes workspace. The App will not be hosted on a local server but deployed to the cloud. 

The app will exist online, hosted by the back2bikes current site. They already run an attendance web app that the volunteers use to sign in and out when they are in attendance. Our app will integrate into this seamlessly.

## 18. Provide an overview and description of your Source control process

### Git branching strategy:

- master

The master branch corresponds to the code that is currently in production. Every time we do a deployment to production, we put a tag in git, so that we have a way to go back to a particular release (in case we ever need to). This branch is protected to prevent accidental updates

- develop

The develop branch corresponds to the code that is currently on the staging server. Similarly these versions are tagged in git when we deploy them, and the branch is also protected.

- feature/xxx branches

Feature branches are for developing particular features, for example a feature to add a part to an order might be named feature/order-add-part. 

All branches should be created from develop.  You should never create a branch from another , unless there is a dependency on code in that branch.

- fix/xxx branches

If you are making changes to address a bug that is not urgent, you should use a branch name like fix/xxx. This change will go through the regular release workflow just like feature changes.

- hotfix/xxx branches

If you are making changes to address a bug that is urgent, and needs to be installed without delay, then you can use the hotfix prefix. The branch should be created from the master branch, as it will be merge directly into master, and deployed from there. This workflow is unusual, and does not follow the regular release procedure. It should be limited to small changes, to minimise the risk of failure.

