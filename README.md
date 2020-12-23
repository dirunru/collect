# collect
### 微信收藏学习技巧总结
### 把Webpack 配置为禁用预取和预加载，这样就可以针对每个函数单独执行此类操作。在根文件夹中创建一个 vue.config.js 文件并添加禁用预取和预加载的相关配置
       module.exports = {
          chainWebpack: (config) => {
              // 禁用预取和预加载
              config.plugins.delete('prefetch')
              config.plugins.delete('preload')
          },
        }  
