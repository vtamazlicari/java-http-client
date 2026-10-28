# Java Client
Building an HTTP client.

Client-server communication uses Apache HttpClient.
The `HTTPMethods` class implements the HTTP methods GET, POST, PUT, PATCH and DELETE.
Requests are sent to [httpbin.org](http://httpbin.org) and the response is printed to the console.
`Main` provides a console menu built with a switch statement.

## Structure
- `src/Main/Main.java` – console menu
- `src/Main/Keyin.java` – keyboard input
- `src/methods/HTTPMethods.java` – HTTP methods
- `lib/` – libraries used (`httpclient`, `httpcore`, `commons-io`, `commons-logging`)

## Build and run
Linux / macOS:
```sh
javac -d bin -sourcepath src -cp "lib/*" src/Main/Main.java
java -cp "bin:lib/*" Main.Main
```

Windows:
```bat
javac -d bin -sourcepath src -cp "lib/*" src/Main/Main.java
java -cp "bin;lib/*" Main.Main
```

## Menu
```
1. Get
2. Post
3. Put
4. Patch
5. Delete
0. Exit
```
