<img src="https://i.imgur.com/UDnNX4I.jpg"/>

# Express Lab
# My Dev Skills - Part 2
---

## Intro

In recent lessons you saw how to use HTML forms and Express middleware, such as:

- `method-override`

to perform **Create**, **Update** & **Delete** data operations in an Express application.

This lab builds upon the `express-dev-skills` project you created in the _My Dev Skills - Part 1_ lab where the **Read** data operations were implemented.

##### This Lab is a Deliverable

## Exercises

The goal of the lab is to do put in a rep doing everything that you did during the _Express - Middleware_ lesson by adding the following functionality to the `express-dev-skills` project:

1. Display an _Add Skill_ link on the **index** view that when clicked, displays a **new** view that includes a form for entering a new Dev Skill.

2. When a new Dev Skill is submitted, add the skill to the simulated "database" and redirect the user to the **index** view.

3. On the **show** view, display a _Delete Skill_ button (the submit button within a `<form>`) that when clicked, deletes the skill from the "database" and redirects to the **index** view.

Note: All routes should follow those described in the [RESTful/Resourceful routing chart](https://gist.github.com/jim-clark/17908763db7bd3c403e6)

##### Hints

- Be sure to install, require & mount the `method-override` middleware.

## Bonus Exercises

1. On the **show** view, display an _Edit Skill_ link that when clicked, displays an **edit** view that displays a form for editing that Dev Skill.

2. When the edit Dev Skill form is submitted, the skill should be updated in the "database" then redirect the user back to the **show** view.

##### Hints

- The controller action will need to get the Dev Skill being edited using the `Skill` Model and pass it to the **edit** view.
- Prefill `<input>` elements by using the `value` attribute and some EJS tags to write out the data properties of the skill passed in, for example, an `<input>` used to edit a skill's `name` property would look like the following (assuming you passed a `skill` object for the previous hint):

	```html
	<input type="text" name="name" value="<%= skill.name %>">
	```

### This Lab is a Deliverable

Please submit the URL of your `express-dev-skills` GH repo as directed.

