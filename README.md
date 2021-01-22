# ExpressJsonDatabase
Server software developed to provide online functionallity to the app [Debtify](https://github.com/OlofSjogren/GoAyo).

## Purpose
As me and my project group started working on Debtify, our original idea was to create a protype with a "mock database". I however, had an old laptop laying around and an intrest in JavaSript and thought it would be cool to have an actual server hooked up with the application.

The project is pretty small, yet it provides complete online capabilities to Debtify and would write tens of thousands of entries during it's hour long testing sessions. Hopefully others can take inspiration from this project, as the technique is easy to setup.

## Modules/Frameworks

- Node
- Express
- Joi

## How it works.

Now this part is simple. The server gets a port, as most servers do. In the Server folder, there's a file called database.json. When someone makes a HTTP-POST request to the server, it simply loads the json file, and adds the new data. It then rewrites the json file. And if the request is HTTP-GET, it sends the required data back. It couldn't get any simpler. Joi is used to make sure that the format of the POST requests are correct.
