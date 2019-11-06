# API Documentation

# Introduction

Project Honoka provides an accessible API (by everyone when the project will be released for public) for game data and game assets (already extracted).

For Patron Beta Testers, they will need to retreive a static dedicated token in order to rereive the data from server

# Retreive the Static Assets Token

Once you got logged in, click on **Profile icon** on the right of the app bar and then click to Profile.

You will see the two text fields: email address and API token. It's the last one which you need now. Copy it.

# Make request 

Once retreived the token, you are ready to make the requests.

Unless you are developing by yourself a library for the access to API, I suggest you some tools to test the API:

* **Insomnia** (macOS)
* **Postman** (Windows)

Make sure that you are doing a **GET** request and add an header called **X-Honoka-Assets-Token** with value the **static token** which you retreived before

Example Request (raw HTTP):

----------------------------------------------------------

GET /api/ja/unit HTTP/1.1<br>
Accept: \*/\*<br>
Cache-Control: max-age=0<br>
Accept-Language: en-gb<br>
Host: beta.api.honoka.makoo.eu<br>
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.2 Safari/605.1.15<br>
Accept-Encoding: gzip, deflate, br<br>
Connection: keep-alive<br>
X-Honoka-Assets-Token: *your token goes here token*


----------------------------------------------------------

# List of available entrypoints

This list of entrypoints will be updated in the future builds

* /api/ja/unit
* /api/ja/unit/*unitId* (change this with internal unit ID)
* /api/ja/still
* /api/ja/still/*stillId* (change this with internal still ID)
* /api/ja/live
* /api/ja/live/*liveId* (change this with internal live ID)
* /assets/*path* (change with the path of the desired assets)