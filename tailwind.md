# 安装
> https://tailwindcss.com/docs/installation

# Tailwind CSS IntelliSense
在 VS CODE中安装`Tailwind CSS IntelliSense`插件

# YouTube教程1
> https://www.youtube.com/watch?v=qmMIz0_c9Ek

新建一个文件夹  -> 里面再建一个`assets`

`npm init -y`

`npm install -D tailwindcss`

 > [`npx tailwindcss init`](https://tailwindcss.com/docs/installation)

```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["*.{html,js}"],   //重点
  theme: {
    extend: {},
  },
  plugins: [],
}
```

根目录建一个`css`文件夹->建一个`input.css`，copy如下：
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```


package.json里面：
```
{
  "name": "2",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "build": "tailwindcss -i .css"   //重点
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "tailwindcss": "^3.4.14"
  }
}

```
