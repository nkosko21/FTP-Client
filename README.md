Main.py uses the command design pattern to implement many functions into the FTP client.

In the main() method, arguments from the command line are parsed through parse_args(), where a method is called in relation to the argument that was inputted. 

"QUIT" calls quit(), which asks the server to close the data connection and quits the FTP client.

"STRU" calls stru(), which sets the connection to file oriented mode.

"MODE" calls mode(), which sets the connection to stream mode

"TYPE" calls type(), which sets the connection to 8-bit bindary data mode.

"PASS" calls passw(), which logs into the FTP client with the given password.

"USER" calls user(), which logs into the FTP client with the given username.

"MKD" calls mkd(), which created a directory at the given path.

"RMD" calls rmd(), which removes a directory at the given path.

"PASV" calls pasv(), which puts the FTP server in passive mode and opens a data channel.

"LIST" calls list(), which prints a list of all the contents of a given directory in the FTP server.

"STOR" calls stor(), which uploads a new file with a given name to the given path to the FTP server.

"RETR" calls retr(), which downloads a file with the given name and path in the FTP server.

"DELE" calls dele(), which deletes a file with the given name and path in the FTP server.

The main challenge with this assignment was figuring out how to parse arguments and how data channels worked. Other than that, the assignment was mostly logic based, trying to figure out how the FTP server worked. 

I tested my code by running all the commands and making sure the messages recieved in the command line were correct, as well as using fileZilla to make sure data created, removed, and listed was correct when commands were called from the client.
