# Group 8's: Java Standard

## FILE BASICS
1. File name consists of the case-sensitive name of the top-level class.
2. Files are encoded in UTF-8.
3. Aside from line terminators and the ASCII horizontal space character, no other whitespace characters should appear in our files.
    3.1. All other whitespace characters in string and character literals are escaped.
    3.2. Tab characters are not used for indentation.
    3.3. Indent like its Python.
4. Any character that has a special escape sequence (\b, \t, \n, \f, \r, \", \' and \\), uses that sequence  rather than the corresponding octal (e.g. \012) or Unicode (e.g. \u000a) escape.
5. For remaining non-ASCII characters, either the actual Unicode character (e.g. ∞) or the equivalent Unicode escape (e.g. \u221e) is used. The choice depends only on which makes the code easier to read and understand.

## FILE STRUCTURE
1. A source file consists of, in order:
    1.1. License or copyright information, if present
    1.2. Package statement - Not line-wrapped. Column limit does not apply.
    1.3. Import statements - Not line-wrapped. Column limit does not apply.
    1.4. Exactly one top-level class - Top level classes are in their own file, the members and initializers are orgainzed logically, not chronologically. 
    *Note: Methods of a class that share the same name (overloads/constructors etc) appear in a single contiguous group.*
2. Exactly one blank line separates each section that is present.

