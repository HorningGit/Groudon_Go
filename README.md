# :whale: Gyarados Golang :whale2:






<!--Linux/BSD_Install-->
#### 🔵 Installing Go on RHEL Based Systems
<ins>To setup the Go environment through the Linux command line, please proceed with the following steps!</ins>
1. Assuming the Linux system is up-to-date, [**cd**](https://man7.org/linux/man-pages/man1/cd.1p.html) into the Linux system's current home directory:
```
$ cd ~
```
2. Use the [**wget**](https://man7.org/linux/man-pages/man1/wget.1.html) command to install the tar archive from the official Go downloads page:
```
$ wget https://go.dev.dl/go1.18.4.linux-amd64.tar.gz
```
3. Add Go to $PATH so that the **go** command is accessible:
```
$ echo 'export PATH=$PATH:/usr/local/go/bin' >> $HOME/.profile
$ source $HOME/.profile
```
<ins>Define the $GOPATH environment variable to make it clear where our Go workspace will be!</ins>
1. Add the following lines to the _.profile_ file with the [**export**](https://www.man7.org/linux/man-pages/man1/export.1p.html) command:
```
$ export GOPATH=$HOME/go
$ export PATH=$PATH:$GOPATH/bin
```
















#### 🔵 Basic Admin Commands
```
- Compile and Run your Go program:
    go run <file path>

- Open Package Documentation using doc command:
    go doc <package>

- Compile your Go package:
    go build <package path>

-  Create a new module:
    go mod init <module path>

- Compile your app package:
    go build <package path>
```

* Install and run from a remote location:

```
go install github.com/bregman-arie/myApp
bin/myApp
```

### 🔵 FMT Cheat Sheet
##### PRINT
```
%v	the value in a default format
	when printing structs, the plus flag (%+v) adds field names   
%#v 	a Go-syntax representation of the value
%T  	a Go-syntax representation of the type of the value
%%	a literal percent sign; consumes no value
```

##### SPRINT
```
- func Sprint(a ...any) string
	Sprintf formats according to a format specifier and returns the resulting string.
```

###### Basic Numberic Types in Go
Data Type | Memory Usage - Number of Bits | Minimum Value | Maximum Value
:------|:------:|:------:|:------:
bool | 1 | 1 | 1
int8 | 8 | -128 | 127
int16 | 16 | -32,768 | 32,767
int32 | 32 | -2,147,483,648 | -2,147,483,647
int64 | 64 | -9,223,372,036,854,775,808 | 9,223,372,036,854,775,807
uint8 | 8 | 0 | 225
uint16 | 16 | 0 | 65,535
uint32 | 32 | 0 | 4,294,967,295
uint64 | 64 | 0 | 18,446,744,073,709,551,615


## Golang (Go) Resources
- [Golang | Home Page](https://go.dev/)
- [Golang | Documentation](https://go.dev/doc/)
- [Golang | GitHub](https://github.com/golang)
- [Golang | Examples of Go Programs/Scripts](https://golangexample.com/)

### Cheat Sheet

* Run your program:

```
go run <file path>
```
* Create a new module:

```
go mod init <module path>
```

* Compile your app package:

```
go build <package path>
```

* Install and run from a remote location:

```
go install github.com/bregman-arie/myApp
bin/myApp
```

___
## :white_circle: *Environment Variable Modification*
  <!-- Default Shell EV -->
#### :small_blue_diamond: Changing Default Shell Prompt
```
[PS1 Environment Variable]
- PS1 is a primary prompt variable which holds @\u@\h \W\\$ special bash characters. 
- Display during terminal login.
- Default bash prompt.

[Location]
Default Location = /etc/bashrc

[Modifying]
PS1='[[prod]\u@\h \W]\$' 

[Modified shell prompt]
[[prod]root@hostname ~]#
````
