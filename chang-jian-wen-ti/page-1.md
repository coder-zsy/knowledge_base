# Page 1

## CocoaPods was not able to update the \`cocoapods\` repo 或 CocoaPods was not able to update the `master` repo. If this is an unexpected issue and persists you can inspect it running `pod repo update --verbose`

```
// 查看当前repo列表
pod repo list
// 删除不必要的repo，现在一般不用mast库，使用trunk索引库(有CDN)，所以可以删除master库的repou引用
pod repo remove master
// 重新更新repo
pod update


// 部分repo可以尝试直接用git命令拉取索引
cd ~/.cocoapods/repos/trunk
git pull
```
