# My Vim Journey

> Basic Vim commands to start the Vim Journey

## Global

```bash
vim <filename>       # Open <filename> in vim
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

## Editing

### Insert

```bash
	i	# insert before the cursor
	I	# insert at the beginning of the line
	a       # insert (append) after the cursor
	A       # insert (append) at the end of the line
	ea	# go to end of the word and insert
	o       # append (open) a new line below the current line
	O       # append (open) a new line above the current line
	ea      # insert (append) at the end of the word
	Esc     # exit insert mode
```

### Remove

```bash
	r       # replace a single character
	R	# replace multiple character // press <esc> to exit
	x	# exterminate the character under the cursor
	X	# exterminate the character before the cursor
	cw	# change to the start of the next word (take to buffer and insert)
	cc	# change entire line
	C	# change rest of the line
	dw	# remove to end of the word and take to buffer
	dd	# remove entire line and take to buffer
	D	# remove rest of the line and take to buffer

```

> **These commands are best when used with the modifiers**

### Copy and Paste

```bash
	yw 	# yank (copy) the characters of the word from the cursor position to the start of the next word
	yy	# yank entire line
	Y	# same as above
	p	# paste before the cursor
	P	# paste after the cursor
```

## Scrolling

```bash
	Ctr + b	 # move back one full screen
	Ctr + f	 # move forward one full screen
	Ctrl + d # move forward 1/2 a screen
	Ctrl + u # move back 1/2 a screen
	zz	 # put the line with the cursor at the center
	zb	 # put the line with the cursor at the bottom of the screen
	zt	 # put the line with the cursor at the top
```

## Visual Mode

```bash
	v	 # start visual mode, mark lines
	V	 # start linewise visual mode
	Ctrl + v # start visual block mode
	o	 # move to other end of marked area
	O	 # move to other corner of block
	<Esc>	 # exit visual mode
```

> With Visual mode you can do commands like yank, delete, change etc.

## Search

```bash
	/pattern	# search for a pattern which will take you to the next occurrence.
	?pattern	# search for a pattern which will take you to the previous occurrence.
	n		# repeat search in same direction
	N		# repeat search in opposite direction
	:noh		# remove highlighting of search matches
	fx		# jump to next occurrence of character x
	tx		# jump to before next occurrence of character x
	;		# continue jumping
```
