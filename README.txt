This is a homework demonstrating the proper use of shared data structures between multiple child processes occuring from the same "parent" process with the help of semaphore mutexes. Each entity (i.e. the doorman, the waiter, each customer etc) is represented as a process and depending on their status (active/sleeping) they are executing different tasks having always as a goal to be synchronized and concurrent as well as to avoid race conditions and deadlocks.

Readme

Thanasis Filippidis sdi1400215@di.uoa.gr

## Compile

To compile run `make`

## Run

Command line options:
 * -n number of groups to come
 * -l name of configuration file (conf.txt)
 * -d time after which statistics will be printed

Invocation:

    ./restaurant -n customers -l configfile -d time
    
    in all possible combinations 


## Implementation Notes


### Restaurant

For the restaurant implementation, I followed as much as possible the instruction given.
The only things done in a different way because of lack of time are the following:
-No log file available, prints are done in terminal
-The groups in bar, when their turn comes to sit, the discuss and decide if they are bored of waiting
and they are going to leave or if they are going to sit on the table that waits for them
-The statistics are printed after all the groups have been served

### Waiter

For the waiter implementation, one more flag is added, the flag "-p" to give a seperate id to each waiter
