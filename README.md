# NodejsExpressMongodb
A small application using NodeJs, Express Web framework, jQuery and MongoDB
This is a follow up to the tutorial http://cwbuecheler.com/web/tutorials/2014/restful-web-app-node-express-mongodb/
This project uses PUT to update data in MongoDb using Ajaxs.

#Instructions to install
Import github repo to Webstorm

1. Download Webstorm
2. CLone Repo from github
3. Update all dependencies: npm install
4. Run sudo npm install -g express-generator to have the scafolding(in case something is missing)
5. start server by typing npm start(Express 4.0)
6. Add /usr/local/bin (if is not there already) to PATH: Type --> sudo nano /etc/paths

Install MongoDB
1. Download MongoDB
2. Install homebrew(install things that macos does not have)
3. Open terminal and type: ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
4. Update homebrew: brew update
5. Install mongodb by doing bbrew install mongodb
   -If mongodb is already installed, do brew update first and then brew upgrade mongodb
6. Extra InfO:
To have launchd start mongodb at login:
    ln -sfv /usr/local/opt/mongodb/*.plist ~/Library/LaunchAgents
Then to load mongodb now:
    launchctl load ~/Library/LaunchAgents/homebrew.mxcl.mongodb.plist
Or, if you don't want/need launchctl, you can just run:
    mongod --config /usr/local/etc/mongod.conf

7. To run mongodb DB server with data from github repo(Data folder)
   - Go to mongodb folder in the system: /usr/local/var/mongodb
   - Once you cd there, run the following: mongod --dbpath /Users/danilocarrion/WebstormProjects/NodejsExpressMongodb/data
8. Since nodejs server and Mongodb server are running, you can go to localhost:3000/  and it will take you to the Restful app.

*ssh awshost1