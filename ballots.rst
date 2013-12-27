Ballots
========
Ballots are the containers for categories and choices.  Before you can conduct any vote or survey, you need ot create a ballot.


Creating a Ballot
-------------------
On the *Ballots* page click the green *Create Ballot* button to get started.  This will open the 'Ballot Setup Wizard' which will guide you through the process of setting up a ballot, including Category setup and security options.

.. image:: /images/ballot_setup_wizard.jpg
    :width: 600px

.. _ballot-overview:

Ballot Overview Page
----------------------
Once you've set up a ballot, you'll be taken to the *Ballot Overview* page.  This gives you a quick view of the status of your ballot (accepting votes, scheduled, etc.), categories, and voting options (SMS, online, etc.).  

.. image:: /images/ballot_overview.jpg
    :width: 600px

Basic Settings 
----------------
* **Ballot Title:** This is what displays in the list of available ballots before a voter logs in
* **Online Voting:** Check this box to allow voters to vote online
* **SMS Voting:** Check this box to allow voters to vote via SMS (text-message)
* **Result Viewing:** Check this box to allow logged-in voters to view the results in real-time

.. note:: If you don't see the SMS voting option, you need to choose an SMS voting phone number from the :ref:`sms-setup` page

Security Settings
------------------
TallySpace allows you to control exactly how voters are authenticates whether they're voting on line or via SMS.


.. _online-vote-security:

Online Vote Security 
^^^^^^^^^^^^^^^^^^^^^^
Check the box for each field that you want to require voters to fill in prior to being allowed to vote.  Whenever a voter wants to vote online, they'll need to enter the information for each of these fields *as it appears in your contact list* before they can vote 

.. image:: /images/online_security.jpg

.. note:: TallySpace does not offer a voter self-registration process.  Only voters you've imported or entered manually will be able to log in.  Make sure you've imported or entered all of the information you're requiring or else nobody will be able to vote.

.. _sms-security:

SMS Security
^^^^^^^^^^^^^
You have three ways to restrict who votes via text-message:

* **Require users to enter their ID number:** If you choose this option, voters need to begin their text message with their ID number (as shown in the contact list).  For instance, if a voter with ID 87989 wants to vote for a choice with SMS Option 3, they would send:
::

    87989 3

.. note:: TallySpace allows you to run 'mixed-mode' online & SMS votes.  If you set up a ballot to allow online & SMS votes, be sure to select this option - this will prevent users from voting online and via text.  Since they are authenticated by their ID number no matter how they vote, this allows us to ensure they only vote once.  

* **Allow X votes per phone number:** This will allow anyone to vote (*not* just contacts in your contacts list), but only allow X votes per category. You set what X is in the :ref:`Category Settings <category-basic-settings>`.
* **Only allow votes from known contact phone numbers:** If this is selected, only votes from phone numbers associated with contacts in your Contacts list will be counted.  


.. _ballots-advanced-settings:

Advanced Settings
-------------------
The *Advanced* tab provides additional controls over the way your ballot behaves

Scheduled Opening/Closing of Polls
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
If you'd like a ballot to start & end accepting votes at a specific date & time, you can set that here.

.. image:: /images/ballot_schedule.jpg

Publicly Viewable Results
^^^^^^^^^^^^^^^^^^^^^^^^^^
Clicking the *Generate URL* button will generate a unique web address.  Anybody with this address will be able to view the results of your vote without logging in. 

Hide Votes/Voters
^^^^^^^^^^^^^^^^^^
By default, all information about every vote cast is available to the account administrator. This includes who voted for whom, when, and some additional technical info.

In some rare cases, due to privacy requirements, you may wish to hide the voter or their specific choice from the vote logs. 

.. note:: If these options are selected you will not have access to specific voting results, only totals.  TallySpace does keep a record of this information for technical and auditing needs, but it will not be released to the account administrator without a legal order if these options were selected while the votes were cast. 

Respond to Failed SMS
^^^^^^^^^^^^^^^^^^^^^^^^^
By default, if a user's SMS message can't be authorized or matched to a valid SMS Option, the system will respond to them with an error message. If you'd like to disable this behavior, uncheck this box. 

Respond to Succesful Vote
^^^^^^^^^^^^^^^^^^^^^^^^^
By default, no message is sent back to users when a vote is submitted succesfully.  If you'd like to change this, check this box and fill in the message you'd like sent back to voters.


Respond to Failed SMS
^^^^^^^^^^^^^^^^^^^^^^^^^
By default, if a user's SMS vote is succesful, the system does not send any response.  If you'd like to send a response when a vote is counted succesfully, check this box and type in the message you'd like sent back to voters.

.. warning:: Response messages to voters count against your account's SMS messgae allotment.  This means if you're on a plan that allows 5,000 message, you'll only be able to accept 2,500 votes (2,500 incoming votes + 2,500 confirmation responses sent back to voters).


Archiving & Deleting Ballots
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
You can *archive* a ballot by clicking the archive button.  All this does is move the ballot from the *Current Ballots* tab to the *Archived Ballots* tab.  It does not delete results.

Clicking the *Delete this Ballot* button will permanently delete a ballot and all results.

Resetting Results
^^^^^^^^^^^^^^^^^^
The *Reset Results* button allows you to permanently delete all votes for a ballot.

Viewing Results
-----------------
The *Results* tab will take you to the Results page for a ballot - showing the totals for all choices in each category.

Exporting Results
^^^^^^^^^^^^^^^^^^
The green 'Export Results' button at the top of the *Results* page allows you to export detailed results as an Excel CSV file:

.. image:: /images/export_results.jpg

* **All Totals** exports a list of all categories and totals for each choice
* **Eligible voters that have voted** exports a list of just voter names who have voted
* **Eligible voters that haven't voted** exports a list of eligible voters who haven't yet submitted any votes
* **Audit Report** is the most detailed report - it shows exactly who voted for who, when, and from which IP address. 

Live Updating
^^^^^^^^^^^^^^ 
Whether somebody votes online or by text message, the results are counted immediately. It's usually less than five seconds from the time a message is sent to the time our system received, parses, and saves a vote.

However, by default, you need to refresh the results page to get the most up-to-date data.  If you're at a live event or monitoring the results and would like the results to update in real-time without having to manually refresh the page, simply click the *Enable Live Updating* button on the results page. 


