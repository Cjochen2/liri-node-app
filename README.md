# liri-node-app

Welcome to LIRI!

Liri is a node based application designed to search utilizing axios for concerts, songs, and movies from varying API's such as OMDB, BandsInTown, and Spotify. Below is a demonstration of how each feature works. To go more in depth select the liri.js file to get started.

Prior to using LIRI you will need to install the following npm packages and provide your own .env file with Spotify Keys

   * [Node-Spotify-API](https://www.npmjs.com/package/node-spotify-api)

   * [Axios](https://www.npmjs.com/package/axios)

   * [Moment](https://www.npmjs.com/package/moment)

   * [DotEnv](https://www.npmjs.com/package/dotenv)

## Movie This:

![Movie This](/images/Movie-This.JPG)

In the above image you will see the first instance of movie this is run with out a specified movie and an error in syntax due to an incorrect command input. Liri the spits out an example of how the syntax should be laid out. It is set to default to 'Mr.Nobody' if the command input is correct but there is no movie specified.

After that it is demonstrated again with 'The Dark Knight' as the specified input for the command. Liri takes each of the words and runs them through the OMBD API. It then processes the response and pulls out the relevent information such as Title, Rating, Release Year, ect.

## Concert This:

![Concert This](/images/Concert-This.JPG)

In this image you will see the use of the concert command. Much like 'movie-this' if there is any error in syntax it will put out the correct format and command keys. It also will default to Maroon 5 if no artist is given.

When correctly used it will display the artists name along wiht upcoming events and their locations.

## Spotify This Song:

![Spotify This Song](/images/Spotify-This.JPG)

This command will work the same as above only this time it will search for a particular song. Again if there is an error it will display proper syntax or no song it will default to 'The Sign'.

Spotify This returns information on the artist album song and if available a sample URL.

## Do What It Says:

![Do What](/images/Do-What-It-Says.jpg)

This command takes input from the random.txt file and runs it through the above scenarios dependning on the command and search query. In the image above I changed the random.txt file in between the two instances in which I ran do what it says. The first instance random.txt read 'spotify-this-song,"I Want It That Way"' the second read 'movie-this,"The Return of the King"'. This command reads and breaks up the txt file and then inputs it into the formula to run and generate results like the one's above.

## Thoughts and Summary:

This was an introduction into using Node and JS from the command line. My biggest take away from it was a strong understanding of writing modular code and how to use switch cases. Prior to this exercise understanding functions and how to effectively use them was eluding me. This helped shed some light as it all finally clicked and made sense. The biggest hold up was understanding the difference in a paramater when creating the function vs an argument when calling the function. As demonstrated I call the functions using different inputs in the 2 different switch case statements yet they accomplish the same thing. Other than the functions the only other challenge was sorting through the Spotify API as the JSON response was generally massive and took some workarounds and detective work to understand. Un-comment the console log inside the song function and see what I mean.... Overall I this is a good project for gaining exposure to node and expanding my understanding of JS. Please feel free to reach out with any questions!