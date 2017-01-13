# simple-queue
##Simple job queue script

Bourne Shell implementation of a simple queue command.
This script comes in handy for hot-key triggerd scripts and the like.
It does not provide advanced features (like a timer, load based job qeueing).

By default it will execute the same job only once in a row. Use the '-d' option if
you don't like this behaviour.


## Examples

```
squeue --help

echo "wget http://example.org/largefile.bin" | squeue

squeue wget http://example.org/another_largefile.bin

cat commands.txt | squeue -d

```

Have fun!
