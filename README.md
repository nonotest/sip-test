# React Native test

Email a zip with buildable app (android + ios) at tech@stocksinplay.com

Please use the latest available react-native version (61.1 at time of writing)

Using the nasa api (https://api.nasa.gov/) , generate a key

## App organisation

We want a tab stack with 2 screen;
- list of photos from mars
- favourite photos

### List of photos

Level 1)

Using flatlist query Mars Rover Photo api ( https://api.nasa.gov/mars-photos/api/v1/rovers/curiosity/photos?sol=1000&api_key=DEMO_KEY )

Display a infinite list with pagination(load the next items when reaching the bottom of the list) of photos.
Each list item must show:
 * name of photo
 * thumbmail 
 * camera details
 * date of photo
 

Level 2)

Add a "star" icon with an onPress event that will store in local storage "favourite" photos
Add ability to "un favourite" if clicking on an item that has already been added to favourites

### List of favourite photos

Using a flatlist display the current favourite photos of the user.
Tip: re-use the previous list item component
