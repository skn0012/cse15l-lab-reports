# **Week 9 Lab Report - Skyler Nguyen**

## Redoing Researching Commands (Lab Report 3)

* This time I did the command *find*.

## 1. **find -name "filename"**

* This searches for the specific file name that the user inputs in the current directory and its subdirectories. It's useful for searching a whole directory for a single file by name.

```
find -name "Bahamas-History.txt"

./written_2/travel_guides/berlitz2/Bahamas-History.txt
```

```
find -name "ch1.txt"

./written_2/non-fiction/OUP/Abernathy/ch1.txt
./written_2/non-fiction/OUP/Berk/ch1.txt
./written_2/non-fiction/OUP/Fletcher/ch1.txt
./written_2/non-fiction/OUP/Kauffman/ch1.txt
./written_2/non-fiction/OUP/Rybczynski/ch1.txt
```

## 2. ** find -type 'type'**

* This searches for all files of the type that the user inputs. This is useful for finding all of the files of a specific type.

``` 
find -type d

.
./.git
./.git/info
./.git/hooks
./.git/branches
./.git/refs
./.git/refs/heads
./.git/refs/tags
./.git/refs/remotes
./.git/refs/remotes/origin
./.git/objects
./.git/objects/pack
./.git/objects/info
./.git/logs
./.git/logs/refs
./.git/logs/refs/remotes
./.git/logs/refs/remotes/origin
./.git/logs/refs/heads
./written_2
./written_2/non-fiction
./written_2/non-fiction/OUP
./written_2/non-fiction/OUP/Abernathy
./written_2/non-fiction/OUP/Berk
./written_2/non-fiction/OUP/Castro
./written_2/non-fiction/OUP/Fletcher
./written_2/non-fiction/OUP/Kauffman
./written_2/non-fiction/OUP/Rybczynski
./written_2/travel_guides
./written_2/travel_guides/berlitz1
./written_2/travel_guides/berlitz2
```

```
