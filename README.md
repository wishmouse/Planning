# Planning

Tandem aims to create an active, fun safe community for people wanting to share rides in Aotearoa NZ

#Notes
create profile
based on craigslist
classified ads, create listing

save $$
split cost of travel, food, accomodation.
make connections with people (tagline)
when they're going. what their budget is. where they're staying..
you can rate users
browse profile of users, message each other..

concerts, wedding tourism, exercise tourism?

budget
destination
date

#Technologies:

- Knex, PostgreSQL
- bcrypt-node & OAuth w/ OAuth facebook strategy
- server ( express )
- hbs
- tape / nightwatch

#PostgreSQL Database Schema

##users table:
- userID - auto incrementing
- name - string
- email - string
- hashed password
- ratings? - integer?
- comments? - string

##listings table:
- listingID - auto incrementing
- userID - string
- origin - string
- destination - string
- time-date - timestamp? integer?
- description - string

##rides table:
- rideID - auto incrementing
- listingID
- driver(userID)
- passenger(userID)
- Accepted - boolean

##comments table:
- listingID
- commentID - auto incrementing
- commenterID (userID)
- comment - string
