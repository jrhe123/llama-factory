## Adding label to e-commerce product feedback

1. text classification
- positive
- negative
- neutral

2. steps to setup label options
- settings
- labeling interface
- add label choices (Code or Visual)

```
<View>
  <Labels name="label" toName="text">
    <Label value="PER" background="red"/>
    <Label value="ORG" background="darkorange"/>
    <Label value="LOC" background="orange"/>
    <Label value="MISC" background="green"/>
  </Labels>

  <Text name="text" value="$text"/>
</View>
```

3. label the data
- cmd + enter (submit label)