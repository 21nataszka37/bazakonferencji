# bazakonferencji
Here is all the code needed to create a properly functioning database, conveniently divided into four main files:<br />
<b>1. DLLcode</b><br />
This file contains code to create all the tables, foreign keys and constraints. You may adjust some of the constraints if you wish - e.g. limits of participants or characters allowed in strings - however we do recommend leaving constraints concerning creating past and future events, the prices and ensuring uniqueness of certain data as they are.<br />
<b>2. Procedures</b><br />
This file contains all the procedures that have been written for the database. Mostly, they provide more friendly and convenient interface for executing certain actions, although they may also be used as an access restriction. One of the most unusual is Reservations_Per_Week, created especially for cleaning ladies, which aside from showing reservations for the next seven days, automatically assignes rooms if they have not been assigned yet.<br />
<b>3. Triggers</b><br />
While most of the triggers works as intertable constraints, assuring intergrity on many levels, there is one written especially for the Accounting Department, which automatically copies identifier of payment to Enrollment table. Apart from just easing the operation of inserting payments, it also allowes us to deny access to the Enrollment table.<br />
<b>4. Views</b><br />
All the views that may possibly come in handy while using the database. Generally, they were created to be used by clients or participants, who may want to know what conferences they are enrolled for and if their personal data is correct. There are however two or three that should be used by staff exclusively.
