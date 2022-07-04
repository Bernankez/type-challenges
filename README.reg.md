将答题按钮替换成自己的issue：

vscode批量替换

```ts
// 匹配zh-CN按钮
const origin = https:\/\/tsch.js.org\/(\d*)\/answer\/zh-CN

// 匹配没有中文翻译的题按钮
const origin2 = https:\/\/tsch.js.org\/(\d*)\/answer(?=")

const target = https://github.com/Bernankez/type-challenges/issues/new?assignees=&labels=answer%2C+zh-CN&template=1-answer.zh-CN.md&title=$1+-+
```
