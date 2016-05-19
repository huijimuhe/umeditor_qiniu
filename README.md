# umeditor_qiniu
umeditor1.2.2版本上传图片至七牛，目前只支持单图上传。

![](https://github.com/huijimuhe/umeditor_qiniu/blob/master/screenshot/1.png)

##用法

在Qiniu_upload.class.php中将ak、sk、bucket、domain参数改为自己的即可。

````

    //QINIU_ACCESS_KEY
    public $ak = 'KUN6xYZlOAtid2MjHm90-6VFY2M7HC90ijDH4uOR';
    //$QINIU_SECRET_KEY
    public $sk = 'D-K57TE5hPe3krexftxLWFKmL2xbQEKA-mtkrUfB';
    //配置bucket为你的bucket
    public $bucket = "gitwiduu";
    //配置你的域名访问地址
    public $domain = "http://gitwiduu.u.qiniudn.com";

````

##umeditor更改的地方

因为umeditor1.2.2这一版本默认会图片添加根地址，所以需要修改。修改的位置在/dialogs/image/image.js ，已修改。

````

	var $img = $("<img src='" +  url + "' class='edui-image-pic' />")

````

另外把网络地址发布给注释掉了，只允许单图上传
##说明

Apache License

项目修改自

**https://github.com/fex-team/umeditor**

**https://github.com/widuu/qiniu_ueditor_1.4.3**

