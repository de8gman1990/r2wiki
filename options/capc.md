<!-- TITLE: C -->

#  **`C`** Code metadata (comments, format, hints, ..)


```text
Usage: C[-LCvsdfm*?][*?] [...] # Metadata management
```


- **`C`** list meta info in human friendly form
- **`C*`** list meta info in r2 commands
- **`C[Chsdmf]`** list comments/hidden/strings/data/magic/formatted in human friendly form
- **`C[Chsdmf]*`** list comments/hidden/strings/data/magic/formatted in r2 commands
- **`C- [len] [[@]addr]`** delete metadata at given address range
- **`CL[-][*] [file:line] [addr]`** show or add 'code line' information (bininfo)

- [ **`CS[-][space]`** manage meta-spaces to filter comments, etc..](/options/capc/CS)

- [ **`CC[?] [-] [comment-text] [@addr]`** add/remove comment](/options/capc/CC)

- **`CC.[addr]`** show comment in current address
- **`CC! [@addr]`** edit comment with $EDITOR
- **`CCa[-at]|[at] [text] [@addr]`** add/remove comment at given address
- **`CCu [comment-text] [@addr]`** add unique comment
- **`Cv[bsr][?]`** add comments to args

- [ **`Cs[?] [-] [size] [@addr]`** add string](/options/capc/Cs)

- **`Cz[@addr]`** add string (see Cs?)
- **`Ch[-] [size] [@addr]`** hide data
- **`Cd[-] [size] [repeat] [@addr]`** hexdump data array (Cd 4 10 == dword [10])

- [ **`Cf[?][-] [sz] [0|cnt][fmt] [a0 a1...] [@addr]`** format memory (see pf?)](/options/capc/Cf)

- **`CF[sz] [fcn-sign..] [@addr]`** function signature
- **`Cm[-] [sz] [fmt..] [@addr]`** magic parse (see pm?)