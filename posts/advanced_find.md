This one-liner will move all files that meet a case-insensitive regular expression to the desired location and only update it if newer than the destination (via cp's -u)

`find . -regextype 'posix-extended' -iregex ".*\.(jpg|jpeg|png)" -exec cp -u -v -t ~/path/to/dest {} +`

