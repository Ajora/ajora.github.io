---
layout: post
title: Basic Linux Commands
---

The following post is for my notes only. Linux man-pages covers every command in great depth.

### Find

Find command is a powerful tool that helps users search the filesystem with the option to have a variety of filters. 

Basic format:
```find [options] starting/path expression```

Simple command to find `test.text` in current and subdirectories:
```find . -name test.txt```

Look for a certain extension instead:
```find . -name *.txt```

Can search for directories also:
```find . -type d -name "directory-name"```

Can add size constraints (files greater than 1M):
```find . -size +1M```

### Touch

One of the easiest ways to create a new file but also can be used to modify timestamps on existing files and directories.

Basic format:
```touch [options] filename```

Multiple files:
```touch file1 file2 file3```

### Cat

Short for concatenate. Cat can be used to view a single file, multiple file, or create and concatenate files.

Basic format:
```cat [options] filename```

Multiple files:
```cat file1 file2 file3```

View file with numbers for each line:
```cat -n file1```

Create new file:
```cat >file1```

Append file1 to file2:
```cat file1 >> file2```

Combine file1 and file2 to make file3:
```cat file1 fil2 > file3```

### More/Less
Terminal pagers