# RESTful API using Node.js and MongoDB

## Install and Run

In the root directory, run `npm install` in the console.

Run `npm run start` to start the server.


#RESTful API documentation

# Rooms:
Represents talk details
____________________________________________________
# Room attributes:

title(String) : Title of the talk
room(Number) : Room number where talk is taking place.
name:(String) : Speaker name.
company:(String) : Speaker’s company name.
email:(String) : Speaker email.
bio:(String) : Speaker bio.

# HTTPS requests used:
# Get the list of all rooms
GET: /rooms

# Add a room to the conference
POST:/rooms/add

# Add an attendee to a room(talk)
POST: /add/:attendeeId/:roomId
 
# Remove an attendee to a room(talk)
POST:/remove/:attendeeId/:roomId


# Attendees:
Represents attendee details
____________________________________________________
# Attendee attributes:

name:(String) : Attendee name.
company:(String) : Attendee’s company name.
email:(String) : Attendee email.
registered:(Date) : Date of when attendee registered.


# HTTPS requests used:
# Get the list of all attendees
GET: /attendees

# Add an attendee
POST:/attendees/add

# Get specific attendee by Id
GET: /attendees/:attendeeId
 
 
 ### Sample JSON for project:


    
    {
    "title": "Talk 1",
    "room": 101,
    "speaker": {
      "name": "Hendrix Carroll",
      "company": "Songlines",
      "email": "hendrixcarroll@songlines.com",
      "bio": "Magna velit adipisicing ullamco sint duis nisi."
    },
    "attendees": [
      {
        "name": "Sanders Riley",
        "company": "Comtext",
        "email": "sandersriley@comtext.com",
        "registered": "2015-05-24T02:15:04 +07:00"
      }
     ],
    }
     
  
 
