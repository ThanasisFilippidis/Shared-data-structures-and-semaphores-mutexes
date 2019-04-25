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
