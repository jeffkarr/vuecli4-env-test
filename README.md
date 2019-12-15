# vuecli4-env-test
test of using process.env with vue cli version 4 

1. Installed latest version of vue cli.  ("@vue/cli-service": "^4.1.0")
2. Used vue create vuecli4-env-test to create a new app locally. 
    Note:
        When creating app, I chose to manually select features in order to turn eslint off. 
        I did use the babel compiler. I used npm as package manager. All else turned off.  
3. Modified App.vue to remove most boilerplate and added a p tag to show an apikey for a test. 
4. Modified HelloWorld component to indicate app is for process.env tests. 
5. Added new .env file and populated with a dummy apikey. 
    VUE_APP_APIKEY=1234567890
6. Verified that .gitignore contained .env in it. This will skip pushing the .env file to github. 
7. Ran local dev test. npm run serve.
8. Ran npm run build.
8. Added basic express server.js file to serve the dist folder. 
    Then ran npm install --save express.
9. Tested new node server by running node server.js locally after a build. 
10. git cloned local project folder to my github project. 
11. git add, git commit, git pushed the code to my github project.
12. On Github, verified that the .env file did not exist in the repo. 
13. Created new app on Heroku. Connected Heroku app to my github project. 
14. In Heroku, manually deployed github project to Heroku app.
15. In Heroku, went into settings tab and added the .env apikey to config vars. 
16. In Heroku, manually deployed github project to Heroku app after entering the config vars. 
17. Launched Heroku app and verified that apikey was visible, as expected. 

<a href="https://vuecli4-env-test.herokuapp.com">vuecli4-env-test</a>


