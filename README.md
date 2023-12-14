# IVS Chat Web Demo Frontend

A demo web application to demonstrate how you can build a simple live video and chat application with [Amazon IVS](https://aws.amazon.com/ivs/).

## Prerequisites

* [NodeJS](https://nodejs.org/)
* Npm is installed with Node.js

## Configuration

The following entries in `src/config.js` (inside the web-ui project directory) are used to configure the live video player and the chat websocket address.

Values that you do not need to change: 

* `PLAYBACK_URL`
  * Amazon IVS live video stream to play inside the video player
* `CHAT_REGION`
  * The AWS region of the chat room. In this case, `us-east-1`.

Values you need to change:
(The Live Shopping team will provide you with this information when you start the challenge).

* `API_URL`
  * Endpoint for the Amazon IVS Chat Demo backend
* `CHAT_ROOM_ID` (It is unique per team)
  * The ID (or ARN) of the Amazon IVS Chat Room that the app should use.

## Running the demo

After you are done configuring the app, follow these instructions to run the demo:

1. [Install NodeJS](https://nodejs.org/). Download latest LTS version ("Recommended for Most Users")
2. In root directory on your local computer
3. Run: npm install
4. Run: npm start

(When executing the project, 13 warnings will appear, please ignore these warnings).

To send a message you must enter after writing it.
To intercept the message, the code for this functionality is found in the `sendMessage()` function in file `src\components\chat\Chat.jsx`:

## Limitations

* Message and user data for this demo is not saved/persistent (ie. reloading the page would go back to initial state).

--------------------------------------------------

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.