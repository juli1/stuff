# Jq

Query Json files from the command line. Like a swiss-army tool for Json parsing/analysis.

## Printing
Print fields
```
jq '.field' file.json
```

Print all elements from an array
```
jq '.arrayMember | .[]
```

## Searching

```
jq '.[] |  select(.field1 == value1) | select(.field2 == "value2")  ' file.json
```

## Notes
1. The ```|``` character is used to combine operations
