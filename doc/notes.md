## 坑

- husky 无响应，git commit 时没有执行 hook，可尝试删除 node_moduls，单独安装 cnpm i husky -D，成功时会在在.git\hooks 目录下生成相关文件
- react Fragments,React 中一个常见模式是为一个组件返回多个元素。Fragments 可以让你聚合一个子元素列表，并且不在 DOM 中增加额外节点。