# SOC--Project-BloggerHead
A MERN Stack web development project under Wncc, IIT Bombay

 
Week 1 : started with learning HTML, CSS, Javascript, Bootstrap.
Week 2-3: started with MERN
Week 4 : Getting familiarised with all the contents till week 3 we kickstarted the project.
Week 5: user APIs, blogs APIs, sign in authentication, password hashing completed
Week 6 : frontend part for signup and login pages,
Week 7 onwards : read, create, search, edit and delete blogs made possible and all others described below are implemented.
 

Short description of all the files:
In the server folder -
Models-
	blogModel.js- connects blogs to mongodb database
	userModel.js-connect user database to mongo db
Routes-
	blogs.js- contains  rest api 
users.js- contains crud api
Utils-
	auth.js- Uuid set up file
Index.js- server file 

In the Client folder-
Inside src folder-
Components-
Navbar-
navbarelements.js- code to render navbar where all the buttons for signup, login and logout are present. It also has a search bar and user’s name displayed only when the user is logged in.
about.js- This file exports a function which shows the information about this project and us.

CompleteBlogs.js- exports a react component which renders a page where any specific blog is displayed completely  with its title, author name and last updated time if its no of characters exceed 300.
Blogs.js- exports a react component which renders a page where all the blogs (only ten blogs if there are more than ten blogs and a see more option to see next ten blogs) are shown as cards with few lines of description and a read more option which redirects to a page showing the blog completely.
createblog.js- a page with a form taking title, description and author name as inputs and a submit button clicking on which a blog can be created provided all the necessary data is present.  
home.js-  the home page which features a carousel to add to the beauty;), and if the user is logged in, two blogs as cards and a button for the see more such blogs option.
myprofile.js- registered users can see their profile data like their name, username, email Id and also the blogs they created in the same format as discussed above.
searchblog.js- when any word is typed in the search bar present in the navbar the user is redirected to a page where all the relevant blogs (with a matching word in title and author name) are displayed. 

pages-
delblog.js-  when clicked on delete button for the blogs, redirected to a page where users are asked for the password for authentication before deleting the blog. There are also cancel and confirm buttons with functions matching their name.
deluser.js- when clicked on delete button for the users profile, they are redirected to a page where users are asked for the password for authentication before deleting their account. There are also cancel and confirm buttons with functions matching their name. After successful deletion, they are redirected to the home page and logged out.
editblog.js- when clicked on the edit button of the blog in myprofile page,they are redirected to a page very much similar to the createblog page, where they can edit their blogs.  
edituser.js- when clicked on the edit button of the profile in myprofile page,they are redirected to a page very much similar to the signup page, where they can edit their account data like username, email Id (provided they are unique), firstname, lastname and password as well. 
login.js- login page where registered users can fill details and login. 
signup.js- registration page where users can fill all the required details and register themselves.
App.js- all the react components mentioned above are imported here and rendered using routes.
index.js- The app component wrapped in Router is rendered here.
