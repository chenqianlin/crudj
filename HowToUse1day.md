# Learn crudj in one Day #

Crudj is powerful because it can deal with the business model files. Requirements is the most important thing to the success of an app. How to analyse requirements and how to design the system structure accordingly are the two emphasiss of software industry. We are not along. Many genius have worked hard in this field, they invent many theories, methods and tools. Some are good, and some aren't. Crudj have absorbed the the thinking of DDD/MDD, and strictly obey the rule of layed development. What's more, it seperate the business model files from the code, and take upon it self to generate the app from the model files directly. <br />

# DSL file #
In crudj, business model files has ".dsl" extension, that is the abbreviation of "Domain Specialist Language". It is a text plain file. You can open it by windows Notebook.<br />
The picture below show one dsl file in Exampl1:<br />
![http://wiki.crudj.googlecode.com/git-history/master/img/dslContent.jpg](http://wiki.crudj.googlecode.com/git-history/master/img/dslContent.jpg)<br />

All dsl files are in the sub path of the configuration file.(If you know nothing about the configuration file, please study it in the linkage here: <a href='http://code.google.com/p/crudj/wiki/HowToUse1hr'>Learn crudj in one hour</a>)<br />
The picture below show the dsl file structure in Exampl1:<br />
<pre>
${example}<br>
|<br>
|__学生管理<br>
|   |<br>
|   |__学生.dsl<br>
|   |__班级.dsl<br>
|<br>
|__师资管理<br>
|   |<br>
|   |__老师.dsl<br>
|<br>
|__config.properties<br>
<br>
</pre>

The dsl file is not permitted in the same directory with the configuration file. Because dsl files' path structure build the menu in the app. Each dsl file should under the sub-directory of the directory that contains the configuration file.<br />
The picture below show the relation between dsl file path structure and the menu in Exampl1:<br />
![http://wiki.crudj.googlecode.com/git-history/master/img/dslPathToMenu.jpg](http://wiki.crudj.googlecode.com/git-history/master/img/dslPathToMenu.jpg)<br />

One dsl file, one list view page. The file name had better be simple, and express the business meaning accurately. This is important for the view page to show the information.<br />
The picture below show the dsl file name "学生" used in the different view pages in Exampl1:<br />
![http://wiki.crudj.googlecode.com/git-history/master/img/dslNameToView.jpg](http://wiki.crudj.googlecode.com/git-history/master/img/dslNameToView.jpg)<br />

One dsl file, one model POJO...

# property type #
There are seven types of property supported by version 1.0. They are integer, float, string, long string, date, enum, user define class. The table below show the relation of the type between java class and html control shown on the view page.<br />
![http://wiki.crudj.googlecode.com/git-history/master/img/ptype.jpg](http://wiki.crudj.googlecode.com/git-history/master/img/ptype.jpg)

# enum type #
...

# class type #
...

# run time package #
...

<br /><br /><br />

<a href='http://code.google.com/p/crudj/wiki/HowToUse1week'>to next one week's learning</a>
<a href='http://code.google.com/p/crudj/wiki/HowToUse'>Back to Index page</a>