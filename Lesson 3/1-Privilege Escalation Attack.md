### Privilege Escalation.
<pre>1. Horizontal vs Vertical Privelege Escalation.
2. Visible vs Invisible role based privilege escalation.</pre>

### <b>Privilege Escalation Testing Methods.</b>
<pre>1. Role based Testing Methodology.
2. Privacy based Testing Methodology.
</pre>

### Role based Testing Methodology 
<pre>1. Find all API endpoints.
2. Identify roles.
3. Try Privilege Escalation.</pre>

<pre>Privilege Escalation can be 
1. User to User.
2. Admin to Admin.
3. User to Admin.</pre>

<pre>In same excel sheet answer a question, how many roles are there.
E.g. facebook has pages, pages have role such as administrator, editor, moderator, etc.
So excel sheet will have.</pre>

|How many roles?|Multiple roles and tasks| 
|---------------|-------------|
|Administrator  |Admin of page. Page can have multiple admins.|
|Editor         |Can edit or create posts.|

Now completely focus on privilege escalation.

### Privacy based Testing Methodology

<pre>1. Find all API endpoints.
2. Identify privacy settings.
3. Try Privilege Escalation.</pre>

<pre><b>Note:</b> Privilege Escalation means accessing data which is not in our scope.
In same excel sheet answer a question, what are privacy settings.
A user to user privilege escalation is also as high as user to admin.
E.g. In a room booking app, unpublished rooms are only accessible by admin and other 
users can just view published rooms. So excalating privilege to access a unpublished room is a bug.</pre>