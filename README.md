git-sparse
==========

git command extention for sparse-checkout.  
**This command enables you to share sparse-checkout setting in the team and apply it easily.**

## Installation

clone this repository and move `git-sparse` file to ...

* Linux/Mac user  
  ~/local/bin/
* Windows user  
  %UserProfile%\bin

## How to use

#### 1  prepare `.gitsparse` file and write target file/folder.

`.gitsparse` file is like below.

```
target/folder
targetfile.txt
submodule:target/folder
```

if you apply sparse-checkout to submodule, write as `<submodule name>:<target folder>`


#### 2 execute command  
Then , only you have to do is executing `git sparse`.

#### Attention
`.gitsparse` must be `utf-8` encoding **without BOM**.  
`.gitsparse` must include more than 1 carriage return (crlf or lf).
