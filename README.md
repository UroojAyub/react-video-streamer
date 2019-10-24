# react-video-streamer

A simple React CRUD application that fetches stream data and allows users to view live streams.

![Dashboard](https://raw.githubusercontent.com/UroojAyub/react-video-streamer/master/screenshot-1.png)
![Dashboard](https://raw.githubusercontent.com/UroojAyub/react-video-streamer/master/screenshot-2.png)
  It includes the following features:
- OAuth2 authentication
- Create Streams
- Edit and Delete Streams associated with your Google Account
- View anyone's live stream. Uses flv.js for video player
- Use of Redux store, Redux Thunk and Redux Forms 
- Axios for making REST API requests
- Uses React Portals to show modals
- RTMP Node media server and OBS (Open Broadcaster Software) used to connect live stream

## Getting Started

### Prerequisites

- Gmail account
- Node.js installed
- OBS installed

### Installing

  

  

1. Clone or download this repository

2. Run the following command in each of the client, rtmpserver and api folders

```
npm install
```

3. Navigate to the Google Cloud Console and setup a new project. Under that project create new OAuth2 credentials and whitelist the domain http://localhost:3000.
5. Copy the created Client Id and paste it into`client/.env` infront of the variable
    

`REACT_APP_OAUTH_CLIENT_ID=insert your oauth2 client id here`


4. Now run the following command in each of the client, rtmpserver and api folders

```
npm start
```

5. This will launch the development server and the app will be served on http://localhost:3000
6. Login and create a new stream. Note the ID of the stream created in the route when you click on the stream to view it.
7. Configure the OBS to stream on the server `rtmp://localhost/live` and use stream key same as the ID of the created stream in the application. Then click on start streaming in the OBS and open the stream with the same ID in the react app to view it.
  

## Built With

* ReactJS
* JSON Server
* Node Media Server

  

## Authors

*  **Urooj Ayub**- uroojayub17@gmail.com
-[(Github)](https://github.com/UroojAyub)

## License


This project is licensed under the GNU GENERAL PUBLIC LICENSE Version 3 - see the [LICENSE](https://github.com/UroojAyub/react-video-streamer/blob/master/LICENSE) file for details