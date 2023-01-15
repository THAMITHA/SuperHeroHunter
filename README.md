# Super Hero Hunter

# The data is accessible through a REST API
# API References
BASE URL = https://superheroapi.com/api/access-token
# e.g.- https://www.superheroapi.com/api.php/3306871969584088/555/image
access-token  = 3306871969584088

# Authentication for Server-Side Applications
Server-side applications must pass two parameters in addition to the apikey parameter:

ts - a timestamp (or other long string which can change on a request-by-request basis)
hash - a md5 digest of the ts parameter, your private key and your public key (e.g. md5(ts+privateKey+publicKey)
# For example, a user with a public key of "1234" and a private key of "abcd" could construct a valid call as follows: http://gateway.marvel.com/v1/public/comics?ts=1&apikey=1234&hash=ffd275c5130566a2916217b101f26150 (the hash value is the md5 digest of 1abcd1234)

# Use the Marvel API:  https://developer.marvel.com/docs 
Register yourself to the above website https://developer.marvel.com/signup and generate the public and private key.
Now follow the instruction on how to use the API key https://developer.marvel.com/documentation/authorization. You need to use the timestamp as ts and then create the hash using md5 hash of ts, private-key and public-key. 
How to generate md5 hash? 
<!-- // first install crypto-js
npm install crypto-js
// now use md5 as below
var MD5 = require("crypto-js/md5"); 
console.log(MD5("text to hash").toString()); -->

# Requirement
Create a superhero hunter app using only vanilla javascript.

## Set up and execution  
  Open the index.html file in your preferred browser

## Application flow
  * Start searching for you favourite hero by typing into the search bar
  * You will suggestions as you type
  * Click on your favourite heros name from the suggestions to see an in detail info about the selected super hero
  * If you want to add a particular hero from suggestions to your list of favourite hero click on "Add to favourites" option next to the hero name
  * You can un favourite a hero too from suggestions
  * You can navigate to your Favourite heros page from by clicking on the favourite heros link on the top right corner of the home page 
  * You can view a list of your favourite super heros in the favourites page and can remove a super hero from this list by selecting the respective option



