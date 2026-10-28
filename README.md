# Leo CocoaPods Specs

Aeris / LeoURN 的公开 CocoaPods Specs 分发仓库。预览规格已进入 Specs 索引：AerisContracts / Aeris / AerisHost 0.25.0、LeoURN 0.1.0。源码固定为公开完整 commit。npm 包的上传和安装验收单独记录。

接入方在 Podfile 添加：

```ruby
source 'https://github.com/zhangguozhong/leo-podspecs.git'
source 'https://cdn.cocoapods.org/'
```

Aeris 的原生依赖通过此仓库解析。React Native 插件和 LeoURN 通常从 npm 安装后自动链接；不要为同名 Pod 再声明不同的 Git 或 :path 来源。

Swift 的容器模块仍使用 `import URN`，Pod 名为 LeoURN。React Native 基线为 0.87.0 / React 19.2.3 / iOS 15.1+。

正式 Specs 应使用不可变 tag 或完整 commit，已经发布的同版本规格不覆盖。Candidates 不代表版本已正式发布，也不应加入生产依赖。
