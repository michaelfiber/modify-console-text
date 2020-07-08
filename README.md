# Modify Console Text
This is a dead simple tool to modify text so that it has more style on console output. There are more featureful tools out there for styling console output but this does exactly what I needed for my projects.

This example imports the module, then uses it to set a yellow foreground, red background, and makes the text bright. The module simply adds all the modifiers to the front of the string and adds the Clear modifier to the end.
```typescript
import modify from 'modify-console-text';

console.log(modify('This is the message', 'FgYellow', 'BgRed', 'Bright'));
```

The following codes are availabile:

Style | What gets inserted
----- | ------------------
Reset | "\x1b[0m"
Bright | "\x1b[1m"
Dim | "\x1b[2m"
Underscore | "\x1b[4m"
Blink | "\x1b[5m"
Reverse | "\x1b[7m"
Hidden | "\x1b[8m"
FgBlack | "\x1b[30m"
FgRed | "\x1b[31m"
FgGreen | "\x1b[32m"
FgYellow | "\x1b[33m"
FgBlue | "\x1b[34m"
FgMagenta | "\x1b[35m"
FgCyan | "\x1b[36m"
FgWhite | "\x1b[37m"
BgBlack | "\x1b[40m"
BgRed | "\x1b[41m"
BgGreen | "\x1b[42m"
BgYellow | "\x1b[43m"
BgBlue | "\x1b[44m"
BgMagenta | "\x1b[45m"
BgCyan | "\x1b[46m"
BgWhite | "\x1b[47m"