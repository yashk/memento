
## Replacing epoch with human readable date
https://www.farsightsecurity.com/blog/txt-record/jq-20181030/

Syntax

```
(.field |= todate) ? //.
```
This can also be used to transform other fields with functions.
