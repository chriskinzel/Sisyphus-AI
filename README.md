# Sisyphus AI
Solves Sisyphus problem instances (assigning people to rooms based on constraints) using a genetic search algorithm. Constraints include things such as putting a smoker with a non-smoker is bad, secretaries should be close to managers, room occupancy cannot exceed room capacity, etc...

# Compilation & Running
In the project directory
    javac *.java
  
    java SisyphusI [`<env-file>` [`<time-in-ms>`]]
  
where env-file is the input file consisting of ASCII input in predicate form (i.e. person(jim)) and time-in-ms is a timeout period after which the program will print the best solution so far to the output file. -1 can be specified to indicate no timeout should occur. If no options are specified the program runs in interactive mode where predicates and commands can be performed in real time as the system is running. The program writes the output solution in the form of assign-to predicates (i.e. assign-to(jim, room1)) in an output file named by appending .out to the input file path.