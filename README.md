# Leo CocoaPods Specs

Aeris 和 LeoURN 的 CocoaPods Specs 索引，供 iOS 原生工程、React Native 和 Flutter 插件解析原生依赖。

## 配置 Podfile

```ruby
source 'https://github.com/zhangguozhong/leo-podspecs.git'
source 'https://cdn.cocoapods.org/'

platform :ios, '15.0'

pod 'AerisContracts', '= 0.26.0-preview.2'
pod 'Aeris/Core', '= 0.26.0-preview.2'
```

按需选择 `Aeris/UIKitContext`、`Aeris/Transports`、`AerisHost/Web`、`AerisHost/Unity`、`AerisHost/ReactNative` 或 `AerisHost/Flutter`。

RN/Flutter 插件通常由各自平台工具自动链接。使用 npm 包 `leo-urn` 时，`LeoURN` 和 `AerisRN` 由 RN 自动链接，Podfile 保留上面的源配置，不要重复声明其他来源的同名 Pod。URN 最低 iOS `15.1`，Swift 模块名为 `URN`。

## 版本

| 组件 | 当前版本 |
|---|---|
| AerisContracts / Aeris / AerisHost | `0.26.0-preview.2` |
| LeoURN | `0.2.0-preview.3` |

更新依赖后执行 `pod install`，通过生成的 `.xcworkspace` 打开应用。

## 使用说明

- [Aeris](https://github.com/zhangguozhong/aeris-sdk)
- [URN](https://github.com/zhangguozhong/leo-urn)
- [FlutterHull](https://github.com/zhangguozhong/flutter-hull)
