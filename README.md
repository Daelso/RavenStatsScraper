
# RavenStats

Yet another goofy project for the SS13 server Lifeweb. This node.js project scans the Lifeweb discord for showlad entries and files, it then parses them down into usable data to generate a rough estimate of the amount of times a role has been played as well as providing user statistics. The final output will be a csv that is an amalgamation of both user posts and scraped text files containing much of the same data. The csv will be formatted for SQL or excel importing, so feel free to use whatever you like.

It is very likely that I will personally use this data for some APIs or to populate a DB, what you do with it is up to you.


##Thank You!

This project would not be possible without the DiscordChatExporter (It is seriously stupid hard to automate scraping discord channels, bless this dudes work) - https://github.com/Tyrrrz/DiscordChatExporter


## Disclaimer
Player data is collected via the Showlads commanda at the end of the round and the formatting and provision of it is spotty at best. Data collected is likely of horrific integrity and contains duplicates as well does not include pre-discord games nor games that no one bothered to post.


## Installation

You will need node, npm and dotnet to run this program. A discord account with access to the Lifeweb Hideout is also required.

Clone down the repo locally and within your RavenStats folder create a file titled .env, this is where you will put your sensitive data.

ENV Format:
```env
DISCORD_TOKEN = yourtokenhere
FILE_DIR = "C:/Users/yournamehere/OneDrive/Desktop/coding projects/RavenStats/showlads_dump"
```

To get your discord token, please view the instructions for the DiscordChatExporter here:
https://github.com/Tyrrrz/DiscordChatExporter/blob/master/.docs/Token-and-IDs.md#how-to-get-user-token

File_dir refers to where you would like to export your contents to.

```bash
  npm install
```
We use several dependencies so please install them before attempting to run the program.
    
## License

[GNU](https://choosealicense.com/licenses/gpl-3.0/)
