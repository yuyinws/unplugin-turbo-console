# 配置

## 插件选项

| 属性        |      类型      | 默认值 | 描述 |
| ------------- | :-----------: | ----: | ------------- |
| prefix / suffix    | `string` | "" | [自定义前后缀](/zh-CN/features/custom-prefix) |
| disableLaunchEditor |   `boolean`   | false | 是否禁用[编辑器跳转](/zh-CN/features/launch-editor)功能 |
| specifiedEditor | `string` | "" | 指定打开的编辑器，[所有支持的编辑器](https://github.com/yyx990803/launch-editor#supported-editors) |
| disableHighlight      |   `boolean`   | false | 是否禁用[高亮输出](/zh-CN/features/highlight)功能 |
| port | `number` | 3070 | 指定插件的服务端口号 |
| extendedPathFileNames | `string[]` | [] | [拓展路径文件名](/zh-CN/features/highlight.html#拓展路径文件名) |
| babelParserPlugins | `ParserPlugin[]` | ["typescript", "jsx"] | babel插件，传入的值会与默认值自动合并。[所有插件](https://babeljs.io/docs/en/babel-parser#plugins) |
| silent | `boolean` | false | 阻止项目启动时插件的终端输出 |