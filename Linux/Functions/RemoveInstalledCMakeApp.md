# Remove an Installed CMake Application

If you've installed an application through cmake, and now want to uninstall it, this is how you do so.

## Usage

type this into a terminal that is CDed into the build folder of your cmake app.

```
$ xargs rm < install_manifest.txt
```

## Notes

