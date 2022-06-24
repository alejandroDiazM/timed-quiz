# TIMED QUIZ

This small application, written in Go to test the use of basic packages, will make you answer easy math problems within a time limit. 

The program expects a CSV file called "problems.csv" with the next format:

```csv
5+5,10
2+3,5
...
```
<br>

There is such a file in the repo, but feel free to add your own problems. The default time limit is set at 30 seconds, but you can change it updating line 14 in main.go:

```go
timeLimit := flag.Int("limit", 30, "the time limit for the quiz in seconds")
```
<br>

## Usage:

After cloning the repo, and assuming you have GoLang installed, go to the directory and run the next command to start the game:

```powershell
go run main.go
```
<br>

The output will be something like this:

```
Problem #1: 5+5 =
```
<br>
Input your answer, press Enter, and keep going until you finish or the timer expires! After one of those conditions is met, the program will tell you your score.