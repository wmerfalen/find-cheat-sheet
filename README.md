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

# Excluding files based on directory prefix
Let's say we want to find all `.js` files in the current directory but we want to exclude `./node_modules/*`:
```
$ find -name "*.js" -not -path "./node_modules/*"
```
