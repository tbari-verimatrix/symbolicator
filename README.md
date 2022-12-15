# Crashlog symbolicator

This is a command line tool to resolve/symbolicate iOS crashlogs. The tool uses Spotlight search (`mdfind`) to locate the corresponding dSYM files.

## Requirements
* Ruby (developed and tested with 2.6.10)
* `Open3` gem
* `colorize` gem
* Xcode installation (`dwarfdump`, `dsymutil`, `atos`, `mdfind`)

## Usage
To use the tool you'll need the following on your machine:
* a text file containing the crashlog
* the Xcarchive of the application

For the arguments needed please see the help of the script:
```Shell
symbolicator --help
```
