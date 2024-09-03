%%%%%%%%%%%%%%%%%%%%%%%---WEB Developing---%%%%%%%%%%%%%%%%%%%%%%%%%%%

First start with skeleton structure of the design specification to need
----------------------------------------------------------------------
                             MOVIE SEARCH
----------------------------------------------------------------------
FILE STRUCTURE 

     index.html
     
     style.css
     
     app.js
-----------------------------------------------------------------------
-----------------------------------------------------------------------
                                index.html
-----------------------------------------------------------------------
TO START WITH SEE THE EXTENSION OF HAVEING THE HTML FILE:

! The boiler plate is having structure of been analysis which version have been used here

! The html tag is the main tag in the file with inside consists of the head tag and body tag.

! The head tag is consists of link and title of contant using title tag ,in our case it is Movie Search tilte.

! The body tag is consist of header tag , main tag and link to link the app.js using script tag.

! In inside the the header tag there will the form tag with id of form and having input tag of 
attribute of type of containt used to indicate with text, to have autocomplet off state, 
id of the a name in search , placeholder of name of Search and last of having the class name of search

! The main tag is having the id name of main to used to style and used in condition in javascript.

! The scrpit tag is used src attribute to link with app.js file.

-------------------------------------------------------------------------
                                  style.css
-------------------------------------------------------------------------
TO START WITH DESIGN AND STYLE A WEBPAGE

! At first is setting all value to box-sizing of border-box and import the necessary fonts from google fonts

! Body tag is having a style of  margin of 0, background-color of #afe33e and font-family of "Poppins", sans-serif.

! Header tag is having a style of background-color of #24d1a0 with padding of 1 rem,display of flex and justify-content of flex-end.

! The search class is having a style of padding: 0.5rem 1rem with border-radius: 40px , border: 2px solid #0d0f30 ,background-color: transparent ,font-family: inherit ,color: #eee,
font-size: 1rem to them.

  # placeholder is add to search with color of #f1f2f5 and having a focus of outline of none and background-color of #05082c to them.
  
    
! The main tag is have display setting of flex and flex-wrap of wrap to them.

! The movie class is form the app.js to api call elemet to display the contain in them , which has the box-shadow of 0 4px 5px rgba(0,0,0,0.2) with border-radius of 5px, width of 300px to required size,with have the background-color of #111a79,margine of 1rem, overflow can be hidden to respected to the positon of the relative contant.

  # movie class is also having the image by img tag with source reference by api calls of having the width of 100% to them.
        
! The movie-info class is consists in javascript file , to properties of display of flex,jusitfy-content of space-between, padding of 0.5rem 1rem 1rem, color of #eee with letter-spacing of 0.5px with align-items to center to have clear ui.

 # The h3 tag in movie-info class can have the margin of 0 and span of properties of backgorund-color of #22254b with padding of 0.25rem  for left and right and 0.5rem for up and bottom aliment of having the border-radius of 3px and font-weight of bold, and have span of green,orange and red of color value to the elements of content.

! The overview class for div elements of the javascript having properties of position of absolute and aliment of top right left bottom of 0 with background-color of #fff,padding of 2 rem of the transform of translateY(100%) to which having the transition of transform of 1seconds with easein of max-width of 100%.
 # The hover effect is added to movie and overview class with the transform of translateY(0) and h4 tag of overview class of margin-top of 0.
--------------------------------------------------------------------------------------------
                                                   app.js
--------------------------------------------------------------------------------------------
TO CREATE THE FUNCTIONALY TO THE WEBPAGE

! At start which is declaration of API calls with suitable variable name to access to specific variable name for specific api call.

! Declaration of the id name with variable of main,form,search of the give content and getMovies is the function of have paramenter value of APIURL to show the main content while loading.

! While the request is send to them there will be the waiting time , so used async function to the getMovies() with url of them to fetch adn responeDate with actual value.

! console.log is used to see the getting content and having the showMovies() of paramenter value of respDate.results inside the async function of getMovies().

! Then creating the showMovies() function with the parameter input of variable name of movies ,
 inside them there will be main element with innerHTML properties and movies is consists of forEarch loop to show the relevant content to them of list with movieEl with classList of add function with movie arugument with consists of img tag and div element of having a class name of movie-info and overview with getClassByRate() to see the average review from the people,with h2 tage to display the movie title. with main with appendChild()function of arugements of movieEl inside the showMovies().
 
! The creating the getClassByRate() function with the parameter of vote of having the condition of voting range in greater or equal to 8 are to  indicate with green color and if the vote is greater or equal to f are indicate by orannge and if not statified the both condition then there will be red color indication.

! Then adding the addEventListener to check the error in the form by analysis with the creating the const variable of name searchTerm of have the value of search with value attribute and condition is having for the searchTerm of getMovies() function is having the arguments of SEARCHAPI with searchTerm in them the search value to them.


----------------------------------------------------------------------------------------
# THIS IS THE SIMPLE PROJECT IN MOVIE SEARCHING APP.
---------------------------------------------------------------------------------------


