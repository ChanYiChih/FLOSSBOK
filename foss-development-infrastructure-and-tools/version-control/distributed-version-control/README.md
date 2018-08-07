# Distributed Version Control

In the past five years or so a new breed of tools has appeared: so-called “distributed” version control systems \(DVCS for short\). The three most popular of these are Mercurial, [Git](http://www.atlassian.com/git/) and Bazaar.

These systems do not necessarily rely on a central server to store all the versions of a project’s files. Instead, every developer “clones” a copy of a repository and has the full history of the project on their own hard drive. This copy \(or “clone”\) has all of the metadata of the original.

This method may sound wasteful, but in practice, it’s not a problem. Most programming projects consist mostly of plain text files \(and maybe a few images\), and disk space is so cheap that storing many copies of a file doesn’t create a noticeable dent in a hard drive’s free space. Modern systems also compress the files to use even less space.

The action of getting new changes from a repository is usually called “pulling,” and the action of moving your own changes to a repository is usually called “pushing”. In both cases, you move change sets \(changes to file groups as coherent whole\), not single-file diffs.

One common misconception about distributed version control systems is that there cannot be a central project repository. This is simply not true – there is nothing stopping you from saying “this copy of the project is the authoritative one.” This means that instead of a central repository being required by the tools you use, it is now optional and purely a social issue.

## Advantages Over Centralized Version Control

The act of cloning an entire repository gives distributed version control tools several advantages over centralized version control systems:

* Performing actions other than pushing and pulling change sets is extremely fast because the tool only needs to access the hard drive, not a remote server.
* Committing new change sets can be done locally without anyone else seeing them. Once you have a group of change sets ready, you can push all of them at once.
* Everything but pushing and pulling can be done without an internet connection. So you can work on a plane, and you won’t be forced to commit several bug fixes as one big change set.
* Since each programmer has a full copy of the project repository, they can share changes with one or two other people at a time if they want to get some feedback before showing the changes to everyone.

## Disadvantages Compared to Centralized Version Control

To be quite honest, there are almost no disadvantages to using a distributed version control system over a centralized one. Distributed systems do not prevent you from having a single “central” repository, they just provide more options on top of that.

There are only two major inherent disadvantages to using a distributed system:

* If your project contains many large, binary files that cannot be easily compressed, the space needed to store all versions of these files can accumulate quickly.
* If your project has a very long history \(50,000 change sets or more\), downloading the entire history can take an impractical amount of time and disk space.

The authors and contributors of modern distributed version control systems are working on solving these problems, but at the moment, no bundled, built-in features solve them.



