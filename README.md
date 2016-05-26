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

#PostgreSQL Database
- users table: userID, name, email, hashed password, 
- listings table: listingID, to, from, time, date (maybe time & date are one field?), userID, description
- rides table: listingID, driver(userID), passenger(userID), Accepted(boolean)
- comments table: listingID, commenterID (userID), 
