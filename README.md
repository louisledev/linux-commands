# Linux Commands
This repo aims to list the set of Linux commands that helped me in my work life.

## curl
Transfer data from or to a server.

See [Man Page](https://linux.die.net/man/1/curl)

## cut
Remove sections from each line of files.

See [Man Page](http://man7.org/linux/man-pages/man1/cut.1.html)

### Examples
Display the first field in a line with `,` as delimiter:
```bash
cut -d ',' -f 1 names.csv
```

## find
Search for files in a directory hierarchy.

See [Man Page](http://man7.org/linux/man-pages/man1/find.1.html), [Tutorial](https://www.lifewire.com/uses-of-linux-command-find-2201100)


### Examples
#### Remove large file from a folder
```bash
find . -size +2M -exec rm {} \;
```

## locate
Identify location(s) of a file. 

Note that it relies on a database for this search, which can be updated with 
`sudo updatedb`.


See [Man Page](http://man7.org/linux/man-pages/man1/locate.1.html), [Tutorial](https://www.howtoforge.com/linux-locate-command/)


## lsof
List on its standard output file information about files opened by processes. 

An open file may be a regular file, a directory, a block special file, a character special file, an executing text reference, a library, a stream or a network file (Internet socket, NFS file or UNIX domain socket.) A specific file or all the files in a file system may be selected by path.

See [Man Page](https://linux.die.net/man/8/lsof), [Tutorial](https://www.howtoforge.com/linux-lsof-command/)

### Examples
Show all processes using port 2377:
```bash
sudo lsof  -i :2377
```

## nc
Read and write data across network connectiosn, using TCP or UDP protocol.

See [Man Page](https://www.commandlinux.com/man-page/man1/nc.1.html)

## pidof
Find the process ID of a running program.


## sed
Filter and transform input text.
See [Man Page](https://linux.die.net/man/1/sed)

## tail
Read a file and outputs the last part of it.

See [Man Page](http://man7.org/linux/man-pages/man1/tail.1.html),[tutorial](https://www.computerhope.com/unix/utail.htm)



