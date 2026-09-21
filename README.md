# grepwc
What grepwc does: This fancy command combines grep and wc. The grepwc file will take a filename argument and a pattern argument. This command will then return the lines with this pattern, along with the line number and word count for that line.
Grepwc Syntax : node grepwc <FILENAME> <PATTERN>
Grepwc Expected Behavior: Return Line that includes pattern, along with Line number and word count for line.
Grepwc Edge Cases: If pattern does not appear in document >> Nothing will return. 
If pattern is a substring of a longer word (EG. ErrorInfo for Error pattern), it will still return that line, similar to the actual grep command.


#What I used AI for
AI helped me identify how to fix problems, while also creating test cases for my edge cases to ensure that the code worked. When I asked for test cases, it also pointed out an underlying bug which I did not notice in my if process.argv.length < 3 argument, which I tweaked to 4 to make sure that the pattern is required.
