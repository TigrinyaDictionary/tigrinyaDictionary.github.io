---
layout: post
title: 404 Gender not found
description: This post explains how DVLA are subtly insensitive to gender identity
---

# DVLA ARE GENDER INSENSITIVE!!!

Now that I've got that out the way I can explain to you why I think that.

I recently worked on a project for making it easier to verify and approve drivers, en masse, for businesses that require it. As part of the project I had to build a licence "verification" tool to prevent drivers from inputting wrong details or licence numbers into the system. The tool works by creating its own licence number from the user's personal details and comparing it with the number they provided - If there's a match then the system can continue on to the next step, otherwise throw a big red "invalid" message back to the user.

The licence number is derivable from the personal information due to the way DVLA designed it - This can be found [here](https://www.gov.uk/government/uploads/system/uploads/attachment_data/file/518243/INS57P-information-on-driving-licences.pdf). In a nutshell, each driving licence number has a 16 digit long unique sequence of characters and is constructed using the following rules:<br/>

1.  1-5th The first five letters of your surname. If surname is less than five characters in length,
the remaining spaces will comprise of the digit 9.
2. 6th The decade digit from the year of birth.
3. 7-8th the month of birth. Add 5 to the 7th character if driver is female
4. 9-10th The date of birth
5. 11th The year digit from the year of birth
6. 12-13th The first two initials of your forenames. The second character will comprise of
the digit 9 if no middle name
7. 14-16th Usually 9, Computer check digits

<br/>

**Note: For our purposes we can discard the last 3 digits and work with the rest**

So after reading that, do you see any problem with how the number is generated?  
.......................... go on, take your time ..............................  
................ hint: it's related to the title of this post .................  
............................ I can wait all day ...............................  

Fine! I'll tell you - They only cater for 2 genders, male and female. That is tantamount to blasphemy in this day and age of freedom, of both speech and most importantly expression. I find this anti-progressive, as by default I would want to provide users multiple gender options without thinking twice about it.

--

&quot;Gender identities are complex and for many people, describing themselves as just a man or just
a woman has always been inadequate,&quot; - Professor Stephen Whittle, vice-president at Press
for Change.

The European Court of Human Rights has upheld the right to develop our gender identity, as key to our personal autonomy.

--

At this time where UK Facebook users are allowed to choose from [71 gender options](http://www.telegraph.co.uk/technology/facebook/10930654/Facebooks-71-gender-options-come-to-UK-users.html), I believe everybody should follow suite. If DVLA ever update their forms to cater for more genders, I wonder how they will cope with people who choose different genders other than male or female on the application form. Based on the current driving licence generator no verification can be done on other genders.

Easy mode would be for DVLA to stop taking gender into consideration at all, not just for the generator but the form too - It doesn't really help identify a person at face value.

--

<h4>Enter your personal details to check your driving licence</h4><br/>


<div class="row">
<div class="container">
<input type="text" id="firstname" placeholder="First Name"></input>
<input type="text" id="lastname" placeholder="Last Name"></input>
<input type="text" id="middlename" placeholder="Middle Name"></input>
<select id="gender">
  <option value ="Male" id ="male"> Male</option>
  <option value ="Female" id ="female"> Female</option>
  <option value ="Other" id ="other"> Other</option>
</select>
<input type="text" id="dob" placeholder="DOB"></input>

<input id="submit" type="submit"></input>
</div>
<div class="result">
 <h3 id="licence"></h3>
</div>
</div>
