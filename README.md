# Owls Casing Scheduler

## What are the main features of the portal?
* Profile Management (Privilege: Anyone)
  * Enter your Name, Email, Mobile Number
  * Enter your preferences for receiving email notifications. **You have to opt in!**    
* Session Creation (Privilege: Anyone)
  * Create a session
  * Specify the start and end time, venue etc.
  * (Optionally) add people to the session
  * Add at least one case to the session. Cases can be filtered by name and category while adding them.
* Session Updation (Privilege: Session owner)
  * Modify an existing session
  * Add/Remove cases
  * Add/Remove participants (except the session owner)
* Session Search (Privilege: Anyone)
  * Search by Session ID, Session Participants, Range for Start Time, Case Categories, Cases
* Session Actions (From the search results)
  * View the session details (the session title is hyperlinked)
  * Sign up for an existing session (from the search results)
  * Opt out of an existing session that you are part of (from the search results)
  * Edit the session (if you are the session owner)
  * Delete the session (if you are the session owner)
* View a list of cases available
* View a list of users (and their contact details)

## When will I receive an email notification?
* In order to receive an email notification, you have to choose the corresponding options on your profile page
* You might want to add `owl.casing.2017@gmail.com` to your contact list.
* You will receive a notification in the following scenarios:
  * You get added to a session
  * You get removed from a session
  * A session you are part of gets updated by the session owner
  * A session you are part of gets deleted by the session owner
  * A new participant signs up for a session that you are part of
  * An existing participant opts out of a session that you are part of

## When will I not receive an email notification?
* If you have unchecked all the notification preference checkboxes on your profile page
* If you have selected *Yes* for the *Block notifications* field
* Even with notifications on, you won't receive notifications for your own actions, such as:
  * You create a session
  * You update a session
  * You delete a session
  * You sign up for a session
  * You opt out of a session

## Bugs? :bug:
A wise T-shirt once said
> If at first you don't succeed, call it version 1.0

* The portal hasn't gone through rigorous testing, so there still are a few bugs in there.
* Form inputs aren't completely validated.

## New features
* If there are simple changes which have consensus, I'll be happy to make them.
* It's very unlikely that I will add new features. The portal was meant to serve as a `stop-gap solution`.
* I don't know whether there's going to be a v2.0 or who's going to build it.

## What's the technology stack?
The portal is hosted on free infra, and hence isn't built for high performance. The notifications are sent through a new Gmail account. If for whatever reason, Gmail blocks the account, this feature will require a more standardized service email account.
* MySQL database on `GearHost`
* Flask web app on `Heroku`
* UI scaffolding with `Bootstrap`
* The usual stuff: `HTML`, `JS`, `jQuery`, `CSS`
