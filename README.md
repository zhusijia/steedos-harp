# website

> Website for SteedOS Apps. use Harp

## 1.Install Harp

### On OS X and Linux

    sudo npm install -g harp

### On Windows

    npm install -g harp

## 2.Init a project

    harp init myproj

## 3.Start local web server

    打开cmd,cd到[项目文件]的上级目录

    输入：harp server [项目文件]
    
    服务启动在：http://localhost:9000

## 4.编译发布

    打开cmd,cd到[项目文件]的上级目录

    输入：harp compile [项目文件]
    
    编译完成后，会在项目文件的根目录下生成一个www文件，用于存放编译后的静态网页

## 5.注意事项

- help文件夹固定路径为/cn/help，不可以更改。
- `<%- current.path %>`获取当前显示网页的路径[Array]，`<%- current.source %>`获取当前显示网页的文件名[String]。
- `_harp.json`文件用于设置网页默认的title和description，该文件放在项目根目录， `_data.json`文件用于设置单独网页的title和description，该文件放在需要单独设置的网页的目录下。网页引用title和descritpion的方式：`<title><%= title %></title>`，`<meta name="description" content="<%= description %>" />`

关于harp的更多文档可以参见官网，[harp]:http://harpjs.com/docs/

