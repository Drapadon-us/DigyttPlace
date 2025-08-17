# ty jalen for the code lmfao

# This project is running at https://place.drapadon.us

Do you want to run your own r/place?

I know rummaging through the code was hard for me to figure out, so here's how!

clone this repository by opening a terminal window and running `git clone https://www.github.com/digytt/digyttplace.git`

make sure you have node.js installed on your machine.

go to /data/config.json and change guildId, guildName, guildInvite, and adminRoles to your own server's.

create a new file in the data folder named 'botdata.js' and inside paste the following:
```
const clientToken = "yourtoken";
const clientId = "yourid";
const clientSecret =  "yoursecret";

export {clientToken, clientId, clientSecret};
```

go to https://discord.com/developers/applications and create a new application.

go into the OAuth2 Section, and in redirects add one with 'http://localhost:8080/login/redirect', and add two more with your own domain if you're hosting this publicly (one with http and one with https) example: http://place.drapadon.us/login/redirect and https://place.drapadon.us/login/redirect

Copy client ID, change botdata.js clientId to it

Reset secret, Copy secret, change botdata.js clientSecret to it

Go to Bot section, create a bot user, reset token and copy, change botdata.js clientToken to it.

go to OAuth2 section, scroll down to the URL generator, turn on the 'bot' checkmark, turn on administrator permissions, select integration type as 'guild install', copy URL and add the bot to your own server.

Go into Installation section, change "Install Link" to none

Now you can close this.

Make sure your user has the admin role you specified earlier in the config.json file.

now, open a terminal or command prompt window to the folder the project is saved in

finally, run `node main`
it should be hosted at http://localhost:8080/

Side note: you can also go into the code and change things from 'DigyttPlace' to your own website name, or change any other text content in the .html files if you'd like to personalise your experience.

Have fun!

Admin Commands
colors (hex code, hex code, hex code, etc)
cooldown (seconds)
expand (length, width, length, width)

r/place regular color pallette: colors 6B0119 BD0037 FF4500 FEA800 FFD435 FEF8B9 01A267 09CC76 7EEC57 02756D 009DAA 00CCBE 244FA4 3790EA 52EAF3 4839BF 695BFF 94B3FF 801D9F B449BF E4ABFD DD117E FE3781 FE99A9 6D462F 9B6926 FEB470 000000 525252 888D90 D5D6D8 FFFFFF
