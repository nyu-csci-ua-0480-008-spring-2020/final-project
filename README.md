# quaroutine

## Overview
The outbreak of COVID-19 has proven to be a stressful and anxiety-provoking time for many people. Seeing as the entire world is currently undergoing quarantine conditions, we were inspired to create a tool that would help the community adapt to these social changes by creating a routine. We envisioned a platform that would encourage everyone to 1) help themselves through developing healthy & enjoyable habits 2) help others by contributing to those businesses/hospitals/vulnerable populations in need.


## Data Model
The application will have two large branches - "Help Yourself" and "Help Others" and each activity has the following: name, description, site, filtering categories. 

* a category has multiple activities
* an activity has the properties: name, description, site, category 

2 Example Activities:

```javascript
{
  name: "Facebook's Community Help Directory",
  description: 'Facebook\'s location-based board for individuals offering and requesting help (supplies, errands, information) within their local communities.',
  site: "https://www.facebook.com/coronavirus_info/request_offer_help/",
  category: "community volunteering"
}

{
  name: "#findthemasks",
  description: 'How and where to donate masks and other protective equipment for healthcare workers.',
  site: "https://findthemasks.com/,
  category: "medical supplies"
}
```

An Example Category: 

```javascript
{
  user: // a reference to a User object
  name: "medical supplies"
  list: [
    { name: "#findthemasks", id: "9876", checked: true},
    { name: "mask-match", id: "5423", checked: true},
  ],
  submittedBy: username, // could this be connected to google cal?
  submittedAt: //timestamp
}
```

### [Link to Commented First Draft Schema](db.js) 

## Wireframes
[click here for a simple prototype](https://www.figma.com/file/itAqlX48A355QwhHh8yYTk/Quaroutine?node-id=0%3A1)

## Site map
landing page (split screen, hover)
    -- calendar
    -- help others - (different categories)
    -- help yourself- (different categories)
    -- submit new activity

## User Stories or Use Cases

1. as non-registered user, I can register a new account with the site (not sure)
2. as a user, I can log in to the site (not sure)
3. as a user, I can drag the boxes (of activities)/items to a list (daily schedule form)
4. as a user, I can add activities (either under #helpyourself or #helpothers)
5. as a user, I can share my quaroutine with others (by capturing the schedule as an image/using it as a template)
6. as a user who loves to schedule and block out time, I can modify the boxes to the duration I want 

## Research Topics

* (5 points) use React
* (1 point) form submit for approval
* (1 point) google calendar api? not sure. some kind of scheduling/calendar library
* (1 point) cookies
* (1 point) bootstrap
    * we will use a reasonable amount of customization of the css framework


### [Link to Initial Main Project File](https://github.com/jacquine/quaroutine) 
(this is a link to our create-react-app we made, barebones still)

## References 

1. [passport.js authentication docs](http://passportjs.org/docs) - (add link to source code that was based on this)
2. [react doc](https://reactjs.org/) - (add link to source code that was based on this)
3. [google calendar API](https://developers.google.com/calendar)