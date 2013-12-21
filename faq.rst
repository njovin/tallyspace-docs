Frequently Asked Questions
===========================

How does the SMS voting work?
---------------------------------------------------------------------------------------------
It's simple: you pick a 10-digit phone number to receive SMS votes at.  You set up a ballot with categories and then choices for each category.  You assign each choice an *SMS Option* which can be a number or word.  Voters send a text message to your SMS phone number with their choice, and it's counted immediately.  This is explained in more detail 

How do voters vote online? Do they need a special link? Do they need to register?
---------------------------------------------------------------------------------------------
When you sign up for an account, you're automatically assigned a custom link for your voter's to log in at.  This can be viewed and changed from the :ref:`custom-voting-address` page. 

.. note:: If your voters end up on tallyspace.com without using your custom link, they can still log in to vote.  They'll be prompted to find your organization (by name), once they'll selected it, they can log in

From your organization's voting page, voters will see a list of all open ballots.  They can click on any of them and they'll be taken to a login page where they log in with the information you selected when you :ref:`set up the ballot<online-vote-security>`.

The beauty of TallySpace is that voter's don't have to sign up or create their own account - they log in with information they already know, using information you :ref:`import for them<importing-contacts>`. 


Why is TallySpace so much less expensive than some other SMS voting providers?
---------------------------------------------------------------------------------------------
Many other SMS providers use shortcodes (4 and 5 digit phone numbers).  These are very expensive and you usually have to share the code with all of that provider's accounts.

TallySpace allows voting using standard 10-digit phone numbers.  Because these are less expensive, we can assign a dedicated number to each account.

Why is TallySpace more expensive than services like Google Forms, SurveyMonkey, or Wedgies?
---------------------------------------------------------------------------------------------
Those services are great for setting up quick surveys where security isn't critical.  For election-type surveys where you need to be certain that voters aren't gaming the system, TallySpace is the right tool for the job.

How do I make sure each voter only votes once, or how do I let them vote more than once?
---------------------------------------------------------------------------------------------
When voting online, voters only get one vote, by default.  You can allow voters more than one vote in the :ref:`Category Settings <category-basic-settings>`.

For SMS voting with the *Require ID* option set, the same rule applies.  Voters' identity is verified by their ID number - they will be able to vote either online or via SMS, but not both.  

For SMS votes with the *Limit Votes by phone number* option selected, the number of votes can still be set on :ref:`Category Settings <category-basic-settings>`, but no contact information is cross-checked.  The system allows X votes per phone number.

How do I replace my contact list with all new contacts? 
---------------------------------------------------------------------------------------------
When importing your contact list, there is an option to delete all existing contacts and replace them with the new ones.  See :ref:`importing-contacts` for details.

I want somebody else in my school/organization to be able to use the service, can I do that?
---------------------------------------------------------------------------------------------
Absolutely!  You can manage additional users from the :ref:`User Management <user-management>` section of your account.  You can even set it so that they only have access ot view and manage the ballots that they set up, and no one else's. 

It doesn't look like my SMS votes are being counted, what do I do?
---------------------------------------------------------------------------------------------
There are a few things that you should check if SMS votes aren't being counted as expected:

#. Check the :ref:`sms-security` options for the ballot. If you're requiring an ID number, make sure that the voters are including the ID number before their choice.  You can view the incoming messages from the :ref:`SMS Activity <sms-activity>` page
#. Make sure your Ballot is accepting votes, by checking the :ref:`ballot-overview`.
#. Make sure voters are sending their messages ot the correct phone number, which you can check on your :ref:`sms-setup` page.