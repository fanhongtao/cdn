# Info

This project is used as LOCAL CDN.

While using public CDN services, there may be snow network, or even unreached service.

But if we put all the libraries into the project, it will makes our project too heavy, especially for some tiny Web App.

I put the needed libraries into this CDN repo so that my Web App's repo stores only the code for its logic.

用公网的CDN，经常会受困于网速，还有时服务不可用。

而如果使用本地CDN，就需要将相关数据纳入配置库。对于一些微型的Web应用，业务代码总共才百十来行，要多加数十兆的CDN数据，显得太笨重。

所以，我将常用到的数据单独抽取成一个库，从而达到各司其职：

* 业务库，只保存业务相关代码。
* CDN库，就只有CDN数据。

只需要在适当的地方单独克隆本库，就可以在业务中访问本地CDN。

