This is an spring 5 application JDK 11 is being used. 
Maven is needed in order to compile it

There is a game.properties file in the path config/game.properties 
in that file there is a game.maxNumber property, it has 5 by default, the value can be changed for a any Integer number.
this property defines the amount of people that will be taken as the total group of people where just one is the celebrity.

The celebrity is choosen randomly, and obviosly it is represented with a number between 0 and the maxNumber - 1, then the data 
is printed on the console from 1 to maxNumber
A matrix is generated in order to specify if a person knows another person. If that is the case a 1 is written in the matrix, 
if thats not the case a 0 is written. In order to simplify a person is not known by him/herself so a 0 is assigned.

One stack is used to push all people, then a function is used to recognize if the matix has 1 o 0 as input for all people 
against a particular person, if so, that could be a celebrity and it shoulbe pushed onto the stack, if it is not known then it
will be poped from the stack. The process continues till there is just on element, the celbrity index

HOW TO SEE THE RESULTS:

Run the CelebrityProject project, the celebrity will be generated randomly
The matrix is printed on the console
The algorithm will search the celebrity
If the celebrity is found then a message will confirm the result with the ID that belongs to that person, also the value of 
that ID prior to the process is printed just for purpouse of checking the result.



