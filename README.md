Language speed comparison
=========================

Language relative speed is assessed by measuring speed
of solving specific problem using specific algorithm
implemented with most natural (idiomatic) tools available
in given language.

The problem that is being solved by test programs
is building a *trie* (a prefix tree) for Polish language
dictionary \([gz](http://codestation.org/download/slowa.txt.gz), [bz2](http://codestation.org/download/slowa.txt.bz2)\).

Most implementations use their respective hash-maps
to link prefixes with tails.

All tests runs were performed with tcmalloc preloaded
(if using it improved performance).

| Language   | Time (seconds) | Memory (KiB) | Run-time/Compiler version |
|------------|---------------:|-------------:|---------------------------|
| C++        |           1.36 |       501080 | GCC 5.3.1                 |
| C#         |           5.30 |       983968 | 4.2.1.0                   |
| Go         |           2.99 |       548948 | go1.6rc                   |
| [Huginn](http://codestation.org/?h-action=menu-project&menu=submenu-project&page=&project=huginn) | 59.72 | 3135352 | (HEAD) |
| Java       |           2.90 |      1265092 | Oracle Java 1.7.0         |
| JavaScript |           5.97 |       492272 | NodeJS 4.2.6              |
| Julia      |          11.10 |      3341924 | 0.4.7                     |
| Lua        |          20.60 |      1364400 | 5.2.4                     |
| Perl       |          69.46 |      1801748 | 5.22.1                    |
| PHP        |          78.24 |      1487980 | 7.0                       |
| Python     |          22.89 |      1376728 | 3.6.3                     |
| Ruby       |          16.30 |      1282492 | 2.2.4                     |

Dictionary loaded contains 2709883 words, with 30504772 characters in total.

