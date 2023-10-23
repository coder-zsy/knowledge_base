# 子模块

当项目中存在子模块时，直接使用`git clone xxx.git`会发现子模块文件夹是空的，这个时候有两种方法：

## 方法一：递归的下载子模块

```shell
git clone --recursive xxxx.git
```

## 方法二：下载完主模块后，更新子模块

```shell
git clone https://xxxmainModule.git
cd subModule
git submodule update --init
```

