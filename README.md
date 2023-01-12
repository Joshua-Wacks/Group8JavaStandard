# Group 8's: Java Standard, built upon [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html#s4-formatting)

## Source file basics & file structure

### 1. File name consists of the case-sensitive name of the top-level class. Top level classes are in their own file, the members and initializers are orgainzed logically, not chronologically. Methods of a class that share the same name (overloads/constructors etc) appear in a single contigious group.
### 2. A source file consists of, in order:
### - License or copyright information, if present
### - Package statement - Not line-wrapped. Column limit does not apply.
### - Import statements - Not line-wrapped. Column limit does not apply.
### - Exactly one top-level class per file.
### (These are divided by one blank line.)

## Formatting & naming

### 3. (refers to rule 4.1.2) Opening braces are on new lines. Except for empty functions which can be on one line.
### 4.(Refers to rule 4.2) Spaces instead of tabs. Indent like you are writing Python. Indentations are 4 spaces.
### 5. (Refers to rule 4.3) A function should complete 1 purpose and one statement per line
### 6. (Refers to rule 4.8.3.1) Arrays should be declared and initialized all on one line, excpet in the case of 2D arrays.
### 7. (Refers to rule 4.8.6) Rules for Comments: Any comment style is allowed such as // but /* */ should be used for larger comments. Comments should not duplicate the code. Good comments do not excuse unclear code.  If you can’t write a clear comment, there may be a problem with the code.  Comments should dispel confusion, not cause it. Provide links to the original source of copied code. Write comments at incomplete code.

## Programming practices & Javadoc

### 8. Use @Override when you are expecting to override
### 9. Don't ignore caught exceptions
### 10. Call static methods on class not instance
### 11. Detailed comment for a class at the top of the file
### 12. Comments on methods only where explanation is needed taking into account public methods may require more comments

## Overall Rules 
### Rule 1) Explicit over implicit: Be clear and verbose over unreadable and over-simplified. This applies to variable names, functions, errors, classes etc.
### Rule 2) Every if should have an else.
### Rule 3) Use a for loop if the number of iterations is knows. While(true) is a no-go.
### Rule 4) A function should complete 1 purpose.
### Rule 5) Avoid global variables where possible,unless using constants/config files.
