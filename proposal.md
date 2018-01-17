PRODUCT OVERVIEW

The Spotify Music Visualizer is a webapp that users will be able to use their spotify account to see what kind of music they like based on the music inside of their library. This will be presented as charts, graphs,etc.

SPECIFIC FUNCTIONALITY

The home page will have a link for a user to log in to their account. This will redirect them to spotify where they will need to login/approve my app to see their saved tracks. Then they will be directed back to my site where I will visualize it. There may also be a user profile page for them to see their specific user info. for MVP there will be at most 3 pages.

My app will take in the user specific tracks. Save them to a database and then make a second request to find the artist for the tracks (the genre is tied to the artist). I will be then be able see how many times an artist shows up in a users library thus telling me how many times a specific genre shows up. Eventually I will be able to use my library to search for information instead of making a call to Spotify's API for the information.

I will store the users tracks but I will also store values of their genres so I can visualize the values something like this:

Username
    rock - 76
    classical - 80
    eletronic - 90
    country - 22
    hip-hop - 55

Sub genres will be color coded to match their umbrella genre. Example Alt-rock, garage rock and punk rock will be visualized individually but will share the same color.


DATA MODEL

What are the persistent “nouns” you need to save across pages in your project MVP?
What do they represent?

We’ll be using a relational database which models things like a spreadsheet.
There are fixed fields and every instance

How do you need to search for specific instances of nouns?

TECHNICAL COMPONENTS

Spotipy which is a library for Python will be used to make queries and retrieve data used for visualization.
D3.js is a javascript data visualization tool that will be used to show the users their music taste based on the information gathered using Spotipy.

SCHEDULE

Data collection - 1.5 week
 • I want to make sure I can collect the data from Spotify and store them in a database
Data Visualization - 1.5 week
 • Learn how to visualize the data from the database in D3.
 • Decide how the data will look and if animations/interactiviy will be possible
UI/UX - 1.5 week
 • Design the frontend (css/js interactivity)
 • Only 3 pages planned out so I think I may look into frontend framekwork like Vue.js to handle SPA functionality


FURTHER WORK

The ability for users to compare their taste with friends or other users. Look at trends based on location within the US. More details like age and gender would be fun to compare as well. 