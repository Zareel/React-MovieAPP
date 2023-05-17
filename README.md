# Learning React.js
## I learned to create this beautiful movie app from JavaScript Matery

# What is API

Application programming interface is a software that allows two applications to interact with each other without any user intervention. It is a code that helps two different software to communicate and exchange data with each other

# 2. omdbapi

obdbapi.com will give you access to data about these data

# 3. omdb API KEY



# 4. How we can call this api to get data

create a static variable and
const API_URL = "https://omdbapi.com?apikey=KEY"
Now we can use that from inside of our component to gather data. more specifically we want to fetch date from this api as soon as our component loads.
for this we can use useEffect hook

# 5. useEffect hook

useEffect hook accepts a callback and an empty dependancy array as the second one only if we want to call it at the start

# 6. NEXT STEP

Create new function searchMovies = an async function
async stands for asynchronous data which means that it takes some time to fetch these movies

- the searchMovies is going to accept a search title
- there we can say const response is equal to await fetch and then we can use a template string, you can do that by using a backtick
- there we can dinamically use our API_URL and then say &s= and one more time here we want to specify the title dinamically so this is going to call our api now.
- once we get the response we have to get the data from it by saying const data is equal to await response.json()
- now inside of this data object we should have the data about the movies
- call search movies inside useEffect
- provide it a title which is going to be a srting of yor favourite movie
- console.log(data.search) and check

# . What is components in React?

Components splits the UI into reusable independent parts and we combine these components to build cool applications

# 2. What to learn?

- Managing states
- Components
- Props

# 3. next steps

- generate APIkey
- assign url value to the variane API_URL ie const API_URL = "http://www.omdbapi.com?apikey=c76fc7b0 ";

# 4. imprt useEffect hook and call it

uereffect accepts a callback function and an empty dependancy array as the second one

# 5. What is API

Application Programing Interface is a software that allows two applications to interact with each other without any user intervention. It is a code that helps two different softwares to communicate and exchange data with each other.

# 6. What is json?

JavaScript Object Notation is a lightweight format that is used for data interchanging. It is a language indpendent data format. It supports almost everykind of language framework and library

# 7. Fetch movies and check if API is working

- At the top if useEffect hook call a function 'searchMovies' that going to fetch movies
- seachMovies equal to async arrow function
- async stands for asynchronous data which means that it takes some time to fetch these movies and
- the searhMovies is going to accepet a search title that we want to search by like superman or any other title
- there we can say const response is equal to await fetch and in there we can use a template string, you can do that
  by using backticks so we can dinamically specify the api url
- so API_URL then say & s is equal to and one more time we want to specify the title
- like (${API_URL}&s=${title})
- so this is going to call our API
  -now once we get the response we have to get the data from it by saying const data is equal to awaint response.json
- now inside of this data object we should have the data about the movies so lets simply console.log it
  -console.log(data.search)
- call the function search movie inside useEffect and provide it a title which is going to be a string of your favorite movie and search
- inspect the brouser check if you get spidrman movies
- if so api is full working
