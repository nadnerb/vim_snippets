# vim_snippets

Beginner vim snippets. I am sure there are better ways to do some of these.

#### split commas into new lines:
```
s/, /\r/
```

## Search and Replace

-- remove n characters from the end of a line
```
s/.\{n}$//
```
#### remove first characters
```
s/\(characters\)\(.*$\)/\2/g
```

#### change `'key' : '#some-value',`
```
s/\(.*: \)\('#.*'\)\(,\?\)/\1{'element': \2, 'default': ''}\3/g
```

#### insert before

```
ctrl v
j to where u want
shift i
esc
```

### save readonly

`:w !sudo tee %`

