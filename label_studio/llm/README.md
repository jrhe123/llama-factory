1. import chat history (data.txt)
2. select any NLP template
3. use code to edit the label pattern

```
<View>
  <!-- 任务说明 -->
  <Header value="特定领域信息抽取" />

  <!-- 展示文本：假设导入数据时字段名为 text -->
  <Text name="text" value="$text" highlightColor="#ffffaa" />

    <!-- 情感分析编辑区 -->
    <View whenTagValue="位置信息">
        <Header value="位置信息"/>
        <TextArea name="position" toName="text"
                  editable="true"
                  rows="3"
                  placeholder="描述情感特征"/>
    </View>

    <!-- 文本分类编辑区 -->
    <View whenTagValue="组织信息">
        <Header value="组织信息"/>
        <TextArea name="organization" toName="text"
                  editable="true"
                  rows="3"
                  placeholder="组织信息"/>
    </View>

    ....more
</View>


```