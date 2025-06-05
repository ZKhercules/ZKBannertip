# ZKBannerTipView

一个简洁、高度可配置的 iOS 顶部弹出提示视图组件，支持成功 / 错误 / 警告三种状态，自动避让刘海，支持手势关闭、自动消失、拦截交互等。

---

![IMG_1041 HEIC](https://github.com/user-attachments/assets/2fe91409-d2d8-40a3-a679-eb972f66f09e)
![IMG_1042 HEIC](https://github.com/user-attachments/assets/50ae43ab-7889-46bf-8087-9de7bcf06a6c)



## ✨ 特性 Features

- ✅ 纯原生 UIKit 编写，无第三方依赖
- ✅ 支持横竖屏
- ✅ 三种状态支持：成功（绿）、错误（红）、警告（黄）
- ✅ 自动避让刘海区域（Safe Area）
- ✅ 支持点击背景空白区域关闭
- ✅ 支持设置自动消失时间（也可以不消失）
- ✅ 同一时刻只弹出一个提示（自动复用）
- ✅ 使用单例，节省内存开销
- ✅ 支持遮挡全屏交互，适合全局提示

---

## 📦 安装 Installation

将以下两个文件拖入你的项目中：
ZKBannerTip/

├── ZKBannerTipView.h
└── ZKBannerTipView.m


| 参数名                | 类型                | 说明                                  |
| ------------------ | ----------------- | ----------------------------------- |
| `message`          | `NSString *`      | 提示文字                                |
| `type`             | `ZKBannerTipType` | 提示类型：`.Success`、`.Error`、`.Warning` |
| `duration`         | `NSTimeInterval`  | 自动消失时间（单位秒，<= 0 表示不自动消失）            |
| `enableTapDismiss` | `BOOL`            | 是否允许点击背景空白区域关闭提示视图                  |

🛠 自定义说明
如需定制提示视图样式（字体、颜色、背景动画等），你可以直接修改 ZKBannerTipView.m 中的实现，例如：
* font 修改为粗体 / 自定义字体
* messageLabel 增加图标或 Emoji
* 修改 show 动画为弹簧动画
* 调整背景颜色为渐变等
