# Inventory Management System for College Clubs
A Full-Stack Web Application to facilitate sharing resources in college clubs. Clubs have resources that any of their members can borrow upon request. Members can borrow resources when approved by the convener of the club.

Three roles exist, namely, Admin, Convenor and Member.
- Admin - Can give roles and add new clubs & members
- Members - Can request for resources following a request-approval flow
- Convener - Can approve/reject member requests, update the club inventory
	
The roles and their respective permissions can, however, be extended. Each user can be a part of multiple clubs and exercise different roles in each of them. All this is made possible by a custom role-permission framework.
 
It also supports email notifications to different stakeholders
<br>

<h3>Virtual Environment</h3>

- `pip install virtualenvwrapper-win`
- `mkvirtualenv test` &nbsp; _test = name of virtual env_

<h3>Install required packages:</h3>

- `pip install -r requirements.txt`<br>
- _After ensuring that we are in a virtual environment (If not, use `workon test`)_

<h3>To run project:</h3>

- `python manage.py makemigrations`
- `python manage.py migrate`
- `python manage.py runserver`
- Visit development server at http://127.0.0.1:8000

<h3>Create Super user:</h3>

- `python manage.py createsuperuser`
- Enter desired credentials

<h3>To see emailing features</h3>

- Visit https://www.wpoven.com/tools/free-smtp-server-for-testing
- Enter the desired email to see the inbox</p>

<h3>Admin Site:</h3>

http://127.0.0.1:8000/admin

<br>

<h3>Implemented Features</h3>
<ul>
    <li>Member
        <ul>
            <li>View club items</li>
            <li>Request for items</li>
            <li>View request status</li>
            <li>View statistics about their requests </li>
        </ul>
    </li>
    <li>Convenor
        <ul>
            <li>View all members of club</li>
            <li>View club items</li>
            <li>Add, Update items</li>
            <li>View member requests</li>
            <li>Approve/Reject requests</li>
            <li>Validation of quantity of requested item</li>
            <li>View statistics pertaining to the club</li>
        </ul>
    </li>
    <li>Admin
        <ul>
            <li>View all clubs, users, items and requests</li>
            <li>Add new club(s)</li>
            <li>Add, Update items</li>
            <li>Add new user or existing users to clubs</li>
            <li>Delete users</li>
        </ul>
    </li>
    <li>Authentication and page restrictions</li>
    <li>Reset, Change Password</li>
    <li>Email respective users about request flow</li>
</ul>
<br>
