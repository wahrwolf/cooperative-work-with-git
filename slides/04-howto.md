# howto
## config stuff
- generate ssh keys
  - `mkdir -p ~/.ssh/keys`
  - `ssh-keygen -f ~/.ssh/keys/gogs_rsa`

### ssh config:
```
Host gogs
	Hostname gogs.mafiasi.de
	User gogs 
	IdentityFile ~/.ssh/keys/gogs_rsa
	IdentitiesOnly yes
```

## setting up the team
- [mafiasi team](https://mafiasi.de/groups/create)
  - for mail list
  - for etherpad
- [gogs organisation](https://gogs.mafiasi.de/org/create)
- `{lecture}-{semester}-{slug}`
- add all members by email
  - double check mails!
  - send test mail

## setting up the repo
- e.g. [gogs](https://gogs.mafiasi.de)
  - add correct .gitignore
- `git clone gogs:user/{lecture}-{semester}-{slug}`
- edit README.md
  - add all members by name/email
  - how to access new tasks
  - how to submit solutions
  - submission deadlines
- add a points
- `git add README.md points`
- `git commit -m "orga: adds submission info`

## setting up the Makefile
- collection of scripts to build your project
- define useful targets
  - next: to get next tasksheet
  - abgabe: to pack everything for submission
  - current: to build everything
- comment everything!
- use variables
  - `%.o: %.c` - partwise match
  - `$@` - target file
  - `$<` - source files
- keep it simple/readable
- keep it reusable!


## dummy solution
- `make 00`
- `git add 00/`
- `git commit -m "00: init"`

### example dir
```
06
|--- ddt.pdf
|--- task-06  
|   |--- ddt.tex  
|   |--- img  
|       |--- octopus.png
|   ---- Teilaufgaben  
|       |--- 6.1.tex  
|       |--- 6.2.tex  
---- tasksheet-06.pdf  
```
