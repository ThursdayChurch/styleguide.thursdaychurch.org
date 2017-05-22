# Rock Docs

## Email

### Email Overview

![Communication Overview](http://storage.rockrms.com/documentation/Books/8/1.6.0/images/new-communication.png)

1. Email is the default communication medium, but this can be updated from the communication selector at the top of the page.
2. The recipient list will be filled with all of the people you previously selected as recipients. You can also add and/or remove names from the list at this point. Don’t forget that if you started with a blank communication you'll need to enter all of the names manually. You may notice that some names are in red. These names either do not have an email address or have been marked as not wanting emails or bulk emails.
3. Determine if this message should be treated as a bulk email. Bulk emails will have the unsubscribe link added to them. They will also not be sent to people who have asked that they not receive bulk emails from your organization.
4. If you would like to use a previously created email template you can select it here. For more information on creating templates see the Email Templates chapter below. This page can be set with a default template. Out-of-the-box this will show your organization’s header and footer with the sender's signature.
5. Fill in the email address that you would like the email to be sent from. By default, your contact information will be input, but you can change this as needed.
6. You might want replies to go to a different address than the one you're sending from. For example, when you send emails from the organization's leader, you may want the replies to go to an administrative assistant.
7. You can add any number of attachments you want to the email. Why limit a good thing?
8. Next, enter the subject of your email. A well-written subject can greatly increase the response rate of the email. Here are a few tips: provide context for the content of the message and a hint about the organization sending it. Remember to focus on catching the eye of the reader. You can use lava merge fields in your subject line so by all means, be creative.
9. Now the fun part - your message. While you can enter any generic message in this box, consider personalizing your message using merge fields. The message editor has a button `{}` for selecting a merge field to add. Personalization is one of Rock's main strengths so be sure to use it to its fullest.
10. For those with text-based mail clients (sigh), you'll want to provide a simple text version of your message. If you don't, they will see a link to a page that displays the HTML version of the message.
11. If you'd like you can delay the sending of your message to a date and time in the future. What a timesaver!
12. Before sending the email it's wise to send a test. Using the Test button will send the contents of the email to the currently logged in user. The first recipient will be used to process any merge fields in the email.
13. Finally, you can send the communication or save it as a draft to be completed later. This draft will be available to complete from `Tools > Communication History`. Take the time to get it right!

### Email Deliverability in Rock

Rock allows people to unsubscribe to **all** email communications from NorthPointe. As a organization we want to respect the ability of someone to remove themselves from our email communication; because it’s the right thing to do, and we are required to obey federal law. For every violation where someone has opted out, [the CAN-SPAM Act](https://www.ftc.gov/tips-advice/business-center/guidance/can-spam-act-compliance-guide-business) enforces penalties of up to $16,000 per violation.

As such, if your communication is “Bulk”, and not specifically related to event based communication. The **Bulk Email** checkbox must be selected to keep compliance with CAN-SPAM. When selected, you’ll notice many people selected in your email list will have red addresses that show “No Mass Email” when you hover over their names. These people will not receive your bulk email.

#### Email Not Active

If someone’s email server refuses to accept our email, Rock will automatically switch their email to an inactive status. In most cases this is because we have an incorrect address, or their spam filter has flagged our messages as spam.

If you have confirmed that their email is correct, ask them to check their spam folder and mark any NorthPointe messages as “Not Spam”. And switch their email status in Rock to active.

**Current Problem Sites**

- FPU.edu
- yahoo.com
- sbcglobal.net

## Event Registration

Rock's event registration features provide a simple tool to not only know who is planning to attend, but also to take care of many of the mundane tasks like event payments. The first thing that people want to know about event registration is the feature list.

### Event Registration Basics

#### People in Events

When someone registers, a person record is automatically created with all the information they provide on the registration form. A Rock administrator will automatically merge duplicate records to select the most up to date information. If they are logged in, their details will be automatically updated.

A timeline note will be automatically created for the registrar and the registrant in an event, allowing you to see at a glance who signed up for an event.

#### Registrar vs. Registrant

There are two parties involved with every registration that occurs. The registrar, the person who is actually entering the registration, and the registrant, the person who is registered for the event. In some cases this could be the same person. For instance, Ted Decker may register himself for an upcoming event. Many times though this will not be the case. Ted Decker might register his two children for camp. In this latter case, Ted would be the registrar while his two children, Noah and Alexis, would be registrants. While we're often most interested in the registrants for an event, we also need to be able to store and report on the registrars.

#### Automatic Replies

Rock automatically generates a response email with a payment receipt that shows any balance as well as a payment link.

##### Additional Confirmation Details

Additional Confirmation Details are included with the event registration confirmation email. To add additional details, submit it as part of your event request, or edit your Registration Instance and look for the **Additional Confirmation Details** text box.

##### Additional Reminder Details

Text sent with the optional event reminder email. This email is triggered by setting a **Send Reminder Date** on the event registration instance.

#### Notifications and Registration Contacts

One registration contact (Staff Member or Church Member) can automatically receive notifications when someone registers for an event. If notifications need to go to multiple people, send in a Rock request.

### Payments

#### Costs and Fees

##### Fees

#### Cash Payments

To process a cash payment… DEVELOPING

#### Credit Card

Rock currently accepts credit card payments through the front end of the website (my.northpointe.org). The form for backend payments will be fixed in V6.3 (ETA April 2017).

### Event Groups

Groups also play a role in event registration. In many cases the end point of the event registration process is the placement of the registrants into a group that you configure. While you're not required to have your event registrations add people to groups, in most cases you'll want to enable things like event check-in.

You can also do other clever things with the relationship between registrations and groups. Since nothing is keeping you from having more than one registration linked to a single group, you can handle complex registration scenarios. Say that your summer camp can only take so many boys vs. girls. In Rock you could setup two different registrations with separate caps for boys and girls. Both of these registrations can also put their registrants into the same group, giving you a single list of all children attending camp.


## People

### Merge Requests

You can create a merge request from any list of people within Rock. Most commonly you’ll use the search box to find records that need to be merged. Use the checkboxes to select the people to be merged, and the group of three people icon in the bottom of the list to merge.

**Search Examples**

- Search by name i.e. `gar joh` to merge records `Garrett Johnson` and `Garret Johnsen`
- Search by address `1600 Pennsylvania Ave` to merge duplicate children at an address


## Reporting in Rock

### Our Reporting Strategy

We’ve worked to create as many data views as possible to account for many different possible criteria that ministry leaders may need.

Ministry related Data Views are found under `Ministries`. Depending on your view rights you may see many other views.

**Ministries Data Views**

- Campus Safety - Security team, authorization, and related views. (Clearance may be required)
- College - College Ministry specific data views.
- Global - All church reusable views. Includes Baptism, Address Location, Core Classes, eRA, 1st Time Guests, Marriage, Membership, and gender specific targeting.
- Home Groups - Views used for
- NorthPointe Staff - Building blocks for staff related queries.
- NP Kids - Building Blocks for children, their parents, and NP Kids Volunteers.
- Wherehouse - Building Blocks for students, their parents, and Wherehouse volunteers.

### What Makes Up a Report?

There are two facets to any report: filter and display criteria. Consider this example. Your organization's leader walks in your door and asks for a list of attendees over the age of 18 who began attending within the last two years. He would like to have their names, contact information and the number of times they have attended. Using this example, let's look at each of the facets of reporting.

1. Filter Criteria: These are the criteria that limit the results to display. They answer the "Who" part of the request. In the case of the example, the criteria would be:
	2. Attendees
	3. Greater than 18 years of age
	4. Began attending in the last two years
5. Display Criteria: Once the results are filtered you must display them, with the necessary attributes, to the user. In the case of our example, these attributes might be:
	6. Name
	7. Phone
	8. Email
	9. Address
	10. Number of Times Attended

Once you create your handy report for your leader, it's very likely she'll be back asking for further changes. Perhaps now she wants another report with the same logic but only showing females. In most systems you'll have to start over and make a copy with the addition of the new criteria. Now you have two very similar reports to maintain.

With Rock, we have deliberately chosen to split the filter and display activities in reporting. You create your filters by defining **Data Views**. You then create your display by creating **Reports** that use the **Data Views**.

### Data Views



### Reports
