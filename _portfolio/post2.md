---
layout: post
title: Blocmetrics
feature-img: "img/sample_feature_img.png"
thumbnail-path: "img/blocmetrics.png"
short-description: API Tracking Service & Reporting

---
#### Blocmetrics is a:

* Client-side JavaScript snippet that allows a user to track events on their website.
* Server-side API that captures and saves those events to a database.
* Rails application that displays the captured event data for a user.

### Application Features

#### User Story:
  * A user can sign up for a free account by providing a name, password and email.
  * A user can sign in and out of Blocmetrics.
  * A user can register an application for tracking.
  * A user can associate events with a registered application.
  * A user can see a graph of events for each registered application.

#### Authentication with Devise:
Blocmetrics incorporates [Devise](https://github.com/plataformatec/devise) for user authentication. The authentication system allows users to sign up and sends emails for account confirmation. Users can sign in and out of Blocmetrics.

#### CORS
Client-side JavaScript sends an AJAX request to the Blocmetrics API so that it can store events. Browsers normally do not allow such cross-origin requests to occur. This is to prevent security vulnerabilities such as cross-site scripting. CORS allows us to allow cross-origin requests in a controlled manner without opening up security vulnerabilities.

CORS works by making a preliminary request to the target server, asking if the cross-domain request will be permitted.

#### Chartkick & Groupdate
To show events for each registered application Blocmetrics uses [Chartkick](https://github.com/ankane/chartkick#installation) and [Groupdate](https://github.com/ankane/groupdate). Using Groupdate, Chartkick allows for a line chart of events over time.

#### Video Walk Through
<iframe width="560" height="315" src="https://www.youtube.com/embed/Gjd3QbME2-E/0" frameborder="0" allowfullscreen></iframe>

#### Heroku Link
[Blocmetrics](https://still-reaches-71761.herokuapp.com/)
