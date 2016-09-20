# Protocols
What messages Client and Server user to communicate with over sockets

Both Client and Server will *link* to this package.

So for example lets say we have the directories:
```
Mode                LastWriteTime     Length Name
----                -------------     ------ ----
d----         9/19/2016   9:58 PM            Client
d----         9/19/2016   9:21 PM            Protocols
d----         9/19/2016  10:02 PM            Server
```

To link Protocols to both client and server you would do something like this:
```
$ cd Protocols
$ npm link
$ cd ..\Server
$ npm link juke-protocols
$ cd ..\Client
$ npm link juke-protocols
```

Afterwords Client should be able to build and Server should be able to start up!
