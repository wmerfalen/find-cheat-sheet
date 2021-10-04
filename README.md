# find-cheat-sheet
A cheat sheet for the find command.

# Finding files
```
$ find -type f
```

# Finding directories
```
$ find -type d
```

# Running a command for every matched file
Let's say we want to run `wc -l` on each file...
```
$ find -type f -exec wc -l {} +
```

# Files accessed 20 minutes ago
```
$ find -type f -amin 20
```

# Files modified 20 minutes ago
```
$ find -type f -mmin 20
```

# Files owned by user 'jack'
```
$ find -type f -user jack
```
