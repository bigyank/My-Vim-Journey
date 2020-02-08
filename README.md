# My Vim Journey

> Basic Vim commands to start the Vim Journey

## Global

```bash
vim <filename>   # Open <filename> in vim
    :help <topic>    # Open up built-in help docs about <topic> if any exists
    :q               # Quit vim
    :w               # Save current file
    :wq              # Save file and quit vim
    ZZ               # Save file and quit vim
    :q!              # Quit vim without saving file
                     # ! *forces* :q to execute, hence quiting vim without saving
    :x               # Save file and quit vim, shorter version of :wq
```

## Vim Modes

```bash
	:	# exec mode
	<esc>	# command mode
	v	# visual mode
	i	# Insert before cursor
	a	# Append after cursor
	I	# Insert at beginning of the line
	A	# Append at the end of the line
```

## Navigation

### General Movement

```bash
	h	# move one character left
	j	# move one row down
	k	# move one row up
	l	# move one character right
```

### Moving Horizontally

```bash
	w	# move to beginning of next word (Does'nt Ignore punctuation)
	b	# move to beginning of previous word
	e	# move to end of word
	W	# move to beginning of next word after a whitespace
	B	# move to beginning of previous word before a whitespace
	E	# move to end of word before a whitespace
	0	# move to beginning of line
	$	# move to end of line
	^	# move to first non-blank char of the line
```

> **All the above movements can be preceded by a count; e.g. 4j will move down 4 lines.**

### Moving Vertically

```bash
	gg	# move to first line
	G	# move to last line
	nG	# move to nth line
	:n	# (same as above)
	H	# Move to top of screen
	M	# move to middle of screen
	L	# move to bottom of screen
	%	# Jump to matching parenthesis
	}	# jump to next paragraph (or function/block, when editing code)
	{	# jump to previous paragraph (or function/block, when editing code)
```
