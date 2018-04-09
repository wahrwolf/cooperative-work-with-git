# thoughts (and prayers)

# the fix
## tooling
- git
- grep
- make
- compiler
  - gcc
  - pdflatex

# the fix - init

## project dir structure
```
lecture-practice
|--- .git
|--- .gitignore
|--- points
---- README.md
```

## init - extended
- add a .gitignore
- private vs public repo

## add a task sheet
- create a dir per lesson
  - e.g. 00, 01, 02 ...
- setup a simple structure
- add first tasksheet, material etc
  - `git commit -m "0X: init"`

## task dir structure
```
01
|--- 01-extra
|--- solution
|--- src
---- tasksheet-01.pdf
```

## create dummy solution
- seperate tasks
- add a build script
  - makefile
- `git commit -m "0X: adds dummy"`

## dummy solution - exapmle
```
06  
|--- Abgabe  
|   |--- ddt.pdf  
|   |--- timempi2.c  
|   |--- timempi.c  
|   ---- timempi.sh  
|--- task-03  
|   |--- ddt.tex  
|   |--- img  
|   ---- Teilaufgaben  
|       |--- 3.1.tex  
|       |--- 3.2.tex  
|       |--- 3.3.tex  
|       ---- 3.4.tex  
---- tasksheet-06.pdf  
```

