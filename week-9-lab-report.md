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


## 2. **find -type 'type'**

* This searches for all files of the type that the user inputs such as files, directories, sockets, etc. This is useful for finding all of the files of a specific type.

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
find -type f
./.git/info/exclude
./.git/hooks/commit-msg.sample
./.git/hooks/prepare-commit-msg.sample
./.git/hooks/update.sample
./.git/hooks/pre-rebase.sample
./.git/hooks/pre-merge-commit.sample
./.git/hooks/push-to-checkout.sample
./.git/hooks/pre-push.sample
./.git/hooks/pre-commit.sample
./.git/hooks/post-update.sample
./.git/hooks/pre-receive.sample
./.git/hooks/applypatch-msg.sample
./.git/hooks/fsmonitor-watchman.sample
./.git/hooks/pre-applypatch.sample
./.git/description
./.git/refs/heads/main
./.git/refs/remotes/origin/HEAD
./.git/objects/pack/pack-b98cb6a4ca64cc7b2944f0fa07d3e03927d66064.pack
./.git/objects/pack/pack-b98cb6a4ca64cc7b2944f0fa07d3e03927d66064.idx
./.git/HEAD
./.git/config
./.git/logs/refs/remotes/origin/HEAD
./.git/logs/refs/heads/main
./.git/logs/HEAD
./.git/packed-refs
./.git/index
./written_2/non-fiction/OUP/Abernathy/ch1.txt
./written_2/non-fiction/OUP/Abernathy/ch14.txt
./written_2/non-fiction/OUP/Abernathy/ch15.txt
./written_2/non-fiction/OUP/Abernathy/ch2.txt
./written_2/non-fiction/OUP/Abernathy/ch3.txt
./written_2/non-fiction/OUP/Abernathy/ch6.txt
./written_2/non-fiction/OUP/Abernathy/ch7.txt
./written_2/non-fiction/OUP/Abernathy/ch8.txt
./written_2/non-fiction/OUP/Abernathy/ch9.txt
[...]
```
* There are a lot more files not included, hence the [...].


## 3. **find -name "filename" -exec rm -f {} \;**

* This commands removes the specific file that the user inputs. This is useful for removing an unneeded file.

```
find -name "Vallarta-WhereToGo.txt" -exec rm -f {} \;

find -name "Vallarta-WhereToGo.txt"

```
- Since the "Vallarta-WhereToGo.txt" file was removed, the terminal doesn't print out anything.

```
find -name "Vallarta-WhatToDo.txt" -exec rm -f {} \;

find -name "Vallarta-WhatToDo.txt"

```


## 4. **find 'directory' -user 'username'**

* This command finds all of the files in the directory and it's subdirectores that belong to the inputted user. This is useful for seeing which files were created by which user.

```
find ./written_2 -user cs15lwi23aiz               
./written_2
./written_2/non-fiction
./written_2/non-fiction/OUP
./written_2/non-fiction/OUP/Abernathy
./written_2/non-fiction/OUP/Abernathy/ch1.txt
./written_2/non-fiction/OUP/Abernathy/ch14.txt
./written_2/non-fiction/OUP/Abernathy/ch15.txt
./written_2/non-fiction/OUP/Abernathy/ch2.txt
./written_2/non-fiction/OUP/Abernathy/ch3.txt
./written_2/non-fiction/OUP/Abernathy/ch6.txt
./written_2/non-fiction/OUP/Abernathy/ch7.txt
./written_2/non-fiction/OUP/Abernathy/ch8.txt
./written_2/non-fiction/OUP/Abernathy/ch9.txt
[...]
```

```
find ./written_2 -user jpolitz
find: 'jpolitz' is not the name of a known user
```
* Since the files in this directory were cloned by me, there are no other users.


## Finding the Source

* I searched up 'how to use the command find in linux'.
* I used two websites. Here are the links:
    * [Link 1](https://www.redhat.com/sysadmin/linux-find-command)
    * [Link 2](https://www.tecmint.com/35-practical-examples-of-linux-find-command/)
