#### Single regex that matches either of these: `antelope rocks out`, `antelopes rock out`
=> `([a-zA-Z]+?)(s\b|\b)`

#### Regex that matches either of: `goat`, `moat`, but not: `boat`
=> `[^b]oat`

#### Regex that matches dates in YYYY-MM-DD format. (Year can be 1-4 digits, and month and day can each be 1-2 digits). This does not need to verify the date is correct (e.g 3333-33-33 can match).

`2000-10-12`, `1999-1-20`, `1999-01-20`, `812-2-10`
=> `\d{1,4}-\d{1,2}-\d{1,2}`

#### VT-100 regex
=> `\[\d{1,2}[\w;]\d?\d?\w?`