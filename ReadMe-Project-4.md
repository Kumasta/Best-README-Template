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

#### Giveaways
- Get all `Get /api/giveaways`
- Get one `Get /api/giveaways/{giveaway ID}`
- Post new*+ `POST /api/giveaways`    
![image](https://user-images.githubusercontent.com/94964514/159490560-8f6cc06d-e68a-4fd5-9f06-eb32d55d2aa7.png)
- Update one*+ `PUT /api/giveaways/{giveaway ID}`   
![image](https://user-images.githubusercontent.com/94964514/159490641-bedbb702-c71f-45b2-a78a-e85318c0b998.png)
- Delete one* `DELETE /api/giveaways/{giveaway ID}`

#### Comments   
- Add comment*+ `POST /api/giveaways/comments/`    
![image](https://user-images.githubusercontent.com/94964514/159491006-67b074b8-77ef-4b38-a852-9b4f35d0ec4f.png)
- Updated comment*+ `PUT /api/giveaways/comments/{comment ID}`   
![image](https://user-images.githubusercontent.com/94964514/159491115-6aadcd27-b692-4fd8-8fda-f277654dec96.png)
- Delete comment* `DELETE /api/giveaways/comments/{comment ID}`

#### Login / Register
- Register User+ `POST /api/register`    
![image](https://user-images.githubusercontent.com/94964514/159491227-7023c17c-9e13-4437-8cd4-6fb09d0c2068.png)
- Login user+ `POST /api/login`     
![image](https://user-images.githubusercontent.com/94964514/159491261-a0d3b79c-e058-48f9-b9fc-e95e52d61b60.png)

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
