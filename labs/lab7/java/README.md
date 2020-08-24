# COSC 304 - Introduction to Database Systems<br>Lab 7: Building a Database-enabled Web Site using JSP

**For this assignment, create a directory `Lab7` on `cosc304.ok.ubc.ca` under your home directory in the folder `public_html/tomcat/`.**

## Example 1

Here is the code to show "Hello World!" using JSP:

```
&lt;html&gt;
&lt;head&gt;
&lt;title&gt;Hello World in JSP&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;

&lt;% out.println("Hello World!"); %&gt;

&lt;/body&gt;
&lt;/html&gt;
```

[Click for a demonstration of the Hello World code](http://cosc304.ok.ubc.ca/rlawrenc/tomcat/Lab7/HelloWorld.jsp)

The URL of the JSP file is: `http://cosc304.ok.ubc.ca/rlawrenc/tomcat/Lab7/HelloWorld.jsp`

We can modify this code either by being logged in to `cosc304.ok.ubc.ca` and editing it with `nano` or by editing the file on our local machine and transferring it to `cosc304.ok.ubc.ca`.

Try and change the code so that the output looks like this:

# Hello World Again!

<pre>
1
2
3
4
5
</pre>

[Click here for a demonstration of the Hello World Again code](http://cosc304.ok.ubc.ca/rlawrenc/tomcat/Lab7/HelloWorldAgain.jsp)

### [Solution - HelloWorldAgain.jsp](code/HelloWorldAgain.jsp)

## Example 2

[Example code](code/JdbcQuery.jsp) to query the workson database and return some answers in a table.  Make sure that the url is `jdbc:mysql://cosc304.ok.ubc.ca/workson` and put in your user id and password.

## Example 3

Modify the sample JSP code for querying WorksOn such that for each department you list its projects and then its employees.  The output should look like <a href="http://cosc304.ok.ubc.ca/rlawrenc/tomcat/Lab7/WorksOnDeptEmpProj.jsp">this (click here)</a>.

### [Solution - WorksOnDeptEmpProj.jsp](code/WorksOnDeptEmpProj.jsp)


## Example 4

You can pass and receive parameters between JSP pages.  An example is to create an HTML form that collects user input and then passes this information to a JSP file to perform the query and return the answers.

### [Query Form Example](code/QueryJSP.html)

### [JSP Code for Performing Query](code/EmpQuery.jsp)


## Example 5

Create your own query form for the WorksOn database. Your form should have boxes for the Employee name and Project name that accept partial matches (using `LIKE '%queryString%'`).  The JSP file should receive the parameters and create a query that lists all WorksOn records where the employee name and project name are as specified.  Show the count of the # of records at the bottom of the page.  An [example query form and system](http://cosc304.ok.ubc.ca/rlawrenc/tomcat/Lab7/WorksOnQuery.html) is available.

### [Solution - HTML File](code/WorksOnQuery.html)

### [Solution - EmpProjQuery.jsp](code/EmpProjQuery.jsp)

## [Lab 7 Assignment](assign/)
