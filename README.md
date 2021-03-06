

# Green Wallet Staging/Integration

[![Build Status](https://api.shippable.com/projects/54e3067d5ab6cc13528c48c9/badge?branchName=master)](https://app.shippable.com/projects/54e3067d5ab6cc13528c48c9/builds/latest)

<b>Caution:<b> DO NOT TAKE THIS BADGE AS AN INDICATOR OF A PRODUCTION READY APP.

This project is still in development & is not suitable for production use.

Some key features are still missing and will be integrated in the coming weeks.


<u>Join the Green Wallet project by submitting your pull requests today! Forks & branches are encouraged!</u>

# Getting Started
- Download & Install the latest version of Meteor.js framework
- Configure your coins daemon or QT with the proper RPC User/Password settings.
- Edit the settings.json file in the project root to match your wallet RPC user/pass/port etc.
- From the command line run the follow: meteor --settings="settings.json"

(If you're unsure what to work on, search "TODO:" in the project directory or find the list on github and find something that needs work!)

# TODO's:

- Insert new mongo document for each generated address (half done, currently pulling from daemon directly).
- ~~Insert new mongo document for sent transactions.~~
- ~~Daemonize getInfo server method and update details in network collection.~~
- ~~Calculate sent tx from DB~~
-- ~~Calculate receieved tx from DB~~
- Configure coin daemon walletnotify feature to insert incoming tx's into our database.
- Add transaction pagination 
- Make the user settings actually work... (form is already in place, just need to pull from DB).
- Add basic unit testing using Mochajs/Chai.
- ~~Add basic integration testing using Mochajs/Phantomjs & Casperjs.~~
- ~~Setup shippable.com continuous integration file & bash script (SubCreative will do this).~~
- Log server method errors & possibly add a gaurd dog / spam watch for potential attacks.
- Add a walletCount function to determine the current count of wallets for each user.
- Push new address to our account document by using label name from input (ie. Savings).

# TESTING

Add some tests cases, don't be scurred.

# Known Issues:

- Received transactions is not in sync, see TODO's we have an item on the list.
