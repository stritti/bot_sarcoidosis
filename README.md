# bot_sarcoidosis
Twitter Bot to retweet messages about [sarcoidosis](https://en.wikipedia.org/wiki/Sarcoidosis).

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/J3J33A8DT)

## Source

This is a fork of https://github.com/neojato/T-Hawk Many thanks for the contribution.

## Getting Started

* Log in and create a [Twitter app](https://apps.twitter.com/)
  * **NOTE:** Use the account you wish to like & retweet with (which most likely isn't your personal account)
  * **NOTE:** You do not need a Callback URL for this app
* Start a new Google Apps Script project by clicking on ["Start Scripting"](https://www.google.com/script/start/)
* Copy the code from [code.gs](https://github.com/neojato/T-Hawk/blob/master/code.gs) into the new file created for you
* Enter the appropriate Twitter keys you received from your new Twitter app in lines 3-6
* Enter your hashtag on line 7 (include "-RT" to exclude retweets from being liked and retweeted)
  * example: "#DevFest -RT"
* From the Apps Script menu, choose "Resources" and then "Libraries"
  * In the "Add a library" field, enter the following project key to load the Twitter library:
    * `11dB74uW9VLpgvy1Ax3eBZ8J7as0ZrGtx4BPw7RKK-JQXyAJHBx98pY-7`
  * Click the "Add" button
  * Change the "Identifier" field to `Twitter`
  * Change the "Version" to `23` (or the most recent)
  * Click "Save"
* Create a trigger to continually monitor the hashtag
  * From the Apps Script menu, choose "Edit" and then "Current project's triggers"
  * Follow instructions to add a new trigger
  * Setup your trigger to match the following settings:
    * hashtag_twitterBot
    * Time-driven
    * Hour timer
    * Every hour
* Enjoy!


### License

Project is published under the [MIT license](LICENSE).
