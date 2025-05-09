# ag

> The Silver Searcher. 类似 `ack`, 但是更快。
> 更多信息：<https://manned.org/ag>.

- 寻找内容包含"小明"的文件，并列出所在的行数：

`ag {{小明}}`

- 在指定目录中寻找内容包含 "foo" 的文件：

`ag {{小明}} {{指定的目录}}`

- 寻找内容包含 "foo" 的文件，但只列出文件名：

`ag -l {{小明}}`

- 忽略大小写，寻找内容包含 "ABC" 的文件，并只输出匹配的内容，而非整行：

`ag -i -o {{ABC}}`

- 在文件名包含"小红"的文件中寻找"小明"：

`ag {{小明}} -G {{小红}}`

- 使用正则表达式来匹配文件内容：

`ag '{{^ba(r|z)$}}'`

- 输出文件名包含"小明"的文件名：

`ag -g {{小明}}`
