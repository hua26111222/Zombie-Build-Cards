# RoguelikeCards APK打包指南

## 快速打包方法（推荐）

### 方法1：HBuilderX 云打包（最简单）

1. 下载安装 **HBuilderX**：https://www.dcloud.io/hbuilderx.html
2. 打开HBuilderX，菜单：文件 → 导入 → 从本地目录导入
3. 选择本项目文件夹
4. 右键点击项目 → 发行 → 原生App-云打包
5. 选择 Android → 使用公共测试证书 → 打包

### 方法2：Android Studio 打包

需要先安装：
- JDK 17+: https://adoptium.net/
- Android SDK: https://developer.android.com/studio

安装后：
```bash
cd android
./gradlew assembleDebug
```

APK文件生成在：`android/app/build/outputs/apk/debug/app-debug.apk`

### 方法3：在线平台打包

1. 访问 https://扣钉.net 或 https://hbuilder.io/
2. 上传项目zip包
3. 等待云端打包完成

## 手机上直接运行

如果只想在手机上测试，可以：
1. 确保电脑和手机在同一WiFi网络
2. 运行 `npm run dev` 启动开发服务器
3. 在手机浏览器输入显示的地址

## 文件说明

- `index.html` - 游戏入口文件
- `game.html` - 游戏主文件
- `manifest.json` - PWA配置文件
