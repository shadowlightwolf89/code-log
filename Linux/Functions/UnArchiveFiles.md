# Unarchiving

If you've downloaded an archive, and want to extract the files within using terminal, this is how.

## Usage

.tar

```
$ tar xvf filename.tar
```

.tar.gz

```
$ tar xzvf filename.tar.gz
```

.tgz

```
$ tar xvzf filename.tgz
```

.tar.gz2

You probably mean .tar.bz2
.tar.bz

```
$ tar xjvf filename.tar.bz
```

.tbz

```
$ tar xjvf filename.tbz
```

.tar.bz2

```
$ tar xjvf filename.tar.bz2
```

.tar.Z

```
$ zcat file.tar.Z | tar xvf -
```

.tar.xz

```
$ lzcat filename.tar.xz | tar xvf -
```

.gz

```
$ gunzip filename.gz
```

.gz2

You probably mean .bz2
.bz

```
$ bunzip filename.bz
```

.bz2

```
$ bunzip2 filename.bz2
```

.Z

```
$ uncompress filename.Z
```

.xz

```
$ unlzma filename.xz
```

.zip

```
$ unzip filename.zip
```

.7z

```
$ 7z x filename.7z
```

.rar

```
$ unrar x filename.rar
```

.dmg

This isn’t a file that can be ‘extracted’ but you can mount and save the files using:

```
$ mkdir /mnt/source
$ mount -o loop -t hfs filename.dmg /mnt/source
$ cp /mnt/source/* /home/username/destination/
```

.img, .dd

These aren’t files that can be ‘extracted’ but you can mount and save the files using:

```
$ mkdir /mnt/source
$ mount -o loop -t iso9660 filename.img /mnt/source
$ cp /mnt/source/* /home/username/destination/
```

## Notes

Do note, that in order to use any of these commands, you must have the associated app installed.

```
$ sudo apt-get install unace p7zip-rar sharutils rar arj lunzip lzip
```

If you have multiple archives to extract, you could use a for statement:

```
$ for t in *.FILETYPE ; do FILETYPEEXTRACTION $t ; done
```

where the term FILETYPEEXTRACTION is the command for that archive as given above.
