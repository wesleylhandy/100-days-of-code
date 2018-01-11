# 100 Days Of Code - Log

<!-- ### Day 0: February 30, 2016 (Example 2)
##### (delete me or comment me out)

**Today's Progress**: Fixed CSS, worked on canvas functionality for the app.

**Thoughts**: I really struggled with CSS, but, overall, I feel like I am slowly getting better at it. Canvas is still new for me, but I managed to figure out some basic functionaliity

**Link(s) to work**: [Calculator App](http://www.example.com) -->

### Day 1: January 1, 2018

**Today's Progress**: Created Repo and initialized CRA for new website to be hosted at http://www.creative.us.com

**Thoughts:** I struggled for focus on a single task. I have a long term goal to solving issues I am having with twitter passport login and create-react-app, but was not motivated to make progress today. I'll get to it tomorrow. I also want to use graphql instead of mongodb on my current backend. However, I set up the repo for mongodb initially. I'll have to change later.

**Link to work:** [Repo](https://github.com/wesleylhandy/creativ.us.com)

### Day 2: January 2, 2018

**Today's Progress**: Solved Twitter CRA OAuth issue by moving away from `passport-twitter` strategy to `react-twitter-auth` and `react-twitter-auth`. 

**Thoughts:** I wanted to solve the passport-twitter and create-react-app issue myself but found it impossible to solve without much further study. I hope to gain better understanding of http methods to be able to build my own express type service from scratch at some point in the future - not for the purpose of reinventing the wheel but for growing in knowledge and experience

**Link to work:** [Repo](https://github.com/wesleylhandy/where-u-at)

### Day 3: January 3, 2018

**Today's Progress**: Moved counter and adding user to state to reducers and actions rather than setting state in React. Begin routing for adding users to going array in db.

**Thoughts:** Moving closer to a final product for this stage of the app. Every little change takes longer to fix since they require decisions on db architecture at a finite level not anticipated at start of project.

**Link to work:** [Repo](https://github.com/wesleylhandy/where-u-at)

### Day 4: January 4, 2018

**Today's Progress**: DB array of going and front-end array of going synced and filted based on date. Added twitter profile image to user. Populated user into going array. Future development to show set of profile images on hover of those going.

**Thoughts:** Honestly, ready to be done, but keep wanted to add features. Want to get list of users who are twitter friends of a given user and display their current choices. Want to allow users to create a list of favorite locations. May not get there for now. Ready to get this operation on Heroku and move on for a bit.

**Link to work:** [Repo](https://github.com/wesleylhandy/where-u-at)

### Day 5: January 5, 2018

**Today's Progress**: Deployed my long-frustrating twitter app for the FCC backed curriculum!!!

**Thoughts:** The functionality of the app in the current state is smooth though I struggled immensely in getting the app deployed to heroku. I was not serializing users properly. And the imageUrl from the twitter profile was not coming through properly in production (for some really weird unknown reason!!!!). There is room for more development in the future, but I'm happy where I'm at right now. 

**Link to work:** [Live Application](https://where-u-at.herokuapp.com/)

### Day 6: January 6, 2018

**Today's Progress**: Fixed bug related to yesterday's deployment. I had neglected to update the React Build before deploying, and I found a fix to my profile image issue. I created repository for next FreeCodeCamp challenge - Stock Viewer App. Also, I spend several hours planning with my new business partner for our side business building sites and mobile applications.

**Thoughts:** Logs are key to debugging. And sometimes seeing a log message when you know there shouldn't be one lets you know you neglected to push an important update - in this case, a rebuild of the front end that solved some bugginess. I also didn't give up and found an easy solution for my profile image problem. 

**Link to work:** [Live Application](https://where-u-at.herokuapp.com/)

**Link to work:** [New Repo](https://github.com/wesleylhandy/stock-viewer)

### Day 7: January 7, 2018

**Today's Progress**: Decided on using [IEX Stocks API](https://iextrading.com/developer/docs/) for the Stocks App. Rather than using Mongoose and setting up Schemas, used `mongodb` package to better mimic Mongo Shell Functions. Also, the backend will not store much data for this project or have user authentication.

**Thoughts:** My plan is to track the date within the state of the application, and update the list of stocks each day from the IEX Api. These stocks will populate a searchable `<select>` element so that users can only search stocks that currently exist and so that stock symbols will be accurate. I will use `socket.io` to update the state of the application across instances and backup the selected stocks in the DB. I am debating on whether or not to also use Redux on the front end of this app as well. I plan on a `create-react-app` front end, using `chart.js` to graphically display stock prices over time.

**Link to work:** [Repo](https://github.com/wesleylhandy/stock-viewer)

### Day 8: January 8, 2018

**Today's Progress**: Refactored api to use version 3.0 of `mongodb` node.js API. Was able to download stock symbols from IEX API and insert into DB and then run an update to insert only new records. 

**Thoughts:** I need to find a faster solution for checking a dataset against the DB and inserting only new records. Currently, I'm checking each individual record to see if it exists in the DB, then creating an array of promises to resolve as a `bulkWrite()` operation on the symbols collection. I'm thinking tomorrow I may choose to get all the records from the DB, stringify the records and compare them to the dataset received from the API, then only update if the two are different, but there has to be a quicker solution.

**Link to work:** [Repo](https://github.com/wesleylhandy/stock-viewer)

### Day 9: January 9, 2018

**Today's Progress**: Created CSS only Stock Ticker. Increased efficiency of upserting new records from API into DB.

**Thoughts:** Making steady progress. I expect to be done with this project much more quickly than others. Of course, I could add additional features, but will just aim for project completion for now.

**Link to work:** [Repo](https://github.com/wesleylhandy/stock-viewer)

### Day 10: January 10, 2018

**Today's Progress**: Integrated Redux and Chart.js. Making steady progress. Objectives seem clear and come to me quickly as I go along. 

**Thoughts:** See the end in sight for version 1. Redux is beautiful! Need to add sockets support for both stock data and across instances of the app.

**Link to work:** [Repo](https://github.com/wesleylhandy/stock-viewer)