### example
#### 使用方法
```
# 开启打包
npm run start

```

#### 作用
组件开发环境，实现开发环境实时打包，并自动添加到 example的 node_modules中

#### 搭建过程
```
# 初始化 package

npm init -y

# 初始化 react项目依赖

npm install -S react react-dom

# babel 配置 (注意版本，各个依赖版本不匹配，无法正常运行)
npm install -D @babel/core @babel/plugin-transform-runtime @babel/preset-env babel-loader @babel/preset-react

# 配置 .babelrc.json
    {
        "presets": [
            "@babel/preset-env",
            "@babel/react"
        ],
        "plugins": [
            "@babel/plugin-transform-runtime"
        ]
    }

# 支持 css\less
npm i -D css-loader style-loader less-loader less

# 

```