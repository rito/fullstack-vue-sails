# fullstack-vue-sails
Architecture in Node with VUE 2 and SAILS Realtime.

2 architectures:

---------------------

API Realtime:

---------------------

- Independent backend using SailsJS. Realtime API with connection to MongoDB, mySQL, SQLite, PostgreSQL and Redis. CRUD with each of the related bases. In addition to a CRUD with GraphQL, accessing each of the bases.

Authentication via local registration / email, facebook, google +, gmail, twiter, github. Each registered user can register 1 profile and associate all the methods above to the same profile.

User must have an associated profile and the API must have session control.

API should have a CRUD with external REST API.

---------------------

Client VUE:

---------------------

- Independent frontend using VueJS and Bootstrap. Vue connecting via Socket Realtime with the Sails API. Registration Screen via methods quoted in the backend (API Sails), Login Screen, Profile Change Screen, Forgot Password Screen, and CRUD Maintenance Screen.

The Client (VueJS) and the Backend (Sails) must be independent. Updates should be realtime. Once an information is loaded on the screen and the same information is updated in the database, the information must be updated in realtime without refresh and without being requested.

The frontend should also have a simple REST API connection too, with no need for realtime.

Check Architecture drawing:

![Architecture in NodeJS](http://webland.pt/arquitetura/Arquitetura.png)
