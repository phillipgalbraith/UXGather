## Deployed Website 

https://front-end-neon-two.vercel.app/

# Front-end

## ☝️ **Pitch**

(at times tests are erroneously referred to potlucks to remind to rename data)

If you have ever tried to organize anonymous usability tests with multiple facilitators and participants through expensive complex applications or a multiplatform work flow, you know why this app is essential. 

In the world of usability test organizers, the "UXGather" is king. This is your place for simple qualitative tests.

## ✅  **MVP**

1. As an `facilitator` I can create an upcoming usability test `potluck` and invite participant to attend

1. As an `facilitator` I can select enter an an upcoming `test` during creation

2. As an `facilitator` I can adjust `date`s, `time`s and `location`s  of the usability test // locations are links to Google Meet or Zoom etc.

3. As an `facilitator` I can use the list feature in my app to add Realistic Actionable Tasks (`items`) - ie "users create a new test" - that we'd like to see in the usability test

4. As a `facilitator` to a usability test I want to be able to confirm that I'm going to the upcoming `potluck` (rebrand usability test)

5. As a `facilitator` I'd like to be able to select which Tasks (`item`s) I'd like to be responsible for mediating.

**NOTE: All of the user stories above should only require a single user type. Users can create "usability tests" and add other users to them.**

## 🏃‍♀️ **Stretch**

1. Add a reminders functionality that allows users to link up their upcoming `date`s to their Google calendar.

2. Ability to upload multiple `photos` from the usability test gathering, like a photo gallery of annotated Screenshots from a past test.

3. As an `facilitator` I can use the list feature in my app to add up to 5 test Subject's email adresses `participantEmails`.

4. Create a unique code for each email to enter without logging in to confirm and cancel (boolean) test participant availablity 

6. The app has an endpoint that displays the going status when a code is entered and has a toggle switch with a submit button that goes to confirmation screen.

5. As an `facilitator` I can see each emails' `going` status. `participantEmails`.



### Link to class names for styling shared doc
https://docs.google.com/document/d/1nkA7Xo5Pbbkb2JkDORICQk7ChhfeQY1nQfXKTpJEIfo/edit?usp=sharing

### API Documentation

**[POST]** to `https://back-end-node-postgresql.herokuapp.com/api/auth/register`: lets a user register.
<!-- This endpoint needs to be fixed in the backend (GIVING A 500 ERROR when called through axios) -->

**[POST]** to `https://back-end-node-postgresql.herokuapp.com/api/logout`: returns the expired authentication information of the user.
<!-- This endpoint needs to be created in the backend -->

**[GET]** to `https://back-end-node-postgresql.herokuapp.com/api/users`: returns a current authentication information of a user. Pass in the following credentials as the `body` of the request: `{username: ``, password: ``}` for a successful login.

**[GET]** to `https://back-end-nodes-postgresql.herokuapp.com/api/events`: returns all the events currently available.
<!-- This endpoint needs to be created in the backend -->
*This endpoint can only be accessed by an authenticated user.*

**[POST]** to `https://back-end-nodes-postgresql.herokuapp.com/api/events`: creates an event object. Returns all available events. Pass the event as the `body` of the request.
<!-- This endpoint needs to be created in the backend --> 
*This endpoint can only be accessed by an authenticated user.*

**[PUT]** to `https://back-end-nodes-postgresql.herokuapp.com/api/events:id`: updates the events using the `id` passed as part of the URL. Returns all available events. Sends the updated event object as the `body` of the request.
<!-- This endpoint needs to be created in the backend (IF THERES STILL TIME!) -->
*This endpoint can only be accessed by an authenticated user.*

**[DELETE]** to `https://back-end-nodes-postgresql.herokuapp.com/api/events/:id`; removes the event with the `id` referenced. Returns all available events. 
<!-- This endpoint needs to be created in the backend (IF THERES STILL TIME!) -->
*This endpoint can only be accessed by an authenticated user.*


Dashboard:
  The features that allow guests to change their item and confirm they're going are tested by axios post requests to reqres. 
