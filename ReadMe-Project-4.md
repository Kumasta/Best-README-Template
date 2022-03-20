### General Assembly Project-4: Full-stack Project. 
#  --Hidden Gems--

Contributers: Mayur Kumar, Bashar

### Project Link : TBA

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
      - [Map Page](#map-page)
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
- Javascript
- SASS (CSS)
- JSX (HTML5 via react)

### Back-end
- express: ^4.17.2,
- jsonwebtoken: ^8.5.1,
- mongoose: ^6.2.1,
- mongoose-unique-validator: 2.0.3

### Front-end
- axios: ^0.25.0,
- bootstrap: 5.1.3,
- buffer: ^6.0.3,
- eslint-plugin-react: ^7.28.0,
- mapbox-gl: ^2.7.0,
- react: ^17.0.2,
- react-bootstrap: ^2.1.2,
- react-dom: ^17.0.2,
- react-map-gl: ^7.0.5,
- react-router-dom: ^6.2.1,
- react-router-hash-link: ^2.4.3,
- react-scripts: 5.0.0,
- react-select: ^5.2.2,
- sass: ^1.49.7

## Install
<img width="184" alt="Screenshot 2022-02-21 at 17 42 32" src="https://user-images.githubusercontent.com/94964514/155004644-f473a963-d049-421c-bae0-3f0cb4125834.png">

If working on local server:  

1. Install mongoDB [https://docs.mongodb.com/guides/server/install/] and start mongo server.       
2. Start database from your terminal `mongosh`   
Back end terminal         
3. Install packages `yarn init`   
4. seed database `yarn seed`   
5. start server `yarn serve`   

Front End terminal    
1. Install packages `yarn`   
2. start site server `yarn start`      

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
