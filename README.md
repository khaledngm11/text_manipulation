# # Linux Text Processing Tools
* grep
* cut
* sed
* sort
* uniq
* Examples ( most important )

  * Log file analysis
  * Frequency analysis

## 1. grep
**GREP** is a tool that uses Regular Expressions, and prints any lines which match a specified pattern .

`Syntax`
`grep [options] pattern [files]`


```
 Most important Options:
-c: Count the number of lines that match a pattern.
-h: Display the matched lines, but do not display the filenames.
-i: Ignore case for matching.
-l: Displays list of a filenames only.
-n: Display the matched lines with line numbers.
-v: Prints all the lines that do not match the pattern.
-e exp: Specifies expression with this option. Can use multiple times.
-f file: Takes patterns from a file.
-E: Treats pattern as an extended regular expression (ERE).
-w: Match whole word.
-o : Print only the matched parts of a matching line.
```
## 2. cut
**CUT**  is a command-line tool for cutting text and writing the result to standard output .

`Syntax`
`cut [options] [files]`
```
Most important Options: 
-b, --bytes=LIST        # select only these bytes
-c, --characters=LIST   # select only these characters
-d, --delimiter=DELIM   # use DELIM instead of TAB for field delimiter
-f, --fields=LIST       # select only these fields;  also print any line that 
```
## 3. sed
**SED**   A stream editor is used to perform basic text transformations , such as searching , editing , replacing , insertion or deletion  .

`Syntax`
`sed [options] [script] [files]`
```
 Most important Options: 
-n  : suppress automatic printing of pattern space
-e  : add the script to the commands to be executed
-f  : add the contents of script-file to the commands to be executed
-i  : Changes in orignal file
-r  : use extended regular expressions in the script
```
```
Operations:
s : for substitution
d : for deletion
p : Print out the pattern space (to the standard output). This command is usually only used in conjunction with the -n command-line option.
g : global replacement
i : Insert data  
a : Append data
```
## 4. sort
**SORT** is used to arrange lines numerically and alphabetically.

`Syntax`
`sort [options] [files]`
```
 Most important Options: 
-d, --dictionary-order : consider only blanks and alphanumeric characters
-f, --ignore-case : fold lower case to upper case characters
-M, --month-sort : compare (unknown) < 'JAN' < ... < 'DEC'
-h, --human-numeric-sort : compare human readable numbers (e.g., 2K 1G)
-n, --numeric-sort : compare according to string numerical value
-R, --random-sort : shuffle, but group identical keys.  See shuf(1)
-r --reverse : reverse the result of comparisons

```
## 5. uniq
**UNIQ** is used to filters out the repeated lines in a file.

`Syntax`
`uniq [options] [files]`
```
 Most important Options: 
-c, --count : prefix lines by the number of occurrences
-d, --repeated : only print duplicate lines, one for each group
-D  : print all duplicate lines
-i, --ignore-case :  ignore differences in case when comparing
-u, --unique :  only print unique lines

```
