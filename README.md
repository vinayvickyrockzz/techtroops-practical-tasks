# techtroops-practical-tasks
Admin and Developement Tasks
User Administration:

1.	Create 10 User account with different user names and Id's fill the complete form and observe all the fields in user table
2.	Create 2 groups ( servicenow support, salesforce support)
3.	 Add 5 users in 1st group, add 5 users in the 2nd group
4.	Check the functionality of roles, Administration, ITIL, itil_admin,ESS by giving to different users
5.	Check the locked out and active checkbox functionality
6.	Check the impersonate functionality
7.	Check the possibility to add roles to users and groups check the behaviour
8.	Check how to add user to group from user record, how to add user to group from group.
9.	Create 2 Roles named as ( brillio_problem, brillio_change) for brillio_problem assign problem application, For brillio_change assign change application give this roles to different users and test the access.
10.	create 1 role names as brillio_IPC  give incident,problem,change application access by using contain roles option.
11.	Create one new company,department,location from the respective tables and add to users.
12.	check the functionality of the delegate user
13.	 Check the functionality of the Override application menu roles checkbox in the module.
14.	Create a role named as prb_createnew that should give access only to the create new module in the problem application, other module access should not come with this role.
15.	Create one elevated role named as brillio_elevate that should give access to system security applications only whenever the user is elevated.
16.	Create one role named IPC_open  that should provide access to all incidents, problems, and change applications Open module only.
17.	 Create a role named as brillio_resolved that should give access to resolved incidents only to the users and should be an elevated role.
18.	 create 1 role names as brillio_IPC  give incident,problem,change application access by using contain roles option. for this requirement make this role as elevated and check whether elevated functionality works or not.
19.	Create a role named as brillio_selfservice that should restrict self service application.
20.	Check the functionality of impersonator role
21.	Check the functionality of timezone and Date format fields in the user table.
///////////////////////////////////////////////////////////////////////////////////////////////////////////////
Tables :

1.	Create table with all field types and observe the functionality of all fields
2.	Create table by Replicating Incident table 
3.	Create 2 custom tables to extend the other table
4.	Observe the schema map of different tables.
5.	Create 2 choice fields: country,state add the choices and check the dependency.
6.	Check the dot walking for the caller and assigned to fields in the incident table
7.	Create a filter of software category records to visible software groups.
8.	Create a filter 'active true,category network,state new. and make it visible to everyone.
9.	create a dot walking in the incident for caller, Assignment group,Configuration item.
 caller - mail, Mobile phone,Manager
 Assignment group - Description, manager 
            configuration item - Location, Assigned to,Model ID. 
10.	Create a filter without the network category, and the state is new or in progress and make it visible to the hardware group .
11.	Observe the Schema map.
12.	Observe the dictionary override functionality.
13.	Create a filter with a state new and Category network this filter should be visible only to the users Part of the network group.
14.	1. Create 2 tables named as copy of incident, copy of user same like OOB user and incident form.
15.	2. Create a table by unchecking the create module checkbox and observe the functionality
16.	3. Create a table by adding to the existing incident application.
17.	4. Create fields by using form layout, form design and form builder
18.	5. check the functionality of these field types Field types:
19.	String,reference,choice,list,image,url,wiki,date,date/time,true/false,currency create fields in 3 ways
20.	Create a dependency On the table create two choice fields Operating system and Os Versions
Operating system - Windows,Ubuntu,Linux,Mac OS .
OS Versions : 2007,windows10,windows11,Ubuntu 21.10,Ubuntu 20.04.3 LTS,Gentoo,Debian,Big Sur,Monterey
for selection of 
⇒ Windows -2007,windows10,windows11
⇒ Ubuntu - Ubuntu 21.10,Ubuntu 20.04.3 LTS,
⇒ Linux - Gentoo,Debian,
=>Mac OS - Big Sur,Monterey
21.	create a dot walking in the incident for caller, Assignment group,Configuration item.
22.	 caller - mail, Mobile phone,Manager
23.	Assignment group - Description, manager 
24.	configuration item - Location, Assigned to,Model ID. 
25.	Create a filter without the network category, and the state is new or in progress and make it visible to the hardware group .
26.	Create one table named as Brillio Parent with (name(string-display-true),Phone(string-readonly),Manager(reference-user-mandatory),Email
27.	create 2 child tables Brillio child1, Brillio child2, check the functionality by extending brillio parent.
28.	Check the dictionary override functionality with above tables try to override read only, mandatory, display, default value,dependency values.
29.	Create related list of incident, problem, in the brillio parent table
30.	Create an auto-number for brillio parent table .
31.	1. Create one table named as Wipro students with columns:
32.	Name(string),Phone(string),Email(string),Qualification(Choice).
33.	Create 2 user accounts (Sai , Ramu) and 2 Roles(internal, external). And add internal to Sai, external to Ramu, Create at least 15 records with your batch data.
34.	2. Create a custom role named as ‘ServiceNow’, create all table level ACL to ServiceNow roles.
35.	3. Provide this ‘ServiceNow’ role to Both Ramu and Sai.

36.	 Give All fields read access to internal role and Phone field read access to external role, Check what access Ramu will get , What access to Sai will get.
37.	Create one more user named shiva with XYZ role, Give write access to the name field. Check how sai and Ramu behavior changes on the name field.
38.	Check if we can add multiple roles in the same ACL.
39.	I want to ensure that Ramu can read only name,phone.
40.	I want to ensure Sai to read only qualification and Email fields.
41.	I want to give delete access only to the Sai.
42.	Give name field write access only to itil.
43.	Prove application access and Table level access is different, By giving different roles table acl’s and application & module.
/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
Update sets:

1.	Local updateset
2.	Merge update sets functionality
3.	Updatesourse and Export Import  process testing.
4.	Backout update set functionality.
5.	Parent or Batch update functionality.
//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
Email Notifications:

1.	Create inbound action for New, Reply, Forward.
2.	Create new type inbound action for ITIL users only.
3.	Create new type inbound action for Abel tuter only.
4.	How to eliminate guest user in incident caller when you create inbound action from the mail which is not present in the user table
5.	Create new inbound action for problems whenever a user sends email from not registered mail it should create one user account in the user table.
6.	Create a reply inbound action for the problem table with problem statement as email subject, Category as software, and description should update with email body.
7.	Create Forward inbound action for problems to create new records.
8.	Create a new inbound action for any custom table to create a new record.
//////////////////////////////////////////////////////////////////////////////////////////////
requirement:1
 
Create a outbound notification in incident table for caller, cmdb asssignedto person,akrc701@gmail.com,callerdepartmenthead.
Whenever short description contains security word.
 
With Subject: Notify users -RPS
Body:
Hi Team,
Security ticket has been created please check the details.
 
Short description :
Description:
Configuration item :
 
 
thanks
requirement 2:

2. Create notification on incident table when caller is VIP and category is network to the users of network group and Caller manager with 
Subject: VIP caller ticket
Body : Hi Team,
VIP user raised the ticket please address this ASP please make it as priority 1 ticket.

Requirement 3:


Check the inbound actions functionality and do research on the inbound actions.

Requirement 4:

8.Create a notification on incident table When Configuration item is Asset IBM or Annie IBM, TO the configuration item Assigned to person, Network group. with
Subject : CI related ticket (Number) is create
Body : Hi ,
Ticket Number(INC0000123) ( ticket number should come hyper link) is created please work on the ticket.
3. Create a notification on event is fired and triggered explore this.

4. Check the inbound actions functionality, new , reply forward


Assignment rules:
—--------------------------------

1. Check the existing Priority lookup rules for both incident and problem table.
2. Delete the existing Priority lookup rules and create the rules again for priority.

3. Add new choices for the impact fields - very high and very low create few new rules based on new choices in the incident.

4. Create new assignment look up rule for Brillio parent table matcher fields are - Category, designation and Assignment group and assigned to should be matcher fields.

5. Research on Exact lookup match field.

6.Create assignment rules for the incident table based on impact and Configuration item.
7.Explore the run on form change, insert , update in the data lookup definition.


SLA Requirements:

1.	Test whether we can design SLA for a Custom table.
2.	SLA for Hardware - hardware group  - priority 1 - Pause on onhold - Stop on Resolved/Closed - (8-15)hongkong - 2 hours
3.	SLA for Hardware - hardware group  - priority 2 - Pause on onhold - Stop on Resolved/Closed - (8-15)hong kong - 4 hours
4.	SLA for Hardware - hardware group  - priority 3 - Pause on onhold - Stop on Resolved/Closed  - (8-15)hongkong- 8 hours
5.	SLA for Hardware - hardware group  - priority 4 - Pause on onhold - Stop on Resolved/Closed  - (8-15)hongkong- 16 hours
6.	SLA for Capacity Mgmt - Capacity management- Priority 1 - Pause on onhold - Stop on Resolved/Closed - (10-17) US/central  - 1 hours
7.	SLA for Capacity Mgmt - Capacity management - Priority 2 - Pause on onhold - Stop on Resolved/Closed  - (10-17) US/central - 3 hours
8.	SLA for Capacity Mgmt - Capacity management - Priority 2 - Pause on onhold - Stop on Resolved/Closed  - (10-17) US/central - 7 hours
9.	SLA for Capacity Mgmt - Capacity management - Priority 2 - Pause on onhold - Stop on Resolved/Closed  - (10-17) US/central - 18 hours
10.	SLA for Help Desk - Helpdesk - Priority 1 - Pause on onhold - Stop on resolved/closed - (9-16) Europe/Brussels- 4 Hours
11.	SLA for Help Desk - Helpdesk - Priority 2 - Pause on onhold - Stop on resolved/closed - (9-16) Europe/Brussels - 6 Hours
12.	SLA for Help Desk - Helpdesk - Priority 3- Pause on onhold - Stop on resolved/closed - (9-16) Europe/Brussels- 8 Hours
13.	SLA for Help Desk - Helpdesk - Priority 4 - Pause on onhold - Stop on resolved/closed - (9-16) Europe/Brussels - 10 Hours
14.	SLA for Help Desk - Helpdesk- Priority 5 - Pause on onhold - Stop on resolved/closed  - (9-16) Europe/Brussels - 2 days

Reports Requirements:

1.	Name : Group Manager - Incidents by Assignment
Description:
Create a report for the incident table on state New,onhold,In Progress based on assignment group manager.
Type : Bar
2.	Name : Incidents created by Belgium users
Description:
Create a report for the incident table on the users created by belgium users.
Type: List
3.	Name : Incident Trending from Jan 2016 to today
Description: Create a report for the incident table records created from 2016 to till now.
Type : List
4.	Name : Open Incidents by Priority
Description: Create a report for the incident table on the priority basis.
Type : Pie
5.	Name : HardwareIncidents - Last 30 days
Description : Create a report on an incident table for a hardware group created in the last 30 days.
Type: Heatmap
6.	Name : Incidents Opened Today
Description : Create a report on incident table opened on today
Type: Single sore
7.	Name : All Incidents Closed By (My Groups)
Description : Create a report on the incident table closed by assignment group where logged in user part of.
Type: Bar
8.	Name : Incidents not updated for 7 days
Description : Create a report on incident table which were not updated since 7 days
Type:  Sigle score
9.	Name:  Incidents related to Causing Changes
Description : Create a report on the incident table which is causing change.
Type: List
10.	Name : Unassigned Incidents 
Description : Create reports on the incident table that are not assigned to any user.
Type : Sigle score
11.	Create a dashboard and attach all these reports to it.
//////////////////////////////////////////////////////////////////////////////////////////////////////////
Client scripts : 

1.	Populates the logged-in user automatically in the caller field only for new Records.

2.	If a logged in user has an itil role, make the description ,channel mandatory.

3.	Display the info message for the new record of the incident with “This is the new record of the incident (incident number ex: INC12345).

4.	Create a Custom Role named as internal_tsb ,add it to the user.Disable Attachment feature on incident form if the logged in user is holding a custom role.

5.	If the logged in user is abel tuter set the configuration item as AssetIBM, and description set with ‘’This is abel tuter ticket please take as priority to resolve’, It should work with new record only.

6.	Autopopulate logged in user in the opened on behalf of variable in variable set of your catalog project.

7.	Hide task SLA related list in the incident for category network records.
8.	Hide task SLA related list for the Users holding Admin Role.

9.	Hide all related Lists for the tickets with category hardware tickets.

10.	If a user changes the caller in the incident form : Description should be the incident is created by the user : caller full name , cmdb mandatory,state should be in progress.

11.	Populate the description in the incident with contact type - email.phone,walk-in,self service,If drop down changes value should change accordingly.
12.	Create Two checkboxes  named as Analysis review and Analysis approved If analysis review is true, Analysis approve should be true automatically and vice versa.

13.	Create a dropdown named as “Related Section” with 3 options by including none with values like Approvals,Governance, Ticket metrics. Create 3 sections named as Approvals,Governance, and Ticket metrics. Display the section based on the Dropdown selection.


14.	Restrict form submission if the assignment group and assigned to is not filled.

15.	Restrict the incident table category from hardware in the list show alert message Security Restrictions cannot edit.

16.	Restrict the change of state to “in progress” from the list if the user has an itil role.

17.	Populate alert messages while submitting the form with category software. If the category is software ,set the values in the description as “this is software ticket”.

18.	On the catalogue item create two select box variables Operating system and Os Versions
Operating system - Windows,Ubuntu,Linux,Mac OS .
OS Versions : 2007,windows10,windows11,Ubuntu 21.10,Ubuntu 20.04.3 LTS,Gentoo,Debian,Big Sur,Monterey
for selection of 
⇒ Windows -2007,windows10,windows11
⇒ Ubuntu - Ubuntu 21.10,Ubuntu 20.04.3 LTS,
⇒ Linux - Gentoo,Debian,
⇒ Mac OS - Big Sur,Monterey

19.	When assigned to is empty, please make urgency mandatory.

20.	If the caller is abel tutor , make the description field mandatory.

21.	Set impact field mandatory if priority is changed to critical.

22.	If caller id is fred luddy restrict form submission.put an alert.

23.	If the description field is empty, set the contact type as self service else change the contact type to ‘walk in’.

24.	If the problem field on the incident form is empty, restrict form submission.put an alert.

25.	 If category is none hide sub category field on form.

26.	 Population assigned to Joe employee when contact type is phone.

27.	If the role is admin it should not allow a short description to edit the list.
28.	If the caller is abraham lincoln set the category to hardware and Remove phone choice in Channel field.

29.	When an incident is assignedTo someone show an alert message(this ticket is assigned to the assigned name).

30.	When a login user is ITIL populates the Help Desk group.

31.	Based on the choice selection checkbox should be checked,
Knowledge checkbox should be checked if the priority is 1.

32.	Take two fields Requested For and Manager, If requested for selected Manager should populate accordingly.

33.	Should not allow users to change the category to network in the list view. Display error message when user tries to change (You cannot change the category to Network). 

34.	If analysis review checkbox checked state should move to inprogress.Else it should be a new state.

/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
Glide Record:

1.	Insert a record in the user table with Userid as tech, phone num as 9999999999.

2.	Create a custom role ‘’ Tsb_snow’’, Assign this role to all the users in servicenow. By using Background script.

3.	Update the records in the user table of gender female,mobile phone empty,department empty with department sales, mobile phone 1234567.

4.	Working with isValidRecord () method Determines if a record was actually returned by the query/get record operation.

5.	Query the incident table with assignment group empty and category inquiry help, description empty update these records short description with –Updated from TSB.

6.	Get the change records numbers whose change type is emergency. And print the numbers and its count.

7.	Print all incidents where the category is software and the sub category is the operating system.

8.	Get incident records of putting a filter which was created between the last 6 months?

9.	Update all category network and assignment group empty tickets to Network assignment group and description with this ticket assignment group is updated from Administrator and it should not trigger any notification.

10.	Change all in progress tickets of software category to resolved, It should not impact system fields and it should send notifications to users.

11.	Change recently updated 2 tickets which are Resolve state tickets to closed but it should not trigger any notifications and it should not impact system fields.

12.	Query all empty configuration item tickets updated with AnnieIBM.

13.	Get the problem records where the resolution code is not empty.

14.	Get change records where model and assigned to is empty.

15.	Get change records where justification and implementation plan is empty.

16.	Get the records of incidents which are of priority high and category software limit it 10.
17.	Get all problem tickets associated with incidents?

18.	Update all incident records where caller is joe employee with abel tuter.

19.	Create a new change request for type is emergency and along with a short description and assigned to whatever you want.
20.	Delete records from the problem table if they are closed.
21.	Delete records on incident if category is none and priority is low and assigned to is empty.

22.	Create four incident records with short description in increment manner like first incident short description should be -Hi Incident created by me 1 and the second record should have Hi Incident created by me 2 and goes on…
23.	Print the numbers category hardware or category network tickets. - addOrCondition().

24.	Delete problem records which are created today.

25.	Update the recently created 10 records of caller abel tuter and category inquiry records with assignment group hardware and assigned to empty.

26.	Update Last created 5 records of category inquiry and assignment group empty records with Helpdesk assignment group.

27.	Get the count of records based on priority 2 and state is new print it in the output.

28.	Query incident records where category is one of hardware and network ,priority is 2 get the Link of it and publish it in description.

29.	Close all change requests where conflict status is not run and CI is empty with priority as 4.
30.	Create a template on problem table and create problem ticket with the template you created. 
31.	Create two templates on problem and incident , insert records at same time on two different tables.
32.	Query incident table with priority is critical and category is network check attachments are present if yes print attachment exists ,if not print attachment does not exist....

33.	Move all on hold incident tickets to in progress.

34.	Update incidents which are having problem records with category as network and a short description as ‘incident as problem related ticket’.

35.	Update the related problem record priority as high from the incident record.


//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
Business Rules :
1.	Prevent users from creating duplicate incident records with the same short description.
2.	Automatically capitalize the short description field before saving an incident.
3.	Ensure that only administrators can modify the priority field in existing incidents.
4.	If the caller is a monitoring system, automatically set the state to "Closed" before saving the incident.
5.	Do not allow updates to records in the "Closed" state.
6.	Incident should not be closed if it is in a new state.
7.	If priority 1 incident creates , Create an associated problem ticket with the same short description.
8.	Automatically create a follow-up task when an incident is moved to the "Resolved" state.
9.	After creating or updating an incident, update the corresponding change request to reflect the change's status.
10.	only allow users with the "admin" role to see incident records with priority "1" (Critical).
11.	Show only active records for non-admin users.
12.	Prevent users from seeing their own records if the incident state is "Closed."
13.	Only allow users to view incidents belonging to their department.
14.	Only allow users to view high-priority incidents (priority 1 and 2) unless the user is in a specified "Support Team" group, in which case they can see all incidents.
15.	Show records within the last 30 days and prevent querying records older than this time.
16.	Prevent the deletion of incidents that are in the "Closed" or "Resolved" state.
17.	Prevent the deletion of an incident if any related task (e.g., change request, problem) exists.
18.	Prevent deletion if there are pending approval records associated with the incident.
19.	Check the current value of state, if current value is not equal to previous value then set impact high .(Before Br)
20.	Restrict form submission if description and assignment group is empty.(before insert/update).
21.	Create a location field in the incident table. It should refer to the location table. If the user fills the wrong location of the configuration item it should show an error message and it should not update or insert the record.(before-insert/update).
22.	If the user is having Admin role show only priority 1, category-hardware, state - new tickets. (before - query).
23.	If priority 1 incident creates , Create an associated problem with the same short description.(after insert)
24.	When Problem is created related Incident state change to “On hold” and onhold reason “Awaiting problem” – afterBR(insert,update)
25.	Attach a child incident to any incident, when the parent incident short description is changed the child incident short description should also be updated.(after - update).
26.	Use any Catalog item which we have created. When a Catalog item is submitted create a record in one custom table with the values in the variables.(after -insert).
27.	Change contact type to phone if the Category is Software. (update).
28.	Update the associated change request assignment group with the problem record assignment group from the problem record .
29.	Show caller email id, company, mobile number and manager when form loads.(display).
30.	Close the related incident ticket from problem form when the problem is closed.
31.	While closing the change ticket, Please check change tasks, If tasks are not closed it should not close the parent change ticket and show an error message ''tasks are not closed please close the tasks before closing the change’’ .(before - update)
32.	Show number of incident tickets for caller id when before submitting the form.(display Br) & on submit
33.	Create change task on change record when change record is closed the related change task should also close.
34.	Create one date field named as follow up time if the date in followup time is less than current time, It should not allow update and insert the record, Show error message please select future date.(before ,insert/update)
35.	Create a change task when the change request is moved to scheduled state and the category is hardware.(after,update).
36.	When an incident is resolved, automatically close all related incidents. This can be a costly operation if there are a lot of related records.
37.	Auto populate the comments from the parent incident to child incident.
38.	Create Incident task when incident is created with Critical priority and task should assign automatically to the assignment group manager and change the ticket to inProgress.
39.	Write a script to close active RITMs when Related catalog tasks do not exist OR All catalog tasks are closed.
40.	If a user in his profile has position equal to non-agent , position is a custom field in the user table and the user has ITIL role,remove ITIL role for the user.
41.	If a user in his profile has position equal to agent , position is a custom field in the user table, add ITIL role to the user.
42.	Change the short description of a problem ticket 30 minutes before a time set in a custom date/time field.
-	Event - After Business Rule- Script Action
43.	Turn off the notifications to all users with a script.
-	Gliderecord - scheduled job
44.	Prevent users from deleting important Configuration Items (CI) marked as critical.
45.	When a task is created under a change request, certain fields like `description` should be copied from the parent to the child task.
46.	Only users with the "admin" role should be able to update impact, urgency fields in the incident table.
47.	Restrict users from creating more than 5 incidents in a 24-hour period.

/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
Script Includes : 

1.	Create 1 checkbox field named as 'approved', and create one date and time field named as 'Time stamp', If the user checks the checkbox it should populate the current date and time, If he unchecks it should clear.
2.	Set the value Assigned to in the incident table with configuration item assigned to whenever the configuration Item changes.
3.	Create a Nokia company and add it to any VIP user When creating an incident  form, if the user is VIP and belongs to Nokia company, show an alert message while form loads (“The requestor is a key leader from Nokia DIGITAX ”).
4.	Auto Populate requester for information in requester for variable set.
5.	Take a field assigned to me on the incident form and populate it with the caller name.
6.	Set assignedTo with caller department Head name, When caller name changes.

Ui Actions : 
1.	Create a button named as "set p1", once it is clicked change the priority 1.

2.	Create a button name is “Assigned to Me” and the functionality is that when you click on an assigned button then the logged in user name should get populated in “Assigned To”  available in the incident form.

3.	create a button on incident form (name: close child). When the user clicks the button, all child incident tickets should close.

4.	create a button on incident form (name:Create child).When the user clicks the button, Create a new child incident for the current record. It should show automatically on the related list(stay on current record).

5.	Create a button on the list named as ‘sendRemainder’ ; it is visible only to hardware group users. It should trigger notification to assigned_to user whenever the user selects the record and clicks on the button. 

6.	Create Button with 'watch list' populate the watch list field with caller id on clicking the button.
7.	Make an UI Action visible only when the logged in user is an admin, and has more than 5 records where he/she is a caller.
- UI Action- GlideRecord - Script Include 




Scheduled Jobs:
—---------------------------------------------------

1.	Automate the removal of obsolete or inactive records (e.g., incidents in a "Closed" state for over 6 months).
2.	Send reminders every hour for pending approvals older than 24 hours.
3.	Generate a report of weekly activity (e.g., resolved incidents) and email it to stakeholders.
4.	Order the catalog item everyday at 6PM.
5.	Identify and notify record owners about stale tasks (e.g., tasks untouched for over 30 days).
6.	Notify users 7 days before their password expires.
7.	Automatically escalate critical incidents that haven't been updated in the last 2 hours. Assign automatically to ‘critical incident group’.
8.	Automatically close change requests in the "Implemented" state for over 14 days.
9.	Notify owners to review knowledge articles that haven’t been updated in 12 months.
10.	Write a script to close active RITMs when Related catalog tasks do not exist OR All catalog tasks are closed.


Reference qualifiers:
—------------------------------------------

1.	If a logged in user is a member of any of those 5 groups then show all groups including those 5. If a logged in user is not a member of any of those 5 groups then show all groups excluding those 5 groups.
2.	We need all the Active users in the Caller Field and all users must belong to the IT Team only.
3.	I want the VIP user available in the Caller Field of Incident Table.
4.	Show users in the caller field who belong to the same department as the logged in users department.
5.	Show only open changes in a related Change Request field.
6.	We want to show/filter the users in the caller field whose location is the same as the Value of Location in the Incident Form.

Email Scripts:
—-------------------------------------
1.	When a caller is inserted new incident trigger notification and shows them total incidents count created by caller and provides the link to see the existing incidents  
2.	Get the Count of Problem tickets Assigned to.
3.	Arrange the data in table format in email body .  






22.	Create 10 Users 
23.	Create 2 groups ( ericson_internal, ericson_External)
24.	Create 2 Roles named as ( ericson, ericson_elevate) for techtroop assign incident application, For ericson_elevate assign problem application access with elevate checkbox true. 
- give Ericsonrole to 1 st group, eicson_elevate to 2nd group, check how it will work by login to the different groups.
///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
