# CODEQUOTER


codequoter is a command line utility made to produce file-path referenced line numbered automatically typed code quotes for markdown documents referencing code under version control in a git repository

it is meant to be the brains behind helpful plugins for vim and other editors 

## env vars

- ``NONUM``  - set to not print hard coded line numbers

usage ``codequoter <file> line1 line2``

example output ``./codequoter codequoter 8 10``:



[codequoter Line 8](https://github.com/cmark0v/codequoter/blob/master/codequoter#L8)
```perl
# File: codequoter
# Lines: 8-11

8  $fname = `basename $file`;
9  chomp($fname);
10 $cmd = "(cd $c ; git ls-files --full-name $fname)";
11 $path = `$cmd`;
```

