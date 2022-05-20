# Bash

See also [Ubuntu](../ubuntu/README.md)

### Page contents

 - [Extract part of a string](#extract-part-of-a-string)

### Extract part of a string

Example - extract the string inside a `name="..."` attribute:
```bash
grep -Po 'name="\K[^"]*'
# -P  Interpret PATTERNS as Perl-compatible regular expressions (PCREs)
# -o  Print only the matched (non-empty) parts of a matching line
# \K  The text matched by the part of the regex to the left of the \K is omitted from the overall regex match
```
