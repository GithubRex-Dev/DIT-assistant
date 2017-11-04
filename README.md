# DIT-assistant GrangeMobile
hybrid mobile app 

Introduction 
As part of the mid-term assignment for social media application, this report includes the documentation of all the requirements for the grangeMobile application. Mainly, jQuery Mobile will be used to the application for UI layout and event handling features. 

1.	User Definition & Use Case 
For this application, I have chosen student as the main user. And use cases listed below will provide explanations of how user will interact with the application.  
1.1 Use Case 1: The student interacts with the application to view one specific module detail.  
Having accessing to the home page, the student taps on one option called module. The app display a list of modules with a search filter to quickly search for a specific module by names. Student selects one module out of them, and the app displays the information of the module, which includes its name, website, address, and the credit it is worth. 
 
1.2 Use Case 2: The student interacts with the application to view the message from his lecturers.
The application provides a function by which student can view the message from his DIT lecturers. Once student taps on “Message” in the home page, the application displays an overview page containing a list of message received. Student can filter messages by key words of message through the search filter. Student selects one specific message, and the app displays a detail page including the sender, the time, the title and the content of this message.
 
1.3 Use Case 3: The student interacts with the application to view his lecturers’ information.  
The “Lecturers” option in home page allows student to check the information about his lecturers related to his major. Once the student taps on this option, a list of lecturers’ name is displayed. Student taps on a specific name, the detail information is displayed, which includes their department and location and email address. The students can tap on the email address to contact this lecturer. 
 
1.4 Use Case 4: The student interacts with the application to find a book in school’s libraries. 
The home page offers the student access to visit library of DIT online to find the book he or she want to borrow. Once student taps on the option “Library”, the page which allows student to search the book by its name through a search filer and displays the address of each library of DIT is created. If the student gets the result he wants, and tap on it, the detail of the book, which includes the title and availability, is displayed. Student can go to corresponding library to broow the book.  

 		 

2.	Behaviours & Prioritisation of Behaviours 
The section will define the behaviours and accociated data, for each use case. And based on this, the behaviours involved will be prioritised based on their perceived importance. 
2.1 Behaviours for Use Case 1(The student interacts with the applicatiocn to view one specific module detail) 
Use Case 1 has two behaviours:
•	GetModuleslist: to list the modules student has been enrolled in. 
•	GetModuleDetail: to display the details of specific module when selected 
Behaviour	Input Data	Output Data
GetModuleslist	Student No. (primary key)	List of Module Name, Module Code (invisible, primary key)
GetModuleDetail	Module Code	Module Location, Classroom, Credits, Website


2.2 Behaviours for Use Case 2(The student interacts with the application to view the message from his lecturers)
Use Case 2 has two behaviours:
•	GetMsglist : to list the messages sent to student. 
•	GetMsgDetail: to display the content of the message selected 
Behaviour	Input Data	Output Data
GetMsglist	Student No. (primary key)	List of message including sender, sending time and subject, msg index(invisible)
GetMsgDetail	msg index (primary key)	Content of message 

2.3 Behaviours for Use Case 3(The student interacts with the application to view his lecturers’ information)
Use Case 3 has two behaviours:
•	GetLecturerlist : to list the lecturers related to the student. 
•	GetLecturerDetail: to display the detail of the lecturer selected 
Behaviour	Input Data	Output Data
GetLecturerlist	Student No. (primary key) 	List of lecturers Name, and their Staff No. (invisible, primary key)
GetLecturerDetail	Staff No. (primary key)	Department, office and email address of lecturer selected 


2.4 Behaviours for Use Case 4(The student interacts with the application to find a book in school’s libraries)
Use Case 4 has three behaviours:
•	GetBookslist: to get a book list stored in local storage or from library database
•	GetBookWantToFind: to type the book’s name in search filter to retrieve in the book list
•	GetBooksDetail: to display the detail of the book selected 
Behaviour	Input Data	Output Data
GetBookslist		List of book including name, press, library, copies, code
GetBookWantToFind	     Book name 	Specific book  
GetLecturerDetail	Code (primary key)	Name, press, library and copies,  

2.5 Prioritisation of Behaviours
Out of the four use cases, to view message should be in the top of priority, since messages are from lecturers and important to student. Since student’s duty in school is study, knowing the details of the lectures they attend is very important. So, the next priority goes to viewing details of module. Lecturers’ information can be useful to student, but it is not quite much needed to student. Then viewing the detail of lecturer follows viewing module detail. Finding books makes many conveniences for student. Alternatively, student can go to library check the book information in library and to borrow the book they have to be in library in person. Finding books is the last in the list. For each use case, the behaviours are closely connected and depend on each other. Therefore, the sequence among them has been fixed. 
Based on the statements above, the list of Prioritisation of behaviours is as follows:
Priority	Behaviour	Use Case
1	GetMsglist	Viewing Message
2	GetMsgDetail	
3	GetModuleslist	Viewing Module
4	GetModuleDetail	
5	GetLecturerlist	Viewing Lecturer
6	GetLecturerDetail	
7	GetBookslist	Finding books
8	GetBookWantToFind	
9	GetLecturerDetail	

Conclusion 
Based on the app design requirements outlined in this report, the application and its user interface will be developed using jQuery Mobile. It will be made available as a NetBeans project.
