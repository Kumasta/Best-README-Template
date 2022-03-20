### General Assembly Project-4: Full-stack Project. 
#  --Giveaway Bae--

Contributers: Mayur Kumar, Bashar Othman

### Project Link : TBA
<img width="1440" alt="image" src="https://user-images.githubusercontent.com/94964514/159168887-5d5fdad7-fa66-4b60-abf1-4a6e04b6650d.png">

## Table of Contents

- [Brief](#brief)
- [Concept](#concept)
- [Languages, Packages and, technology used](#languages-packages-and-technology-used)
  - [Back-end](#back-end)
  - [Front-end](#front-end)
- [Install](#install)
- [Approach](#approach)
    - [Document-Model-Breakdown](#document-model-breakdown)
    - [API-End-Points](#api-end-points)
    - [Front-end components](#front-end-components)
      - [Nav-Bar](#nav-bar)
      - [Home Page](#home-page)
      - [Chowcase](#showcase)
      - [Gem Form](#gem-form)
      - [Profile Page](#profile-page)
      - [Styling](#styling)
      - [Seeding](#seeding)
- [Challenges](#challenges)
- [Future Improvments](#future-improvements--changes)
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

#### Main documents (pins)
- Get all `Get /api/pins`
- Get one `Get /api/pins/{pin ID}`
- Post new*+ `POST /api/pins`    
![image](https://user-images.githubusercontent.com/94964514/155016630-0338f716-fdda-4520-bf81-410db1c59b4e.png)
- Update one*+ `PUT /api/pins/{pin ID}`   
![image](https://user-images.githubusercontent.com/94964514/155016825-4e562a86-c2c2-4cae-b216-e0a3250a73e1.png)
- Delete one* `DELETE /api/pins/{pin ID}`

#### Pin Rating
- Add rating*+ `POST /api/pins/{pin ID}/rating` (Between 1 - 5).   
![image](https://user-images.githubusercontent.com/94964514/155017307-eb729923-826f-41f9-8228-df191e30989e.png)
- Update rating *+ `PUT /api/pins/{pin ID}/rating/{rating ID}` (Between 1 - 5)    
![image](https://user-images.githubusercontent.com/94964514/155017462-bd1b5bb2-b093-4590-b511-c1bc16226987.png)

#### Pin Comment 
(During development we changed terminology from review to comments)     
- Add comment*+ `POST /api/pins/{pin ID}/reviews`    
![image](https://user-images.githubusercontent.com/94964514/155023193-371db78c-07f7-4eef-9be8-a2ae3647470d.png)
- Updated comment*+ `PUT /api/pins/{pin ID}/reviews/{review ID}`   
![image](https://user-images.githubusercontent.com/94964514/155023341-2a0a6ff4-59de-4551-9b51-cba606e84f41.png)
- Delete comment* `DELETE /api/pins/{pin ID}/reviews/{review ID}`

#### Comment like
- Like comment*+ `POST /api/pins/{pin ID}/review/{review ID}/like`        
![image](https://user-images.githubusercontent.com/94964514/155023611-43401d2b-ed57-4d16-abe0-e905c551c4e2.png)
- Unlike comment* `DELETE /api/pins/{pin ID}/review/{review ID}/like/{like ID}`

#### Login / Register
- Register User+ `POST /api/register`    
![image](https://user-images.githubusercontent.com/94964514/155023903-53a24d70-efe8-4591-8ed0-2f9117f5d159.png)
- Login user+ `POST /api/login`     
![image](https://user-images.githubusercontent.com/94964514/155024015-daf589cd-0bf8-4dba-806d-80e4b78a1f93.png)

#### User Profile
- Get one profile `GET /api/profile`    
- Update own profile*+ `GET /api/profile`    
![image](https://user-images.githubusercontent.com/94964514/155024386-6dac1ce5-6922-4580-b11a-183239e4f702.png)

#### Mapbox Geocode API
Enables serach for address on the map. Container props for limited search for Uk & Ireland and fuzzy match.         
`GET https://api.mapbox.com/geocoding/v5/mapbox.places/**{___search_text____}**.json?country=gb,ie&fuzzyMatch=true&access_token=**{_mapbox_token_}**`

### Front-end components

#### Nav-Bar

#### Home page

#### Showcase

#### Gem Form

#### Profile Page

### Styling

### Seeding

## Challenges

## Future Improvements / Changes

## Main Takeaways
