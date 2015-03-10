# DatabaseProject
##Student
#####Attributes:  
the student number,   
name (first and last name),   
phone number,   
alternate phone,   
home address (street, city, postcode),   
date of birth,   
sex,   
category of student (for example, first year undergraduate, postgraduate),   nationality,   
smoker (yes or no),   
special needs,   
any additional comments,   
current status (placed/waiting),   
course the student is studying

If the student is a family student, then names and dates of birth for family members to reside in housing are also stored. Information about next of kin for a student is stored as well (relationship, address – street, city, postcode, and contact telephone number). 

##Housing Options
Types:accommodation for---   
full-time single students,    
couples,   
families

####Residence halls:   
######Attributes:    
name,    
address,   
telephone number,    
and a hall manager who supervises the operation of the hall. 

A hall provides **single rooms** each with a room number, a place number(key), and monthly rent rate. 
The place number **uniquely identifies** each room in all halls controlled by the Housing office and is used when renting **a room to a student**.

####Apartments: 
are either general **student apartments or family apartments** and are all fully furnished. General apartments provide **single-room** accommodation for groups of **three or four students**.    
#####1.student apartments:  
an apartment number(key),  
address,   
and the number of single bedrooms and bathrooms available in each apartment.    
The apartment number **uniquely** identifies each apartment.  
  
Each **bedroom** in a apartment has:    
a monthly rent rate,   
room number,   
and a place number.    
The place number **uniquely** identifies each room available in all apartments and is used when renting a room to a student. 
#####2.Family apartments:
are rented as a whole and are either **one, two or three bedroom apartments**. They have similar information stored as other apartments except for slight differences such as rate is for entire apartment, and they **do not have place numbers.** 

*The housing office also maintains of private accommodation - from rooms in shared houses, to apartments and family homes, for students who prefer to live off campus in the local community. However, this is not an option available to freshmen.*

***Students may rent a room in a hall of residence or apartment. Only university students and approved guests are eligible for university housing. Some specific residence halls are open to only graduate students and upperclass students. ***


##Leases

A student may rent a room in a hall or student flat for various periods of time. 

New lease agreements are negotiated at the start of each academic year with a minimum rental period of one semester and a maximum rental period of one year, which includes Semesters 1, 2, and the Summer Semester. Students submit a request for accommodation along with up to three housing preferences (specific halls, or alternative housing options). The request is given a status of Pending and entered into Housing Office’s request list. If it is approved, its status is changed to Processed, and after it is signed by student, the status is changed to InProgress and after lease is over it is changed to Completed.  

Each individual **lease agreement** between a student and the Accommodation Office is **uniquely** identified using a lease number. The data stored on each lease includes:    
the lease number,  
duration of the lease (given as semesters),   
name and matriculation number of the student,   
place number,   
room number,   
address details of the hall or student apartment,  
the date the student wishes to enter the room,  
the date the student wishes to leave the room (if known). 

Information about the terms of lease agreement is also included such as:   
payment schedule options,   
monthly or once a semester,   
security deposit,   
penalty for early lease termination. 

*Early termination penalty* is certain percentage of the remaining lease before cut-off date after which the entire amount of remaining rent is the penalty. 
To terminate a lease, a student sends a request with a reason and the date he/she wants to terminate. A termination **request** passes through the similar states as a lease request, pending, processed and completed. As part of processing a lease termination request, an inspection date is included to determine any incidentals or damages and to assign fees. Relevant information about the termination request is stored and given a **unique** request number.

##Parking
The university accommodation also offers students parking using some dedicated **parking lots** that each have a limited number of **parking spots**. Each parking lot is identified by a **unique** number and a list of nearby housing options is associated with each parking lot. Parking spots are identified uniquely globally and some parking spots have special classification, handicapped, small car, large car and bike and each have different rental fees. As part of a lease **request**, a student may request a parking spot, denote if a special classification is needed and if a non-nearby spot assignment will be accepted. A parking spot nearby the student’s assigned housing option with the right classification is selected if possible and **a unique parking permit id** is assigned.   
*Parking for housing students is only available to campus residents.* Students may also opt for the more general student parking lots. The parking spots are given based on the availability and “first come first serve” basis.

##Invoices
A student is issued an invoice monthly and includes at least two lineitems: the monthly housing rent, monthly parking rent and then a total. If the student opted for a single semester payment, then only a single invoice in the first month of lease. (Additional lineitems may also be added on the invoice by the housing administration such as late fees, or other incidental charges etc). Each invoice has a unique invoice number which is stored along with associated information such as lease number, payment due, due date, student’s full name and number, place number, room number, and name of hall or apartment. Additional data is also held on the payment of the invoice and includes the date the invoice was paid, the method of payment (check, cash, credit card, etc.). A final invoice is generated at the end of lease and it deducts any pending late fees, penalty, and damage charges from initial deposit. Each student should be able access a list of all invoices and status, paid or billed.

##Maintenance
In case of any problem in the apartment, students should be able to raise a ticket for maintenance. When a student accesses the maintenance ticketing options, a list of ticket types are presented. In the system, each ticket type is associated with a severity, Low, Medium and High (not displayed to student) and a ticket with a unique number and associated information (type, date, student, location) is stored. Tickets are inserted into a ticket list in order that they are received but ordered by severity (i.e. higher severity tickets will be placed higher on list but after earlier same severity tickets) 


##Housing Office Staff
Some information is also held on members of staff of the Housing Office and includes the staff number, name (first and last name), home address (street, city, postcode), date of birth, sex, position (for  example, Hall Manager, Administrative Assistant, Cleaner) and location (for example, Housing Office or Hall). Housing staff can access the list of pending lease, lease termination requests, and maintenance tickets and process them (approve, enter inspection date, damage charges, change status of tickets, etc). The information about which staff took any action on a lease or ticket and date is stored. 





