

# PROJECT GOODCALL

### TEAM MEMBERS

1. Adanna
2. Marco
3. Danny
4. Matt

### PROJECT GOALS

1. Create an API using `Express.js` that possesses full CRUD functionalities.
- POST creates new routines and new users.
- GET retrieves exercises for a routine, and user-saved routines.
- PUT updates the names of existing routines the user saved.
- DELETE removes existing routines.
2. Create a `React.js` application that presents the API's data in a user-friendly way.

### APPROACH

Primarily, we want this app to be convenient for the user.

The ideal scenario for this app to be used is before and during a workout with either a beginner or veteran.

The app allows the user to build a complete routine on the fly, and possibly save that routine for later reference.

Keeping this in mind, we want to reduce the number of "screens" the user will need to use. This way, the user is focused on working out, and not on navigating the application.

The app features log-in functionality as a way to save routines; however, logging in is not mandatory if the user has no intention of saving their routine.

### WIREFRAMES

**Landing Page**
![LANDING PAGE](https://i.imgur.com/QS4QbyQ.jpg)
**Category Page**
![CATEGORY PAGE](https://i.imgur.com/F1KS9yn.jpg)
**Routine Page**
![ROUTINE PAGE](https://i.imgur.com/FxTldio.jpg)
**Exercise Page**
![EXERCISE PAGE](https://i.imgur.com/DRBQAlJ.jpg)
**User Page**
![USER PAGE](https://i.imgur.com/LIHVTVA.jpg)

**API**
![FETCH REQUESTS](https://i.imgur.com/elMA4AO.jpg)
**Component Map**
![COMPONENT MAP](https://i.imgur.com/8bjyTye.jpg)

### TECHNOLOGIES

- `React.js`: a front-end framework that enables the creation of single-page applications by the organization of code into "components."
- `Express.js`: a back-end framework that allows the construction of servers.
- `PostgreSQL`: a back-end framework that creates and manages a database.

### PACKAGE DEPENDENCIES

- `dotenv`
- `bcryptjs`
- `pg-promise`
- `morgan`
- `express`
- `express-session`
- `passport`
- `passport-local`
- `body-parser`
- `cookie-parser`

### ERDS

**Users**

|id|name|password_digest|email|
|:-:|:-:|:-:|:-:|
|Primary||hash||

**Exercises**

|id|name|bodytype|type|url|reps|sets|
|:-:|:-:|:-:|:-:|:-:|:-:|
|Primary|||||||

**Routines**

|id|name|bodypart|type|user|exercises1|exercises2|exercises3|exercises4|
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
|Primary||||Users(id)| Exercises(id) | Exercises(id) | Exercises(id) | Exercises(id) |

### USER STORIES

**Making an account**
1. The user opens the app and reaches the landing screen.
2. The user selects the register button on the header, which takes them to a registration screen.
3. The user fills in the form.
4. Upon submitting the form, they are redirected to their new profile.

**Logging in**
1. The user opens the app and reaches the landing screen.
2. The user selects the login button on the header, which takes them to the login screen.
3. The user fills in the form.
4. Upon submitting the form, they are redirected to their profile.
5. **NOTE:** If the user logged in before, the app retains their log in.
5. **NOTE:** If the user is logged in, the login and register buttons are replaced with user profile and logout buttons.

**Making a routine**
1. The user opens the app and reaches the landing screen.
2. The user selects the routine button, which takes them to the routine creation screen.
3. The user selects the route they wish to do for the day. The randomly-generated routine list appears.
4. The user performs the exercises on the list for the specified rep/set.
5. If the user wants to learn an exercise on their list, they can select that item to go to an exercise screen.
6. The exercise screen has a YouTube video that instruct them on the exercise, including directions & safety tips.

**Saving a routine**
1. The user opens the app and reaches the landing screen.
2. The user selects the routine button, which takes them to the routine creation screen.
3. The user selects the route they wish to do for the day. The randomly-generated routine list appears.
4. The user can save the list with a button at the bottom.

### STYLE GUIDE

_TBD_

### LINKS

[PROJECT BOARD](https://github.com/adanna21/workout-app/projects/1)
