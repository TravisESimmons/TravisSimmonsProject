# Deliverable 1 - Project Setup

This portion of the lab consists of setting up the structured solution, documentation, and functioning code for required entities and DAL layer.

> **Remember to [reference your issues](./Deliverable-1.md)** when committing your work through this deliverable.

## Required Projects

Your solution must be a client-server solution consisting of multiple projects as outlined in the course. The Presentation Layer portion is to be an ASP.NET Web Application (**.NET Core** Razor Pages). The BLL, Entity classes and DAL portions of the system are to be placed in a separate class library project.

## The StarTED Database

The database supplied for this lab is an SQL Server database named "StarTED". The following is a sample of the connection string that may be used for the Presentation Layer.

```json
  "StarTEDDb": "Server=.;Database=StarTED;Trusted_Connection=true;TrustServerCertificate=True;MultipleActiveResultSets=true;",
   "StarTEDRemoteVpnDmitDB" : "Server=DMIT-Capstone1.ad.sast.ca;Database=CPSC1517_1221_yourSection_yourNaitUserName;User Id=yourNaitUsername;Password=RemotePassword.yourNaitStudentId;TrustServerCertificate=True;MultipleActiveResultSets=true",
    "StarTEDRemoteDmitDB" : "Server=CAPSTONE1.dmit.sast.ca;Database=CPSC1517_1221_yourSection_yourNaitUserName;User Id=yourNaitUsername;Password=RemotePassword.yourNaitStudentId;TrustServerCertificate=True;MultipleActiveResultSets=true",
```

In creating the entities for tables from the database, **only create for those tables related to your specific scenario** (deductions may be applied if you create additional entities). You are encouraged to generate the entities and the database context class using [reverse engineering](https://docs.microsoft.com/ef/core/managing-schemas/scaffolding?tabs=dotnet-core-cli#specifying-tables).

## The Forms

There are two pages for the core functionality of this project (described below). Create the pages with appropriate header text describing the page (the functionality of these pages are to be completed in subsequent deliverables). You must name the pages **Query** and **CRUD**. In addition, you must [edit the **Index** page](#default-page) of your web application. All of these pages must use the same [layout](#layout-and-styling).

### Layout and Styling

You are expected to decide upon the styling approach for your site (Holiday, Bootstrap, awsm.css, Tailwind, etc.) and put some effort in to make your content look presentable. In addition, your layout page must contain the following elements:

* **Site Navigation** – Links to all the pages in the web application.
* **Scenario Title** – The number and name of the scenario (e.g.: G1 – Reservations by Group).
* **Student Name** – Your first and last name.

### Default Page

Your default (**Index**) page must contain the following elements (each with their own heading):

- **Deliverable Descriptions** – A brief description (one or two paragraphs) of the `Query` and `CRUD` page's requirements in the project, identifying the name of the page and its purpose, along with any unique constraints or characteristics of the page's behaviour.
- **Known Bugs** – A bulleted list of all the known bugs and incomplete portions of the lab.
- **Entity Relationship Diagram** - The ERD diagram of your specific scenario (you may copy the one from your specific scenario description).
- **Site Styling Decision** - Indicate what [site-wide styling](#layout-and-styling) you are using in your website.

----

## Evaluation - *5%* – Scenario Number: ________

> ***NOTE:** Your code **must** compile. Solutions that do not compile will receive an automatic mark of zero (0).*
>
> If you are unable to get a portion of the assignment to compile, you should:
>
> - Comment out the non-compiling portion of code
> - Identify the non-compiling portion in the **Incomplete Requirements** heading, noting the item's
>   - File name (e.g.: "Account.cs")
>   - Line number(s)
>   - Compiler error number and general message

Your assignment will be marked based upon the following weights. See the [general rubric](./ReadMe.md#generalized-marking-rubric) for details.

| Weight | Deliverable/Requirement |
| ---- | --------- |
| 2 | Creation of Projects |
| 2 | EF Core DAL/Entities |
| 1 | Project References and Configuration |
| 2 | Layout and Styling |
| 2 | Default Page Documentation |
| 1 | Placeholder Pages for Query and CRUD |
| ---- | --------- |
| **10** | **Total Weight** |

<!--

- Project Architecture & Code Quality
  - [ ] Client-Server architecture (multiple projects inside a single solution)
  - [ ] Master Page with functioning site-master based navigation, Scenario Title and student's name
  - [ ] Appropriate Entity CRUD class
  - [ ] Requested annotation for Entity CRUD class (Table, Key, NotMapped, DatabaseGeneration)
  - [ ] Appropriate validation annotation for Entity CRUD class (Required, StringLength)
  - [ ] Appropriate Entity support classes (if required for your scenario)
  - [ ] Requested annotation for Entity support classes (Table, Key, NotMapped, DatabaseGeneration)
  - [ ] DAL class with appropriate code for all the required tables
- Configuration
  - [ ] Proper references have been setup between projects.
  - [ ] web.config file has the correct entry for connection strings
  - [ ] DAL class sets database initializer to null (preventing automatic table creation by EntityFramework).
  - [ ] Your DbContext class references proper connection string.
- Lab Documentation (Web Form)
  - [ ] Requested Lab documentation placed as the home page for the web application (Default.aspx)
  - [ ] List of known bugs & incomplete portions of lab
  - [ ] Entity Relationship Diagram of selected scenario
- CRUD – Single Item CRUD
  - [ ] Blank form with title of selected option in the student's scenario and page banner title.
  - [ ] Content page Title set to CRUD - StarTED
- Query – GridView
  - [ ] Blank form with title of selected option in the student's scenario and page banner title.
  - [ ] Content page Title set to ODS - StarTED
- Site.master
  - [ ] Menu with working links to the Home and CRUD/Query pages
  - [ ] Your name in the menu brand portion of the site navigation

-->
