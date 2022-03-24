### General Assembly Project-4: Full-stack Project. 
#  --Giveaway Bae--

Contributors: Mayur Kumar, Bashar Othman

### Project Link : https://mayur-sei-porject-4.herokuapp.com/
<img width="1440" alt="image" src="https://user-images.githubusercontent.com/94964514/159168887-5d5fdad7-fa66-4b60-abf1-4a6e04b6650d.png">

## Table of Contents

- [Brief](#brief)
- [Concept](#concept)
- [Languages, Packages and, technology used](#languages-packages-and-technology-used)
  - [Back-end](#back-end)
  - [Front-end](#front-end)
- [Approach](#approach)
    - [Document-Model-Breakdown](#document-model-breakdown)
    - [API-End-Points](#api-end-points)
    - [Front-end components](#front-end-components)
      - [Nav-Bar](#nav-bar)
      - [Home Page](#home-page)
      - [Showcase](#showcase)
      - [Gem Form](#gem-form)
      - [Profile Page](#profile-page)
      - [Styling](#styling)
      - [Seeding](#seeding)
- [Challenges](#challenges)
- [Future Improvements](#future-improvements--changes)
- [Main Takeaways](#main-takeaways)

## Brief


## Concept


## Languages, Packages and, technology used:
- JavaScript
- JSX (HTML5 via react)
- Python 

### Back-end
- django
- psycopg2-binary
- pylint 
- autopep8
- djangorestframework
- pyjwt

### Front-end
- @chakra-ui/icons
- @chakra-ui/react
- @emotion/react
- @emotion/styled
- @react-icons/all-files
- @testing-library/jest-dom
- @testing-library/react
- @testing-library/user-event
- axios
- buffer
- emotion-theming
- fontsource-inter
- framer-motion
- react
- react-dom
- react-dotenv
- react-router
- react-router-dom
- react-scripts
- react-select

## Approach


### Document Model Breakdown. 

#### User Model

#### Pin Model


### API-End-Points
(* secure route)   
(+ Body required)   
({ } id/text/token)

#### Giveaways
- Get all `Get /api/giveaways/` 
- Get one `Get /api/giveaways/{giveaway ID}/` 
- Post new*+ `POST /api/giveaways/`     
![image](https://user-images.githubusercontent.com/94964514/159490560-8f6cc06d-e68a-4fd5-9f06-eb32d55d2aa7.png) 
- Update one*+ `PUT /api/giveaways/{giveaway ID}/`    
![image](https://user-images.githubusercontent.com/94964514/159490641-bedbb702-c71f-45b2-a78a-e85318c0b998.png) 
- Delete one* `DELETE /api/giveaways/{giveaway ID}/`    

For the purpose of a user being able to "watch" a giveaway, we stored the giveaway Id in the user profile in a watchlist and the user ID is stored in the giveaway record in a watcher_list field. At the time of building this project we were not able to figure out a smooth way to do this in one request. So we made an end-point for the giveaway so that the User does not need to be the owner of the giveaway to update that ID array. For ease of checking & updating the array we create an unpopulated GET endpoint to get an array of numbers and not objects. 

- Get one unpopulated giveaway `GET /api/giveaways/update/{giveaway ID}/`     
- Update giveaway* (Non-owner) `PUT /api/giveaways/update/{giveaway ID}/`     
![image](https://user-images.githubusercontent.com/94964514/159493219-fb550337-69a4-4ea4-b9fe-0bd690266f90.png) 


#### Comments   
- Add comment*+ `POST /api/giveaways/comments/`     
![image](https://user-images.githubusercontent.com/94964514/159491006-67b074b8-77ef-4b38-a852-9b4f35d0ec4f.png) 
- Updated comment*+ `PUT /api/giveaways/comments/{comment ID}/`     
![image](https://user-images.githubusercontent.com/94964514/159491115-6aadcd27-b692-4fd8-8fda-f277654dec96.png) 
- Delete comment* `DELETE /api/giveaways/comments/{comment ID}/`  

#### Login & Register
- Register User+ `POST /api/register/`      
![image](https://user-images.githubusercontent.com/94964514/159491227-7023c17c-9e13-4437-8cd4-6fb09d0c2068.png) 
- Login user+ `POST /api/login/`     
![image](https://user-images.githubusercontent.com/94964514/159491261-a0d3b79c-e058-48f9-b9fc-e95e52d61b60.png) 

#### User Profile
- Get one profile `GET /api/profile/{user ID}/`     
- Update own profile*+ `GET /api/profile/{user ID}/`     
![image](https://user-images.githubusercontent.com/94964514/159491699-71dc50bf-ffed-4ff6-a008-4aa8c04e3608.png) 
- Delete user* `DELETE /api/profile/{user ID}/` 

#### Regions & Categories
For the purpose of populating drop down select forms  
- Get all regions `Get /api/regions/` 
- Get all categories `Get /api/categories/` 

### Front-end components

#### Nav-Bar

Deskop:       
<img width="1298" alt="image" src="https://user-images.githubusercontent.com/94964514/159913196-98bb7182-6718-41ec-957a-57552f3a9ebe.png">

Mobile:       
<img width="768" alt="image" src="https://user-images.githubusercontent.com/94964514/159913271-30318b1c-288d-44e5-9b9e-b111d5cd3328.png">


#### Home page

Dark mode on Banner:

![Dark mode on banner](https://user-images.githubusercontent.com/94964514/159914783-97dcf0fc-5a71-48db-bfbe-b86f4de0d8d0.gif)

Carousel:

![Carousel gif](https://user-images.githubusercontent.com/94964514/159914218-7b69cf6f-5dac-4441-9389-4cc0aa2def0a.gif)


#### Showcase

Main:     

![Showcase top](https://user-images.githubusercontent.com/94964514/159915319-59b1c998-dbf9-4caf-b3de-f476e96ed78c.gif)

Comment section:      

![Comment gif](https://user-images.githubusercontent.com/94964514/159915927-b1e9d24e-2f8c-4015-bef0-1630377adac4.gif)

#### Search Page

![SearchPage](https://user-images.githubusercontent.com/94964514/159916656-bea7c970-a8c9-4a5e-af53-09a02daaf02d.gif)

#### Dashbaord page

![Dashboard](https://user-images.githubusercontent.com/94964514/159918084-23fb5a89-c78d-46ac-bfc1-8a4491cfc28c.gif)

Form Errors:

![Toast](https://user-images.githubusercontent.com/94964514/159918902-3b12a220-aa9f-407f-b410-db8ead8d8c70.gif)

#### Profile Page

<img width="600" alt="image" src="https://user-images.githubusercontent.com/94964514/159917150-55d74e84-6eb2-4008-bc23-9ab2931da77a.png">

### Styling

### Seeding

## Challenges

## Future Improvements / Changes

## Main Takeaways


