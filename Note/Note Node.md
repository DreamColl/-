# Note node

##### 1. [关于Node.js的__dirname，__filename，process.cwd()，./文件路径的一些坑](https://segmentfault.com/a/1190000009368204)

```
__dirname: 总是返回被执行的 js 所在文件夹的绝对路径
__filename: 总是返回被执行的 js 的绝对路径
process.cwd(): 总是返回运行 node 命令时所在的文件夹的绝对路径
./: 跟 process.cwd() 一样，返回 node 命令时所在的文件夹的绝对路径

require(./)和__dirname 的效果相同
```

##### 2.AMD, CMD, module.exports, export,CommonJS

```
AMD 提前执行（依赖前置）requireJs
CMD 延迟执行（依赖就近）seajs
ES6 Modules
```



##### 3.Install mongodb

```
sudo mkdir -p /data/db
sudo chown -R $USER /data/db
```

