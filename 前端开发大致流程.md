### 前端开发大致流程
## 克隆代码库
获得项目结构


## 安装依赖 
npm install 
npm install ** --save-dev  局部安装

## 运行项目
npm run dev 

## 打包项目
npm run build
打包前注意查看配置信息，如是测试环境还是正式环境：
1. 查看 config -- index.js 里面的 assetsPublicPath路径k

* assetsPublicPath: '/oss/',    // 根目录创建 oss 文件夹(img,js,css) 测试环境
* assetsPublicPath: 'https://ykdstatic.52dd.cn/oss/',   // 正式环境
* assetsPublicPath: 'https://ykdstatic.52dd.cn/oss/wnl/',   // 正式环境 wnl* assetsPublicPath: 'https://ykdstatic.52dd.cn/oss/',   // 正式环境 52dd

2. 查看 src -- api -- index.js 里面的配置API接口地址 root 的值

###### 配置API接口地址
* var root = 'http://apitest.52dd.cn/'   // 测试环境
* var root = 'https://api.52dd.cn/'   // 正式环境

## 开发完成后的测试
1. 优先本地测试
2. 打包测试优先打包测试环境
3. 测试环境测试通过后打包各渠道正式环境分别测试
4. 以上测试都通过后可以告诉产品自测验证，通过后再正式提测


