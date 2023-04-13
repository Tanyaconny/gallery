Milestone 1: Set up
To begin with, I forked and cloned the existing repository, which is an already working application that needs to be translated into a cloud-based application. The application uses a database, and for deployment to Heroku with MongoDB, I used MongoDB Atlas, a cloud-hosted MongoDB service. I followed a short video tutorial to set up a cluster and database user on MongoDB Atlas. I then updated the _config.js file, replacing <USERNAME> and <PASSWORD> with the username and password for the user I created.

Milestone 2: Basic pipeline
To create a basic pipeline, I first ensured that the repository had no tests. I then created a JenkinsFile with the required instructions:

    The pipeline should trigger automatically whenever a new change is pushed to the repository.
    It should ensure that all required software is available, which I figured out from the project requirements. I used npm install to install the required software.
    It should deploy to Heroku using node server to start the server.
    After creating the pipeline, I made a change to the landing page of the website, adding a big “MILESTONE 2” to the site. I then pushed all my changes and made sure that the website I saw through Heroku showed MILESTONE 2.

Milestone 3: Tests
I then switched to the test branch of the repository and found that the repository did have tests. I ran the tests locally using npm test, and the test results looked good. I then merged the test branch with my main branch and updated my JenkinsFile to execute the tests as part of the pipeline. I set up the pipeline to send an email if the tests failed. Next, I made a change to the landing page of the website, adding a big “MILESTONE 3” to the site. I pushed all my changes and made sure that the website I saw through Heroku showed both MILESTONE 2 and MILESTONE 3.

Milestone 4: Slack integration
For Slack integration, I created a Slack channel called Tanyaipgit and invited my team member to it. I updated the pipeline so that on a successful deploy, a Slack message was sent on that channel. The message included the build ID and the link to Heroku where the site was uploaded. I then made a change to the landing page of the website, adding a big “MILESTONE 4” to the site. I pushed all my changes and made sure that the website I saw through Heroku showed MILESTONE 2, MILESTONE 3, and MILESTONE 4.

Conclusion:
In conclusion, I successfully deployed a cloud-based application using MongoDB Atlas, Jenkins, and Heroku. The project involved translating an existing application into a cloud-based application, setting up a basic pipeline, automated testing, and Slack integration. The milestones were completed successfully, and I made sure that the website I saw through Heroku showed all the milestones.

