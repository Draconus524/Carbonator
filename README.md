##**Inspiration**
Climate change is one of the most significant challenges of our time, and the need for action has never been greater. Carbonator was inspired by the urgent need to empower individuals to take action against climate change. By providing access to critical data, tools, and resources, Carbonator aims to help people understand the impact of their actions and make informed decisions that reduce their carbon footprint. Our goal is to make it easy and accessible for everyone to contribute to the fight against climate change, so we can create a more sustainable future for generations to come. We chose the name Carbonator to suggest that our product provides a broad view of climate patterns, much like a telescope provides a view of the cosmos, encouraging users to explore and investigate the facts on their own in addition to incorporating natural language technology to suggest further ways to get involved.

## **What it does**
1. *Carbonator is a way to quantify your carbon footprint accurately*, compare it to the carbon footprint of others, and measure your improvement or regression over time.
Using our carbon calculator, you can determine how much any particular carbon-emitting activity damages our environment.
To encourage you to maintain lower carbon emissions, a task system has been implemented to walk you through sustainable practices in bite-sized assignments rather than forcing significant commitments and lifestyle changes.
After setting up an account and logging in, a logger will be available to document your carbon emissions in real-time. These measurements will be saved, and used to generate statistics to track your emissions and hold you accountable for your contributions to our global struggle.

2. The application takes two entries, a location and a year date. Using these two points, it obtains historical data regarding this region from multiple datasets provided by Google’s Earth Engine (Google Cloud Platform), including precipitation, temperature, changes in local water level, natural disaster threat levels, and other factors like atmospheric analysis of certain compounds. After obtaining data as far back as the information goes, the application attempts to make a future analysis up until the user’s specified year to date. *The application then returns various data charts and an index of how livable the specified area will be in said year.*

##How we built it
We ran the React application on Flask to get user queries from another IP address and respond with information. We used React.js to access the information from the website as well as display the requested information. We then searched Earth Engine’s repositories for datasets we could use to build our project. We used various Python libraries to analyze the data extracted from Earth Engine, including statsmodels to train the machine learning models, and matlab to generate and send images to the frontend. The app was built with Flask, python, html5, css3, and sqlite3. The SQLite database holds user data on carbon emissions and handles login/logout/signup. The Python scripts perform calculations for the carbon footprint. Flask manages redirects and receives form inputs to be given to the Python scripts.

## Challenges we ran into
Integrating the various APIs into one cohesive web application
How to interpret the data from Google’s Earth Engine. There is a vast repository of data regarding hundreds of different aspects of Earth, and this data is stored as a wide variety of different variables and types. The documentation for each dataset is not as comprehensive as we hoped. *We had to learn how to interpret scientific data and then use technology to analyze and accurately extrapolate said data*. We also had to learn how to efficiently parse through images to cut down a large amount of time it takes to train the model. In addition, the team had to learn new tools such as Flask and server hosting, both of which are essential to the project. While we would have loved to demonstrate analysis of various tools like pixel analysis of vegetation and atmospheric analysis of various compounds, we realized that the processing time was too great for this demonstration and that creation of a truly accurate model would take some more time than we have for this event.


## Accomplishments that we're proud of
*Built an accurate carbon calculator with multiple parameters.*
We are very proud of the web design, as well as the login system. Getting the SQL files to work was a big accomplishment.
We are also proud of our ability to have created a web tool that not only will help people decide where to live, but also educate people about the real effects of climate change and the usefulness of space technologies like satellite sensors and imagery.

## What we learned
*Our team learned how to efficiently analyze large datasets for useful information and trends*, in addition to training a model to make an accurate analysis of said data. We learned how to deploy a functional web app over a server. In addition, some members of the team were introduced to libraries like React.js for the first time.
Also learned how to work with Flask and SQLite, and how to make a front end and back end cooperate better.

## **What's next for Carbonator**
Make an app which would be accessible and used by more people which would make it a conventional standard for all people to check their carbon footprint like they check the temperature and work on it individually to make a change.
We also hope to continue to add more significant features and analyses to our tool. We realized that there are truly vast amounts of information about the climate and Earth in a wide variety of useful categories. Potential features include *better analysis of vegetation, droughts, and natural disasters*. We would also look into stronger prediction models more accurate to the specific dataset.
