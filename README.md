# CarsBot : Cars24 Hackathon code 

This is submission code for CARS24 Hackathon. This is a sample chatbot, consisting of Google Dialogflow agent, a NodeJS Server and web interface, which can help users in buying and selling of cars. If the bot is not successfull in answering the user request it forwards the request to a human agent.

This is code is forked and developed on top of [Google dialogflow Sample App.](https://github.com/dialogflow/agent-human-handoff-nodejs)


### Features
* Agent will escalate to a human operator on-demand
* Agent will escalate to a human operator after repeated failure to match an intent
* Server routes conversation between agent and human operator depending on context
* Server supports multiple concurrent conversations between customer, agent and operator
* Customer web client supports real-time chat with agent or operator
* Operator web client supports real-time observation and participation in multiple customer conversations
* Operator web client demonstrates alerting of operator in case of customer escalation

### Limitations
* **There is no authentication of customers or operators. In this limited demonstration, communication
between users is not secure. This code is provided as an example, not a finished solution.**
* Active conversations are stored in-memory with no on-disk persistence (though code could
easily be modified to support this).
* Operators can only monitor and communicate with customers that have subsequently connected. Previously
connected customers are ignored.
* User interface is very rudimentary. 

### Technology Stack
* [Dialogflow](https://dialogflow.com/)
* [Node.js](https://nodejs.org/en/) v6.9.1+
* [Express.js](https://expressjs.com/)
* [Socket.IO](https://socket.io/)
* [JQuery](https://jquery.com/)

### Future Implementation
* Adding a appointment intent so that the user can book appointment with the dealer
* Improve the UI.

## License
See LICENSE.md.
