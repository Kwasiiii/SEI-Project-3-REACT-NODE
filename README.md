# Project 3 - Pint-Pirate

## Team Members
 Kwasi, Wala, Dan

## Project Overview

For the third project of the SEI, the task was to make a full stack application. This was to be a desktop app that uses an Express API and must consume our API on a separate front-end.

## Languages/Technologies Used

- HTML5
- CSS3
- SASS
- Bootstrap
- JavaScript ES6+
- React
- Node
- Express
- MongoDB
- Axios
- Mapbox GL
- Yarn
- NPM
- Git
- GitHub
- Font Awesome
- Google Fonts
## Initial Approach to Brief

Promptly after deciding our theme for the full-stack app, we firstly drew wire-frames of what our intended finish product may look like. This helped us to understand how we might break-down different parts of the app into several React components.
Through the use of pseudo-code, we were able to map out the logic/functionality that would bring our design to life.
<img src="https://i.imgur.com/Wom0YXv.png" alt="pintpirate-page-home" width="400" /><img src="https://i.imgur.com/jnsCrpm.png" alt="pintpirate-page-citylist" width="400" /><img src="https://i.imgur.com/gFiPSMu.png" alt="pintpirate-page-card" width="400" />

## Process🍺

We decided to build an application that shows UK travel destinations via each cities cheapest pint of beer! Users can sort all cities (on our database) either high-low or low-high. For added user immersion users can also search directly for a city through a search bar.

Additional features include the ability for users to post reviews on each of the cities (only authors of the reviews may delete them), we also added a Map page, where users can discover different UK destinations on a fully interactive map. Users have access to a 'My Profile' page where they can view personal login details. On each selected city page users can also find locations on our to find a certain beer.

All research relating to prices/brand of beer was researched and collated by us.

## Featured piece of code

To kick-off the project, we wanted to build out most of our back-end. We first decided to tackle making the seeds for our database. This was a crucial step, as we needed to populate our API with default data in order to build/test the whole application. An example seed is shown below.
![enter image description here](https://i.imgur.com/KpV2Cwj.png)
Following on from this, we defined all the schemas we would need for the app; cities, users and reviews. In coding these, we used 'referenced ' and 'embedded' relationships in order to link data between the different schemas.
![enter image description here](https://i.imgur.com/WBYmAym.png)

For the User schema, we used the `transform()` method for 'password' as we didn't want this information to be returned on a potentially un-secure connection.
![enter image description here](https://i.imgur.com/UVysRVw.png)
Furthermore, using 'bcrypt' we designed a function that will 'hash' a users plain-text password, enhancing account security.
![enter image description here](https://i.imgur.com/W3fITUW.png)

Once all of our schemas had been defined, we next turned our attention to connecting to our MongoDB database and in turn, seeding our database with default user and city information. Through dropping the database and re-populating, we have the control to reset our data to default if a certain situation arises.
![enter image description here](https://i.imgur.com/O9h8xwf.png)
Next, we define functions to handle Axios requests on the back end. These were either `.get` , `.post` or `.delete` requests.

Below is an example of how we handled a user posting a review. We spread in the request JSON body whilst also supplying the API with the current users ID. This proved useful further along the project for displaying who had written each review.
![enter image description here](https://i.imgur.com/CTCnSEa.png)
## Styling
After completing the back-end quite quick as a group. we decided to divide among ourselves when it came to front-end. Using CSS, SASS and Bootstrap to style our pages. One of my task was to style to  city card page which displays all the information about each city and the location of the cheapest pint. Using flexbox properties for positioning made the website responsive in a way where it scales good even on small screens. I had to incorporate mapbox map into one of our pages which adds a nice touch for branding.

 ## Wins & Blockers
 I found working as a part of a team very beneficial, collaborative work seemed to amp up my delivery and code quality to a whole nother level and the encouraging team spirit keep our collective work to a high standard.

This was my first time working with Git as a member of a team so I had some teething problems with getting used to checking out and merging feature branches. Good communication was key to avoid major merge conflicts.

## Challenges
Implementing the mapbox was quite challenging. Initially we wanted a map with markers on it showing every location of the map on the backend but when i came across mapbox gl. My team and I came to a conclusion we will go with normal map style where user can search for any location with it including the cities and pubs.

## Key learnings
This project was definitely the most challenging up to date, bringing together everything we'd learnt on the course so far. Working in a team of 4 had its challenges, and I learnt a lot about the importance of stand ups and regular communication. Having each team member taking ownership of their respective area of responsibility, I came to realise the importance of a managing entity in a development team, i.e. to have someone leading the process and holding all the strings.
