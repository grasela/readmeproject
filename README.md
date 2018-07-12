### THIS IS README ME ###
---

### 14. Provide User stories for your App.
**Volunteer Stories**
* As a bike mechanic, I need to be able to order parts quickly and easily so I have more time to fix bikes and help others learn to fix bikes
* As a unemployed cycling lover I like to volunteer at back2bikes to learn to fix bikes so that I can improve my skills and help the community. I get left alone while parts get ordered on our slow computer when I'd rather have help

**Shop Manager**
* As an experienced manager I don't want my process to change too much so I can continue building relationships with customers
* An an experienced manager I dislike our show ordering process, accessing a slow website on a slow computer as it takes too much time out of my day
* As an experienced manager I find it difficult to explain the price we charge to customers as they can see the wholesale price when we are putting an order through
* As a shop manager, I would like to save parts that need to be ordered throughout a day everyday so I can confirm the order with the wholesaler only once or twice a week at max
* As a shop Manager, I would like to review the order before I confirm it, so I can amend quantity and be able to remove items if they are not needed anymore
* As a shop manager, I would like to be able to quickly distinguish whether I am on searching parts page or reviewing order list so I don't waste my time looking for a parts in the wrong place
* As a shop manager I would like to be able to see the total wholesale price for the order, so that I can see if I am within spending budget
* As a new assistant manager I would like to quickly search for an item using item number and add it to shop ordering cart, so I don't forget to order it later

**Back2Bikes Owner**
* As the owner of the business, I would like to be able to see both the net price and wholesale price within the ordering system, so money in and out can be tracked easily
* As a business we need to earn money to pay our employed manager and cover costs such as delivery and gst so we can continue to survive and grow

**Customer**
* As a bike rider I enjoy the quality and friendliness of the back2bikes volunteers but feel like their ordering system is slow and confusing
* As an owner of many bikes I like to get my bikes fixed quickly and cheaply. I get confused when I see on the back2bikes ordering website that a price is $30 but they charge me $60
* As a customer, I would like to see the final price that it will cost me to fix/service my bicycle so I don't have to do any additional calculations myself
* As a customer I like transparent costing so I don't encounter any hidden costs later on

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

# # 3. Describe the client’s current setup and data.


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
A containerize platform that is designed to make it easier to create,deploy and run applications. By packaging up the parts needed such as libraries and other dependancies which is then deploys everything as one container.

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

The app will be deployed on Heroku. All builds and releases will be managed on Heroku.


# 10. Detail any third party services that your App will use.

There are no direct or obvious third party services used. However we are using: 
* React by Facebook
* Heroku ( Deployment )

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

