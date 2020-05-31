## 坑

- husky 无响应，git commit 时没有执行 hook，可尝试删除 node_moduls，单独安装 cnpm i husky -D，成功时会在在.git\hooks 目录下生成相关文件