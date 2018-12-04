# NativeScript-Vueを始める

## グローバルにvue-cli, vue-cli-initをインストール
```
npm i -g @vue/cli @vue/cli-init
```

## プロジェクト作成
```
vue init nativescript-vue/vue-cli-template <project-name>
cd <project-name>
npm i
```

## Androidで実行
```
tns run android --bundle
```

## iOSで実行
```
tns run ios --bundle
```

## cocoapadsがない
`WARNING: CocoaPods is not installed or is not configured properly.`とでたら、
cocoapadsをグローバルにインストール
```
sudo gem install cocoapods
```

## sixがない
`WARNING: The Python 'six' package not found.`とでたら、
sixをインストール
```
sudo pip install six
```
