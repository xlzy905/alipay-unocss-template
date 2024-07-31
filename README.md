# 支付宝小程序模版

## 简介
基于TypeScript + unocss + biome的小程序原生开发模版，使用biome格式化和校验js/ts规则

## 启动

```bash
npm i
or
pnpm i
```

## vscode插件

- 支付宝小程序开发助手
- biome

## 配置解析
```json
// mini.project.json 编译时启动unocss cli监听文件变动编译 上传时进行bulid
{
  "format": 2,
  "developOptions": {
    "hotReload": true
  },
  "compileOptions": {
    "component2": true,
    "typescript": true,
    "enableNodeModuleBabelTransform": true,
    "resolveAlias": {
      "@/*": "./*"
    }
  },
  "scripts": {
    "watch": "npm run unocss",
    "beforeUpload": "npm run unocss:build"
  }
}

```
