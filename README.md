# Spotify_lab_golang

A simple lab that uses the [Spotify library](https://github.com/zmb3/spotify) written in **Golang**. The example implemented performs the following:
1. Generates a token required to login to the Spotify API
2. Searches through all the playlists that contain the word "Christmas" in their name.
3. Recovers all the songs for each one of the playlists until it has 40 different ones.
4. Prints out the definitive Spotify christmas playlist we can use for next year's holiday season parties.


## Prerequisites

- Golang 1.20 or higher installed
- A spotify account. You can create one [here](https://www.spotify.com/es/signup). Additionally you will need to create a **Spotify APP** and generate the *Spotify Account ID* and the *Spotify Secret*. You can see how to create all this [here](https://developer.spotify.com/documentation/web-api).
- _Recommended but not mandatory VS Code or a similar IDE_

## How to install and Run the project

First you will need to set the environment variables that correspond to the **Spotify** configuration. If you use Mac OS, you can set them like this:

```bash
export SPOTIFY_ID=XXXXXXXXXXXXX
export SPOTIFY_SECRET=XXXXXXXXXXXX
```

If you are using Windows, you can set them like this:

```bash
setx SPOTIFY_ID "Variable value"
setx SPOTIFY_SECRET "Variable value"
```

You will need to download all the external libraries using:

```bash
go mod tidy
```

Finally, navigate to the */cmd* folder and run the following command:

```bash
go run main.go
```