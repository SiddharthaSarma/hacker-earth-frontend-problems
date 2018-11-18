Wonders of the world!

[Problem Statement]

Write a pseudo frontend app which presents information about the wonders of the world.

There are 2 aspects to the challenge. UI and scripting part. In this scenario, the content on the UI is not static and is dependent on the API call at any given point of time.

 

[Tasks]

UI statement points:

 

    Mockups are provided for desktop and mobile.

    The design has to be pixel perfect, cross browser compatible and responsive on all devices - mobile and desktop.

    The hamburger menu on right top corner is just an image, and does not involve any interaction.

    The static assets on the page are provided.

    The content for the body section of the page which contains the card structure, has to be retrieved from the API call (API endpoint details are mentioned under scripting problem statement).

    The description of each structure is shown on the image, on hover for desktop and on touch on mobile. (Please refer the mockups)

    On description overlay, a heart shaped icon is present on top right corner which acts as a like button functionality along with a track of the likes (Details provided under interactions)

    If any of the key values are empty, handle accordingly on the UI.

 

Scripting statement points:

 

    The content on the page has to be retrieved from an API call.

    Implement ‘Search by name’ functionality (Refer the mockup)

    If the search parameter is incorrect, display the appropriate message on UI.

    The user should be able to sort the items on the page based on ‘Ratings’ and ‘Likes’ of the places.

    Implement an interceptor loader during the API call (asset provided).

    Implement the number of API hits by the user and display accordingly on the page (Refer mockup)

 

Interactions:

 

    The heart shaped icon on the description overlay acts as a like feature on facebook.

    Once the user clicks on it, the counter beside it should increment/decrement and the icons’ color should change to green/grey respectively. This should be a toggle feature.

    On toggling of the like feature, the tracker for likes on top should change dynamically.

    The number of likes on the page should remain same even on page refresh and should not be dependent on the API response.


 

[Guide]

Wonders API: http://www.mocky.io/v2/5bdd28dd32000075008c6227

 

Technology Stack:

-- HTML, CSS, JQuery, VueJS.


 

[Mockup Reference]

 

Mobile

http://hck.re/oUc8zK

 

Web/Desktop

http://hck.re/qZiKQ8
