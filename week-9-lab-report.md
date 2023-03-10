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
./written_2/non-fiction/OUP/Berk/CH4.txt
./written_2/non-fiction/OUP/Berk/ch1.txt
./written_2/non-fiction/OUP/Berk/ch2.txt
./written_2/non-fiction/OUP/Berk/ch7.txt
./written_2/non-fiction/OUP/Castro/chA.txt
./written_2/non-fiction/OUP/Castro/chB.txt
./written_2/non-fiction/OUP/Castro/chC.txt
./written_2/non-fiction/OUP/Castro/chL.txt
./written_2/non-fiction/OUP/Castro/chM.txt
./written_2/non-fiction/OUP/Castro/chN.txt
./written_2/non-fiction/OUP/Castro/chO.txt
./written_2/non-fiction/OUP/Castro/chP.txt
./written_2/non-fiction/OUP/Castro/chQ.txt
./written_2/non-fiction/OUP/Castro/chR.txt
./written_2/non-fiction/OUP/Castro/chV.txt
./written_2/non-fiction/OUP/Castro/chW.txt
./written_2/non-fiction/OUP/Castro/chY.txt
./written_2/non-fiction/OUP/Castro/chZ.txt
./written_2/non-fiction/OUP/Fletcher/ch1.txt
./written_2/non-fiction/OUP/Fletcher/ch10.txt
./written_2/non-fiction/OUP/Fletcher/ch2.txt
./written_2/non-fiction/OUP/Fletcher/ch5.txt
./written_2/non-fiction/OUP/Fletcher/ch6.txt
./written_2/non-fiction/OUP/Fletcher/ch9.txt
./written_2/non-fiction/OUP/Kauffman/ch1.txt
./written_2/non-fiction/OUP/Kauffman/ch10.txt
./written_2/non-fiction/OUP/Kauffman/ch3.txt
./written_2/non-fiction/OUP/Kauffman/ch4.txt
./written_2/non-fiction/OUP/Kauffman/ch5.txt
./written_2/non-fiction/OUP/Kauffman/ch6.txt
./written_2/non-fiction/OUP/Kauffman/ch7.txt
./written_2/non-fiction/OUP/Kauffman/ch8.txt
./written_2/non-fiction/OUP/Kauffman/ch9.txt
./written_2/non-fiction/OUP/Rybczynski/ch1.txt
./written_2/non-fiction/OUP/Rybczynski/ch2.txt
./written_2/non-fiction/OUP/Rybczynski/ch3.txt
[...]
```
