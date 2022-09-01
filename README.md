# GeoGenre - Android Application

This project was developed as a part of the Texas A&M Howdy Hack hackathon in 2021 as a group of 3. Being barely sophomores, we focused our time mainly on just learning the software and technology, such as Git and Android Studio, and utilizing APIs, such as Google Maps and Spotify.

The main idea behind this app was to play a specific genre playlist depending on your location of the Texas A&M - College Station campus. Although we didn't finish, we managed to get proper Spotify authentication and connection that played a specified playlist and gave the user all of the normal functionalities, such as skipping, pausing, etc.

### Problems Encounted & Solutions

The primary issues we had during development involved Google Maps API being paid, and the way Spotify stores its music.

For the Google Maps API, you can only make 1000 API requests before you have to start paying, so we figured that it wasn't worth implementing if we would just have to change it later, but we couldn't find a better alternative to get the user's physical location on a map within the time that we had.

As for Spotify, we wanted to just play any song from a specific genre, but using the new and updated Spotify API at the time, we could only get an artist and then their associated genres. As a result, to do what we wanted, we would have to query and then filter all of the stored artists and then make new databases with the song ids for each genre, which was a little beyond our capabilities at the time, and we figured it would be slow. Our solution for this was to just find premade genre playlists (although not very extensive or diverse), get their identification numbers, and hard code them into our internal dictionary as to what to play.
