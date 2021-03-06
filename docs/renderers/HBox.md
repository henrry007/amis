## HBox

| 属性名                     | 类型                              | 默认值         | 说明                 |
| -------------------------- | --------------------------------- | -------------- | -------------------- |
| type                       | `string`                          | `"hbox"`       | 指定为 HBox 渲染器   |
| className                  | `string`                          |                | 外层 Dom 的类名      |
| columns                    | `Array`                           |                | 列集合               |
| columns[x]                 | [Container](./Types.md#Container) |                | 成员可以是其他渲染器 |
| columns[x].columnClassName | `string`                          | `"wrapper-xs"` | 列上类名             |

```schema:height="300" scope="body"
[
    {
        "type": "hbox",
        "className": "b-a bg-dark lter",
        "columns": [
            {
                "type": "plain",
                "text": "Col A",
                "columnClassName": "wrapper-xs b-r"
            },

            "Col B"
        ]
    },

    {
        "type": "hbox",
        "className": "b-a m-t bg-dark lter",
        "columns": [
            {
                "type": "plain",
                "text": "w-md",
                "columnClassName": "w-md wrapper-xs bg-primary b-r"
            },
            "..."
        ]
    }
]
```
