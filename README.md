# quaroutine

## Overview
The outbreak of COVID-19 has proven to be a stressful and anxiety-provoking time for many people. Seeing as the entire world is currently undergoing quarantine conditions, we were inspired to create a tool that would help the community adapt to these social changes by creating a routine. We envisioned a platform that would encourage everyone to 1) help themselves through developing healthy & enjoyable habits 2) help others by contributing to those businesses/hospitals/vulnerable populations in need.


## Data Model

The application will have two large categories - "Help Yourself" and "Help Others" and each activity has a name, a description, a website, and a smaller filter 

* users can have multiple lists (via references)
* each list can have multiple items (by embedding)
* 
*


2 Example Activities:

```javascript
{
  name: "Facebook's Community Help Directory",
  description: 'Facebook\'s location-based board for individuals offering and requesting help (supplies, errands, information) within their local communities.',
  site: "https://www.facebook.com/coronavirus_info/request_offer_help/",
  category: 'community volunteering'
}
{
  name: "#findthemasks",
  description: 'How and where to donate masks and other protective equipment for healthcare workers.',
  site: "https://findthemasks.com/,
  category: 'medical supplies'
}
```

An Example Category: 

```javascript
{
  user: // a reference to a User object
  name: "Breakfast foods",
  items: [
    { name: "pancakes", quantity: "9876", checked: false},
    { name: "ramen", quantity: "2", checked: true},
  ],
  createdAt: // timestamp
}
```


## [Link to Commented First Draft Schema](db.js) 

(___TODO__: create a first draft of your Schemas in db.js and link to it_)

## Wireframes

(___TODO__: wireframes for all of the pages on your site; they can be as simple as photos of drawings or you can use a tool like Balsamiq, Omnigraffle, etc._)

/list/create - page for creating a new shopping list

![list create](documentation/list-create.png)

/list - page for showing all shopping lists

![list](documentation/list.png)

/list/slug - page for showing specific shopping list

![list](documentation/list-slug.png)

## Site map


## User Stories or Use Cases

1. as non-registered user, I can register a new account with the site
2. as a user, I can log in to the site
3. as a user, I can drag the boxes (of activities)/items to a list (daily schedule form)
4. as a user, I can add activities (either under #helpyourself or #helpothers)
5. as a user, I can share my quaroutine with others
6. as a user, I can access the same daily schedule again the next day

## Research Topics

* (5 points) use React
* (1 point) form submit? how do we approve?
* (1 point) google calendar api? not sure. some kind of scheduling library
* (1 point) cookies
* (1 point) bootstrap
    * we will use a reasonable amount of customization of the css framework


## [Link to Initial Main Project File](https://github.com/jacquine/quaroutine) 
(this is a link to our create-react-app we made, barebones still)

## References 

1. [passport.js authentication docs](http://passportjs.org/docs) - (add link to source code that was based on this)
2. [react doc](https://reactjs.org/) - (add link to source code that was based on this)