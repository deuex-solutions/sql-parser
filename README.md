# sql-parser
Userful minimal parser for sql and hive quires.


## Note

We are not official author of this library, We pick few useful files to just parse query & get errors + suggestedKeywords

Please visit  [official website](https://docs.gethue.com/developer/api/#sql-autocompletion) for more info


## How to use

Download or clone this repo by using belowe command

```js
git clone https://github.com/deuex-solutions/sql-parser.git
```
Refer below example for use.

```js
**import** sqlAutocompleteParser from 'sql-parser';

const beforeCursor = 'SELECT col1, col2, tbl2.col3 FROM tbl; '; // Note extra space at end
const afterCursor = '';
const dialect = 'hive';
const debug = false;

console.log(
  JSON.stringify(
    sqlAutocompleteParser.parseSql(beforeCursor, afterCursor, dialect, debug),
    null,
    2
  )
);
```
## Contribute

Found an issue? Post it in the [issue tracker](https://github.com/deuex-solutions/sql-parser/issues). <br> 
Want to add another awesome feature? [Fork](https://github.com/deuex-solutions/sql-parser/fork) this repository and add your feature, then send a pull request.

## License
The MIT License (MIT)