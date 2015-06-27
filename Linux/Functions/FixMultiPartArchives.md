# Fix Multi Part Archives

Sometimes people upload archive files in multiple parts, in order to unarchive these then, you can use this to quickly fix them.

## Usage

Type these commands into the terminal

```
$ cat FILE.zip.* > FILE.zip
$ zip -F FILE.zip --out FILE-fix.zip
$ unzip FILE-fix.zip
``

## Notes

