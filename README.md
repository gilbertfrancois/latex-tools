# LaTeX Tools

*Gilbert François Duivesteijn*



## lxlc: LaTeX label counter

When working on large documents, it can happen that a label for a figure or table has been duplicated, causing all references to be replaced by ??. Finding duplicate labels can be a tedious task. This small utility scans the document(s) and shows all used labels with the line number where they are defined. If a label has been duplicated, it shows a warning.



Example usage:

```
$ lxlc test.tex

label                          | line number          | status
-------------------------------+----------------------+---------
                    20230309-1 |                   33 | [  OK  ]
                    20230309-2 |                   42 | [  OK  ]
                    20230309-3 |                   64 | [  OK  ]
                    20230309-4 |                   83 | [  OK  ]
                    20230310-1 |             104, 138 | [ WARN ]
                    20230310-3 |                  157 | [  OK  ]
                    20230313-1 |                  182 | [  OK  ]
                    20230313-2 |                  214 | [  OK  ]
                    20230313-3 |                  234 | [  OK  ]
                    20230314-1 |                  271 | [  OK  ]
                    20230314-2 |                  293 | [  OK  ]
                    20230314-3 |                  307 | [  OK  ]
                    20230314-4 |                  317 | [  OK  ]
                    20230314-5 |                  335 | [  OK  ]
                    20230314-6 |                  345 | [  OK  ]
```



## Installation

- Make sure you have a recent version of python3 installed and that `/usr/bin/python3 --version` works. The apps don't need any additional libraries.

- Copy the LaTeX cli tools from this project to e.g. `/usr/local/bin` or `$HOME/.bin` folder. That's all.

 

