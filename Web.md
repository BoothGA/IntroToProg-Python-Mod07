# Error Handling and Pickling

## Introduction
This week our assignment was to research new methods within coding; pickling and error handling. We did not receive a script to begin with and needed to present an example of these concepts at work. Pickling is a process to write data to binary which provides a way to cut down on required memory and error handling is a way to assist with code where a mistake could be foreseen and a way to find a possible issue in a code.
Pickling
Pickling is quite easy to achieve. It picks up on writing/reading to files but only this time we are using “wb” or “rb” to write or read the file contents in “binary” mode. A few new functions we will use also require a new library outside of Python. To get this library to be accessible by the code we need to import as shown in Figure 1.1.

![image](https://user-images.githubusercontent.com/125116389/222934506-aad40aec-7b4f-4419-91af-471657f6d6cb.png)

###### Figure 1.1: Importing the pickle library.




With that loaded we can now access some new functions. We’ll be using pickle.load and pickle.dump as our write/read for the binary data. Along with the “wb” and “rb” mentioned above. This is displayed below in Figure 1.2.


<img width="468" alt="image" src="https://user-images.githubusercontent.com/125116389/222934522-8edd181b-7c22-4689-b404-c4065bfede65.png">

###### Figure 1.2: Functions that are writing the data in binary and reading it back in binary.
This is very similar to our write/read functions from previous assignments and just the pickle function is the only change. 
Figure 1.3: This is our data written in binary to the file.


## Error Handling
For error handling we are using a try and except block of code. Essentially this code will run the code indented under our try function. Once run, if it succeeds nothing happens, but if an exception object occurs, we can now manipulate that object and present customizable error messages.

![image](https://user-images.githubusercontent.com/125116389/222934537-c785f946-7b6e-4a7b-b4f4-2168bd658418.png)

###### Figure 2.1: Try and except block of code we are using. This will print the custom message under the “except” function since I have purposefully added the error in to demonstrate.

As shown in Figure 2.1 the try function is attempting some code. This is going to produce an error and then fall to the except block and run whatever is scripted within. The error here is that we are trying to read a pickled file but not using the proper read method. The “r” in the open function should be “rb” for reading binary data.

![image](https://user-images.githubusercontent.com/125116389/222934545-dbb3820c-177b-4c5a-84aa-91bd0c957b78.png)

###### Figure 2.2: Our custom error message displaying at the beginning of the program.

## Summary
This assignment showed a new method of storing data within a file and catching possible mistakes that other might make when providing them our code. In Figure 3-1 it will show the code running in PyCharm and in the Terminal. Notice the terminal window we have the .txt file displayed as well to show the contents is not readable.






<img width="468" alt="image" src="https://user-images.githubusercontent.com/125116389/222934556-8b709888-783f-4fe4-bb8d-6467ee0c7e3a.png">






###### Figure 3-1: This assignment code running in PyCharm and Terminal. The .txt file displayed as well.









