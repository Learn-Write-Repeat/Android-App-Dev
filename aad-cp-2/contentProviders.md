<h1><p align="center">Working with ContentProviders in an android application</p></h1>
<br/>
<h3>Introduction: -</h3>
<hr/>
<br/>
So, what a Content Provider actually is? So, lets take a look into it. If you ever have worked with Native android development then you might have used databases such
as firebase or backendless. But have you ever wondered what if you used a SQLlite database?. Native android development with JAVA/Kotlin supports SQLite database. Now 
to implement SQLite Database Content Providers are something that comes handy and makes your work easy.
<br/>
<br/>

*""In Android, Content Providers are a very important component that serves the purpose of a relational database to store the data of applications. The 
role of the content provider in the android system is like a central repository in which data of the applications are stored, and it 
facilitates other applications to securely access and modifies that data based on the user requirements.""*
<p align="right">-GeeksForGeeks</p>
<br/>
<br/>
So, basically a content provider is something you could say a central storage of data for different apps. Now let's take a look into what are the different operations
we can perform using Content Provider.
<br/>
<br/>
<h3>Operations in Content Provider:-</h3>
<hr/>
These are the following operations available generally termed as CRUD operations(Create, Read, Update, and Delete) - 
<ul>
<li>Create: Operation to create data in a content provider.</li>
<li>Read: Used to fetch data from a content provider.</li>
<li>Update: To modify existing data.</li>
<li>Delete: To remove existing data from the storage.</li>
</ul>
<br/>
Basic working of Content Providers - 
<br/>
<br/>
<img src="https://www.tutorialspoint.com/android/images/content.jpg" align="center"/>
<br/>
<br/>
<h3>Content URI</h3>
<hr/>
By now you all must have heard about a Uniform Resource Identifier(URI). So,a URI nothing but basically a string that provides a unique address (either on 
the Internet or on another private network, such as a computer filesystem or an Intranet) where a resource can be found. So then what is a content URI?
<br/>
Content URI(Uniform Resource Identifier) is the key concept of Content providers. To access the data from a content provider, URI is used as a query string. So, basically
Content URI allows you to access the data in the data base and interact with it with the help of queries, basically similar to the way using which we used to interact 
with the SQL database.
<br/>
<br/>
These are the following parts of Content URI - 
<ul>
<li>content:// – Mandatory part of the URI as it represents that the given URI is a Content URI.</li>
<li>authority – Signifies the name of the content provider like contacts, browser, etc. This part must be unique for every content provider.</li>
<li>optionalPath – Specifies the type of data provided by the content provider. It is essential as this part helps content providers to support different types of data that are not related to each other like audio and video files.</li>
<li>optionalID – It is a numeric value that is used when there is a need to access a particular record.</li>
</ul>
<br/>
<br/>
<h3>Working-</h3>
<hr/>
Components like Activity and Fragments send query requests to ContentResolver using an object CursorLoader.The ContentResolver object 
sends requests (like create, read, update, and delete) to the ContentProvider as a client. After receiving a request, ContentProvider process 
it and returns the desired result. 
<br/>
<br/>
<h3>Methods- </h3>
<hr/>
The different methods of the class which implements Content Provider are - 
<ul>
<li>query() - A method that accepts arguments and fetches the data from the 
desired table. Data is retired as a cursor object.</l1>
<li>insert() - To insert a new row in the database of the content provider. 
It returns the content URI of the inserted row. </l1>
<li>update() - This method is used to update the fields of an existing row. 
It returns the number of rows updated.</l1>
<li>delete() - This method is used to delete the existing rows. 
It returns the number of rows deleted.</l1>
<li>getType() - This method returns the Multipurpose Internet Mail Extension(MIME) 
type of data to the given Content URI.</l1>
<li>onCreate() - As the content provider is created, the android system calls 
this method immediately to initialise the provider.</l1>
</ul>


