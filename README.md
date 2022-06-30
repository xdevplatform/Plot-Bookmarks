# Plot Bookmarks
I don’t Bookmark Tweets very often, and I was wondering how constantly I use the Bookmark functionality on Twitter. To figure out exactly how often I bookmark Tweets,

I built a [demo application](https://plot-bookmarks.onrender.com/) in Python using [Flask](https://flask.palletsprojects.com/en/2.1.x/). This sample code will build an application that will authorize your account using the [OAuth 2.0 Authorization Code Flow with PKCE](https://developer.twitter.com/en/docs/authentication/oauth-2-0/authorization-code) and plot up to your last 100 Bookmarked Tweets.

## Getting set up with the Twitter API

If you don’t already have access to the Twitter API, [you can sign up for a developer account.](http://t.co/signup) Once you have an approved developer account, you must create a Project in the [developer portal](https://developer.twitter.com/en/portal/dashboard). Each Project contains an [App](https://developer.twitter.com/en/docs/basics/apps/overview) with which you can generate the credentials required to use the Twitter API. You will also need to have OAuth 2.0 turned on in your App’s settings. In our [platform overview](https://developer.twitter.com/en/docs/platform-overview), you can learn more about getting started with the Twitter API.

## Setting up your environment

To install all the packages in your requirements.txt file, in your terminal, run the following command:

```bash
pip install -r requirements.txt
```

You will also set up environment variables to ensure you aren’t passing in your secrets directory. To achieve this, you will define environment variables. In your terminal, run the following command:

```bash
export CLIENT_ID=’xxxxxxxxxxxxxx’
export CLIENT_SECRET=’xxxxxxxxxxx’
export REDIRECT_URI=’http://127.0.0.1:5000/oauth/callback’
```

You can obtain your own OAuth 2.0 Client ID and Secret inside of your App’s settings in the developer portal. Use your Client ID and Secret instead of the `xxxxxxxxxxxxxx`.

### Run the file
To run the file, run the following line in your terminal:

```bash
python app.py
```
