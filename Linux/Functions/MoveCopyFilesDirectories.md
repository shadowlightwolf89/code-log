# Move or Copy Files and or Directories

Need to move or copy files and or directories to another location? Here's how.

## Usage

To move all subdirectories of Dir1 to Dir2 use the mv command, to copy them use the cp command.

```
$ [ mv | cp ] -r ~/Dir1/* ~/Dir2
```

To move a single directory called Dir1 into the directory Dir2  use the mv command, to copy them use the cp command.

```
$ [ mv | cp ] -r ~/Dir1/ ~/Dir2
```

To copy files instead of directories, simply omit the -r

## Notes

