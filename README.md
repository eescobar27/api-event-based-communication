# API with Event-Based Communication

	The API uses socket.io to provide event-based communications. The intended purpose of the API is to work with 
	other backend services as part of a microservice architecture.

	The API listens on port: 9000 by default and after the servers starts the clients can connect using the same port 
	and the socket.io-client. the server supports multiple connections and each connection will remain open until one of
	the following conditions are met:

		+ client close connection (disconnect)
		+ server close connection with the client (disconnect)
		+ server shutdown (close all connections)

	Event-Based Communication is useful when the applications need to interact with each other while keeping the connection
	open. It could also be used when the operations that need to be performed could take a while.

## Requirements

	nodeJS v8.5+
	npm 5.3+

## Setup

	npm install

## Run (development)

	the following command will set the ENV variables based on the vars.env file

	npm run start-dev

## Run

	npm run start
	