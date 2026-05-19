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




22.	Create 10 Users 
23.	Create 2 groups ( ericson_internal, ericson_External)
24.	Create 2 Roles named as ( ericson, ericson_elevate) for techtroop assign incident application, For ericson_elevate assign problem application access with elevate checkbox true. 
- give Ericsonrole to 1 st group, eicson_elevate to 2nd group, check how it will work by login to the different groups.
///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
