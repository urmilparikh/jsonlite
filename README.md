# jsonlite

Jsonlite is a variant of json, aims for human readability and writability.

Object key, string value, number vaue, true, false, null in json can all be without quotes, as long as they don't contain special characters: spaces(` `, `\t`, `\n`...), double quote(`"`), comma(`,`), square brackets(`[`,`]`), object start and end (`{`, `}` or `(`, `)`, depending on options), pair seperators (`:` or `=` depending on options).

You can set `jsonObjectFormat` to `false` to use (`=`) instead of {`:`} for objects.

Example 1: `{max-length: 50}` is same to this JSON: `{"max-length": 50}`

Example 2 (with `jsonObjectFormat` = `false`): `(name=jsonlite, birthday=(year=2013, month=7, day=7), isGreat=true)` is the same to `{"name": "jsonlite", birthday: {"year": 2013, "month": 7, "day": 7}, "isGreat": true}`

You can use [TypeScript version](jsonlite.ts), or [JavaScript version](jsonlite.js), ~~or you can play with F12(js console) at this page~~.

```js
var obj1 = jsonlite.parse('{max-length: 50}');
var obj2 = jsonlite.parse('(name=jsonlite, birthday=(year=2013, month=7, date=7), isGreat=true)', false);
```

# Credits

This repo is just a replica from https://deerchao.cn/projects/jsonlite/
