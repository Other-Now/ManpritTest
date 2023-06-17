# ManpritTest (Theory Part-A)
This is the repository for test submission

###  Question 1. Mention the working of Internet Website in Terms of Front-end & Back-end Divisions
Ans: A typical internet website has two major components: the front-end and the back-end. These components work together to offer users with a functional and engaging online experience. Here's a breakdown of how the front-end and back-end divisions work:

**The front-end** , also known as the client-side, is the section of a website that users interact with directly through their web browsers. It emphasises on the website's presentation and user interface. HTML (Hypertext Markup Language), CSS (Cascading Style Sheets), and JavaScript are key technologies used in front-end development.

Front-end developers are in charge of:

* Using HTML to create the structure and layout of online pages.
* CSS, which determines styles such as colours, fonts, and layouts, is used to improve the visual appeal of the website.
* Using JavaScript to implement interactivity and dynamic behaviour, such as animations, form validation, and user input processing.
* Responsive design strategies are used to optimise the website for multiple screen sizes and devices.

**Back-end** :
The server, database, and application logic that power the website comprise the back-end, often known as the server-side. It handles front-end requests, processes data, and conducts other actions to offer the necessary functionality. Back-end technologies include programming languages such as Python, Java, PHP, and Ruby, as well as frameworks such as Node.js, Django, Ruby on Rails, and Laravel.

Back-end developers are in charge of:
* Creating server-side apps that handle client requests and respond appropriately.
* Developing the business logic and algorithms required for the website's functionality.
* Connecting to databases, storing and retrieving data, and maintaining data security are all part of the job.
* Using external services or APIs (Application Programming Interfaces) to add functionality or access external data.
* Optimising the back-end system's performance and scalability to accommodate large traffic and user loads.

Communication between the front and back ends:
Front-end and back-end components exchange data using standardised protocols such as HTTP (Hypertext Transfer Protocol). The front-end sends a request to the back-end server whenever a user interacts with it, for as by submitting a form or clicking a button. The server processes the request, performs the necessary operations, retrieves or updates data from the database, and sends a response back to the front-end. The front-end then renders the response received from the back-end and displays it to the user.

###  Question 2. What are tags in HTML? Explain the each category of tag with an Example.
Ans: Tags in HTML are keywords that define the structure and content of a web page. They are enclosed in angle brackets (< and >) and usually come in pairs, such as <p> and </ p>. There are different categories of tags in HTML, such as:

* Document type declaration: This tag tells the browser what version of HTML the web page is using. For example, <!DOCTYPE html> is the tag for HTML5.
* HTML: This tag wraps the entire web page content. It has two subtags: <head> and <body>.
* Head: This tag contains information about the web page, such as the title, meta data, style sheets, scripts, etc. For example, <title>My Web Page< / title> sets the title of the web page.
* Body: This tag contains the main content of the web page, such as text, images, links, forms, etc. For example, <h 1>Welcome to My Web Page</ h 1> creates a heading with the text "Welcome to My Web Page".
* Structural: These tags define the layout and organization of the web page content. They include tags such as < div >, < section >, < article >, < header >, <footer>, etc. For example, < div id="main" >...< / div> creates a division with the id "main".
* Semantic: These tags provide meaning and context to the web page content. They include tags such as <p >, < e m > , < s t rong>, <a>, <i m g>, etc. For example, < p>This is a paragraph.< / p > creates a paragraph with the text "This is a paragraph".
* List: These tags create ordered or unordered lists of items. They include tags such as <o l>, <u l>, <l i >, etc. For example, <u l><l i>Apple</ l i><li>Banana</ l i><l i>Orange</ l i>< / u l> creates an unordered list of fruits.
* Table: These tags create tables of data. They include tags such as <ta ble>, <t r>, <t d>, <t h>, etc. For example, < t able ><t r><t h>Name</ t h><t h>Age</ t h></ t r><t r><t d>Alice< / t d><t d>25</ t d></ t r><t r><t d>Bob< / t d><t d>30< / t d></ t r>< / t able> creates a table with two columns and three rows.
* Form: These tags create forms for user input. They include tags such as <f orm>, <i nput>, <l abel>, <b utton> , etc. For example, <f orm action= "/ s ubmit" method="POST" ><l abel for="name" >Name:</ l abel><input type="text" id="name" name="name"><b utton type="submit">Submit</ b utton></ f orm> creates a form with a text input and a submit button.

### Question 3. Explain the working Procedure of Virtual DOM.
Ans: Virtual DOM is a concept that is used by some web frameworks, such as React, Vue.js, and Elm, to
improve the performance and efficiency of updating the UI.
Virtual DOM is a **lightweight JavaScript representation of the actual DOM** (Document Object Model),
which is the structure and content of a web page. 


Instead of directly manipulating the actual DOM, which can be slow and costly,
the framework creates a **copy of the DOM** in memory and renders the UI based on that.
Whenever there is a change in the state or data of the application, the framework updates
the virtual DOM first, and then compares it with the previous version of the virtual DOM.
This process is called **diffing**. The framework then identifies the **minimal changes** that
need to be applied to the actual DOM to reflect the new UI, and applies them
in a **batched** and **optimized** way. This process is called **patching**.

By using virtual DOM, the framework can avoid unnecessary and expensive DOM operations,
such as recalculating styles, layouts, and paints, and only update the parts of the UI that have changed.
This can result in faster and smoother user experience.

### Question 4:
Ans: MySQL and NoSQL are two types of database management systems with distinct methods to data storage and retrieval. Some important distinctions between MySQL (a relational database management system) and NoSQL (a non-relational database management system) are as follows:


Data Structure:

MySQL uses a relational data model, which organises data into structured tables with preset schemas. It maintains rigorous data consistency and facilitates cross-table relationships via foreign keys.
NoSQL databases use a variety of data models, such as key-value, document, columnar, and graph models. They provide flexible schemas that enable dynamic and unstructured data storage. Relationships between data entities are often not enforced in NoSQL databases.
Scalability:

MySQL: MySQL databases usually scale vertically by adding more resources to a single server (such as CPU, RAM, or storage) to handle increased data and user load. It supports replication for read scalability, but adding more write capacity can be challenging.
NoSQL: NoSQL databases are designed to scale horizontally by distributing data across multiple servers, also known as sharding. They provide built-in mechanisms for high scalability and can handle large amounts of data and high traffic loads more efficiently.
Query Language:

MySQL: MySQL uses SQL (Structured Query Language) for querying and manipulating data. SQL is a declarative language that allows complex queries, joins, and transactions.
NoSQL: NoSQL databases often have their own query languages or APIs that are specific to the data model they use. For example, MongoDB uses a JSON-like query language, while Cassandra uses CQL (Cassandra Query Language).
Schema Flexibility:

MySQL: MySQL enforces a fixed schema, meaning that data must conform to a predefined structure and adhere to the table schema. Any changes to the schema require altering the table structure.
NoSQL: NoSQL databases offer schema flexibility, allowing for dynamic and unstructured data. They do not require a predefined schema, and each record/document can have its own structure, enabling agile development and easy schema evolution.
ACID Transactions:

MySQL: MySQL provides strong support for ACID (Atomicity, Consistency, Isolation, Durability) transactions, ensuring data integrity and reliability.
NoSQL: NoSQL databases may have varying levels of transaction support. Some NoSQL databases sacrifice strict consistency guarantees in favor of higher scalability and performance, offering eventual consistency models or relaxed transactional guarantees.
Use Cases:

MySQL: MySQL is well-suited for applications that require structured data, complex queries, and strong data consistency, such as e-commerce platforms, financial systems, and content management systems.
NoSQL: NoSQL databases excel in scenarios with large-scale data, high-speed data ingestion, flexible schemas, and distributed data processing, making them suitable for real-time analytics, IoT applications, social media platforms, and content caching.
It's important to note that these are general differences, and the choice between MySQL and NoSQL depends on specific project requirements, data characteristics, scalability needs, and development preferences.

### Q5: Explain any one DBMS Technology in your own words.
I will explain mysql. <br>
MySQL is a popular database management system that helps store, organize, and retrieve structured data. It's like a digital filing cabinet where you can store information in tables and access it whenever needed. Let me explain it in simpler terms:

Imagine you have a collection of books, and you want to keep track of their details like title, author, price, and publication date. MySQL allows you to create a virtual "bookstore" where you can store this information in a structured manner.

In this virtual bookstore, you can create different tables to represent different categories of data. For example, you can have a "books" table to store book-related information. Each row in the table represents a specific book, and each column represents a specific piece of information about the book, such as the title, author, price, and publication date.

Using SQL (Structured Query Language), which is the language MySQL understands, you can perform various operations on the data. For instance, you can insert a new book into the "books" table by providing the details like the book's title, author, price, and publication date.

You can also retrieve information from the database. For example, you can ask MySQL to give you a list of all the books in the "books" table. You can even ask for specific books based on certain criteria, like books published after a certain date or books written by a particular author.

Additionally, you can update existing data in the database. For example, if the price of a book changes, you can ask MySQL to update the price in the corresponding row of the "books" table.

If you decide that you no longer need a book in the database, you can ask MySQL to delete that particular row from the "books" table.

MySQL offers many more features and capabilities, including handling large amounts of data efficiently, supporting complex queries, and ensuring data integrity. It is widely used in various applications ranging from simple websites to complex enterprise systems.
