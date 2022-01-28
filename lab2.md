# Week 4 Lab Report - Bug Fixes
## Bug Fix #1
![Bug 1](lab2/bug1.png)
The first bug is an infinit while loop. The bug occurs because the script keeps looking for links and assumes that the final line of the md file ends with a link. As a result, the script is stuck in an infinit while loop until there is not enough space in the heap. Here is the link to the test file. [test file link](https://github.com/tarunm20/markdown-parse/blob/main/test-file2.md)

```
(base) ➜  markdown-parse git:(main) ✗ java MarkdownParse test-file2.md
Exception in thread "main" java.lang.OutOfMemoryError: Java heap space
        at java.base/java.util.Arrays.copyOfRange(Arrays.java:3821)
        at java.base/java.lang.StringLatin1.newString(StringLatin1.java:769)
        at java.base/java.lang.String.substring(String.java:1912)
        at MarkdownParse.getLinks(MarkdownParse.java:18)
        at MarkdownParse.main(MarkdownParse.java:26)
```

## Bug Fix #2

## Bug Fix #3
