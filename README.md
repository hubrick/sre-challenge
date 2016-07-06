# Hubrick Site Reliability Engineer Challenge

Your objective is to create a small UDP server that listens to port, parses the
received messages and prints the timestamp and the message body in `JSON` to the
`stdout`. Your messages should arrive in the following format
`[DD/MM/YYYY HH:MM] MESSAGE BODY` and your output should have the structure
`{ "timestamp": EPOCH, "message": "MESSAGE BODY" }`. For example:
```
$ echo -n '[17/06/2016 12:30] Time to move' | nc -u localhost 1234
# Server Output:
{"timestamp":1466166600,"message":"Time to move"}
```

You can use the tools and programming language of your preference. Please give
emphasis to code readability, error handling and test coverage.

## Deliverables

You should provide us with your solution either as an archive or a public git
repository. Make sure that there is a README on how to install and run the
application.

### Bonus points

* Provide a Dockerfile for building and running an image of your solution
