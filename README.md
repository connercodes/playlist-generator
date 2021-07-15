# playlist-generator
Technologies
 * Youtube Data API v3
 * Spotify Web API
 * Requests Library v 2.22.0
 * Youtube_dl v 2020.01.24

LocalSetup
1. Install All Dependencies
    pip3 install -r requirements.txt

2. Collect You Spotify User ID and Oauth Token From Spotfiy and add it to secrets.py file

    -To Collect your User ID, Log into Spotify then go here: Account Overview and its your Username
    -To Collect your Oauth Token, Visit this url here: Get Oauth and click the Get Token button
3. Enable Oauth For Youtube and download the client_secrets.json
4. Run the File
    python3 create_playlist.py

      - you'll see Please visit this URL to authorize this application: <some long url>
      - click on it and log into your Google Account to collect the authorization code
  
Troubleshooting
  Spotify Oauth token expires very quickly, If you come across a KeyError this could be caused by an expired token. So just refer back to step 3 in   local setup, and generate a new token!
