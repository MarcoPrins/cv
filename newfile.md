# Curicculum Vitae for Marco Prins

*Last updated 11 September 2016*

## Basic info

```ruby
basic_info = {
  first_name:        :marco,
  last_name:         :prins,
  date_of_birth:     Date.new(1992, 9, 30),
  nationality:       "South African",
  address:           "28 Ludlow road, Vredehoek",
  email:             "snirpocram@gmail.com",
  phone:             "074 581 2845",
  rails_experience:  (2.years + 10.months)
}

links = {
  stackoverflow:     "http://stackoverflow.com/users/2923108/marco-prins",
  facebook:          "https://www.facebook.com/marco.el.presideno"
}
```

## A brief introduction

I am a Rails developer. Keen guitarist. Love nature & the outdoors. Afrikaans.

## Work experience

### Miscellaneous
* Guitar teacher at **Deanian Music** - *Part time, 2009*
* Waiter at **Aandklas Stellenbosch** - *Part time, 2013*
* Internship at **Springlab** (Python and HTML) - *Part time, 2013*
<br>

### Shopstar
***November 2013 - October 2015***
<br>
***Website: https://shopstar.co.za***

I started out at Shopstar with only moderate programming skills, and some HTML/CSS knowledge. I had no real experience with web technology / backend.
<br>
I learned Ruby and Rails working there.
We were 2 developers, we used Rails daily, and we built the front- and backend. Since we were the only devs Shopstar was our baby - We did everything. Deployment, frontend, backend, DevOps, bug fixes. It was awesome.
<br>
Shopstar started out as a single Rails app, and as it grew we split it out into an API (Rails) communicating via JSON with the legacy app (Rails) which handles the admin/cms and shopfronts, an auth service (Backbone.js), a POS system (Ember.js), and a Reviewing and user profile system called ShopstarU (Ember.js) which I built completely on my own (You can view it at https://u.shopstar.co.za).
<br>
By the end of 2015 I got pretty used to using an API to communicate data over JSON (Using JSON:API spec).
We used to store all our images on the one server, but as we grew and split our system onto different servers, moved them to Amazon S3.
<br>
We also considered building an API in Scala, and started playing around with the Play framework, but decided Rails was a lot quicker to develop so we used that instead.
<br>
We used Vagrant to simulate server environments, and construct provisioning scripts that way. I provisioned the server serving the frontend applications (Auth and ShopstarU) using pure shell scripts.
<br>
We ran a standard MySQL database, and it's set up to communicate with both the API app and Legacy app. By the time I left we tried to move everything to communicate through the API, so that all new additions use the API to access the database. We deployed Rails via Capistrano.
<br>
To deploy the Ember app, I wrote a plain and simple bash script to RSync the built files to the server. I don't know if they've changed it since, but it worked pretty well.
Some stuff that I've built (on my own) since joining Shopstar include (to name a few)

* A sales Statistics Report system, which shows detailed breakdowns and graphs of your sales for an adjustable time period.
* A shopfront design manager, which has an interface in the CMS to adjust colours, layout, styling, etc. and when you submit the form, it saves to a database table called Design, and runs a callback which pulls a standard SASS template, embeds your settings from the database as variables into the template, compiles it into CSS with a SASS compiler, and then saves your shop's own css file, which is included in your shopfront. These files are kept in a shared directory
* A system for creating specials for a selected subset of your products
* A voucher system (with a generated voucher code)
* A customised exception logger for the entire app
* A daily job that backs up the database and pushes it to S3
* A script that moved shops from another platform (They were called Ammo, and they closed down their service) and mapped the data to fit our system, and pushed their clients (like 30 or so) into our system.

And a lot more other stuff. I can't think of all of them. You can get a pretty good idea of the stuff we've done by creating a free profile :).
On the frontend side we used the standard stuff - jQuery, a bit of CoffeeScript. And we used HAML for all templates.
<br>

### Prodigy Finance
***Since November 2015***
<br>
***Website: https://prodigyfinance.com***

Prodigy has been a whole new experience. I started out in a team of about 7 developers and just under 40 people in the whole company. Within 8 months the development team grew to 17 people, and the company to a 100. The dev team was split into two teams of 8 and 10 members (with one member in both teams, following a guild structure). I'm part of the smaller team (8 members), the "backspace" team - mainly focussing on backend structure and owning all independent API services. We still do a lot of front-end for the admin interfaces for the external apps.
<br>
In 8 months I've learnt a whole new side to development. I've got completely stuck into SCRUM and agile development. Gotten used to structured communication, continuous integration and being a moving part of a bigger machine.
<br>
We use EngineYard for DevOps. Switched from semaphore to Snap-ci for a continuous integration tool. I've learnt a massive amount about automated testing. Writing unit tests, integration tests, Capybara feature tests and teaspoon front-end tests. At Prodigy nothing is left untested and extra care is taken to educate and improve each individual's automated testing knowledge, capabilities and habits - including two weekly sessions of practice, discussions and reviews. It's a very stimulating environment to learn about better ways to program.
<br>
I've also been part of all the scrum steps - as most of the QA in my team was done by the devs. We use JIRA and follow strict SCRUM.
<br>
It's a much larger app and team than Shopstar and my scalable programming skills have completely taken off from where I left. I've noticed a lot of things about how scalable programming can make life easier in so many ways.
<br>
My work at Prodigy so far has included:

* Working on an automated credit committee application with an API accessed by the main platform
* Building smart admin interfaces to bring data alive and to make life easy for the people using it
* Working on the student application management platform
* Building lots and lots of detailed and robust reporting systems for business use, sometimes with Ruby and ActiveRecord, and sometimes with raw SQL
* Helping to build a step-by-step student application process with advanced front- and backend validations
* Designing data structures
* Helping a lot with large-scale code refactors, extractions into separate applications, optimizations and structural improvements in an extremely fast-growing application and environment
* Helping with Quality Assurance and Code Reviews

## Summary of skills

### Very good:

* Ruby
* Rails
* MVC
* Git + GitHub
* SQL (MySQL, PostgreSQL) and databases
* JQuery and AJAX
* HTML, html.erb, haml
* CSS, Sass
* RSpec, FactoryGirl, Capybara and automated testing
* Unix Terminal and OS X
* Data fixes and persistence structures
* HTTP(S), Network communication, JSON, API's, Auth, etc..
* Amazon S3 and s3cmd
* Continuous Integration
* Scrum / Agile

### Good:

* Linux
* Ember.js
* Plain JavaScript
* Front-end unit tests and teaspoon
* Elasticsearch
* Functional programming style
* Java
* Python


### I forgot most of it and can't really be bothered with it:

* C
* Scala
* Nginx
* Bash (those if-statement syntaxes..)
* SSH keys. I hate SSH keys

## Education

### School

Here are my grades from matric:

```ruby
grades = {
  matematics:                       81,
  engineering_graphics_and_design:  77,
  afrikaans_home_language:          65,
  english_home_language:            65,
  geography:                        60,
  physical_science:                 64
}
```

### University of Stellenbosch

Here are my passed subjects so far from my (still unfinished) BSc CompSci degree:

* Computer Science `114`, `144`, `214` 
* Applied Mathematics `114`; `144`; `214`
* Mathematics `114`
* Physics `114`
* Music Technology `114`

I dropped out because of financial reasons. I'd like to continue studying through UNISA some time