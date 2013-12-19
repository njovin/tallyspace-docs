Ballots
========
Ballots are the containers for categories and choices.  Before you can conduct any vote or survey, you need ot create a ballot.

Creating a Ballot
-------------------
On the 'Ballots' page click the green 'Create Ballot' button to get started.  This will open the 'Ballot Setup Wizard' which will guide you through the process of setting up a ballot, including Category setup and security options.

.. image:: /images/ballot_setup_wizard.jpg
    :width: 600px

Ballot Overview Page
----------------------
Once you've setup a ballot, you'll be taken to the 'Ballot Overview' page.  This gives you a quick view of the status of your ballot (accepting votes, scheduled, etc.), categories, and voting options (SMS, online, etc.).  

.. image:: /images/ballot_overview.jpg
    :width: 600px

Basic Settings 
----------------
* Ballot Title: This is what displays in the list of available ballots before a voter logs in
* Online Voting: Check this box to allow voters to vote online
* SMS Voting: Check this box to allow voters to vote via SMS (text-message)

.. note:: If you don't see the SMS voting option, you need to choose an SMS voting phone number from the :ref:`sms-setup` page

* Result Viewing: Check this box to allow logged-in voters to view the results in real-time

Security Settings
------------------
TallySpace allows you to control exactly how voters are authenticates whether they're voting on line or via SMS.


Online Vote Security 
^^^^^^^^^^^^^^^^^^^^^^
Check the box for each field that you want to require voters to fill in prior to being allowed to vote.  Whenever a voter wants to vote online, they'll need to enter the information for each of these fields *as it appears in your contact list* before they can vote 

.. note:: TallySpace does not offer a voter self-registratio process.  Only voters you've imported or entered manually will be able to log in.  Make sure you've imported or entered all of the information you're requiring or else nobody will be able to vote.

SMS Security
^^^^^^^^^^^^^
You have three ways to restrict who votes via text-message:

* **Require users to enter their ID number:** If you choose this option, voters need to begin their text message with their ID number (as shown in the contact list).  For instance, if a voter with ID 87989 wants to vote for a choice with SMS Option 3, they would send:
::

    87989 3

.. note:: TallySpace allows you to run 'mixed-mode' online & SMS votes.  If you set up a ballot to allow online & SMS votes, be sure to select this option - this will prevent users from voting online and via text.  Since they are authenticated by their ID number no matter how they vote, this allows us to ensure they only vote once.  

* **Allow X votes per phone number:** This will allow anyone to vote (*not* just contacts in your contacts list), but only allow X votes per category. You set what X is in the :ref:`Category Settings <category-basic-settings>`.
* **Only allow votes from known contact phone numbers:** If this is selected, only votes from phone numbers associated with contacts in your Contacts list will be counted.  


Advanced Settings
-------------------
Scheduled Opening/Closing of Polls
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Publicly Viewable Results
^^^^^^^^^^^^^^^^^^^^^^^^^^

Hide Votes/Voters
^^^^^^^^^^^^^^^^^^

Responding to Failed SMS
^^^^^^^^^^^^^^^^^^^^^^^^^


Archiving & Deleting Ballots
-----------------------------

Viewing Archived Ballots 
^^^^^^^^^^^^^^^^^^^^^^^^^


Viewing Results
-----------------

Letting Voters View Results
^^^^^^^^^^^^^^^^^^^^^^^^^^^^


Resetting Results
-----------------

Resetting individual voters' votes 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


