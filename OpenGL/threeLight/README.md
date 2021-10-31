

画一个材质是白色的cube，再定义三个点光源，分别是红色光、绿色光、蓝色光，光源位置在cube的三个可见面的前方。用fragment shader编程实验：

**1）** **只定义漫反射光**

**2）** **只定义漫反射光和镜面反射光**

**3）** **只定义镜面反射光**

**4）** **定义漫反射光、镜面反射光，以及环境光**



![img](https://img-blog.csdnimg.cn/a01c517252d64d50be5097f18bb769af.png) 

 

 

**答：1）只定义漫反射光**

![img](https://img-blog.csdnimg.cn/4d5dd95f50a944d7be63f5a0ea6eaff5.png) 

**2)只定义镜面反射**

![img](https://img-blog.csdnimg.cn/153d9d4bc4e345cea8d459690341bc67.png)![img](https://img-blog.csdnimg.cn/32254fdda69948789337c4ef1a599a62.png)![img](https://img-blog.csdnimg.cn/05665e960cfc4dd19ed1130dc374d7ea.png) 

 **3）只定义漫反射光和镜面反射光**

![img](https://img-blog.csdnimg.cn/ea95b8b28768454d9c3eaa9ade7b8548.png) 

**4)定义漫反射光、镜面反射光，以及环境光**

![img](https://img-blog.csdnimg.cn/976343d0b8314097a990794f4e5f5ceb.png) 

Shader对应文件：

[Gitee：点击进入资源文件链接](https://gitee.com/shAdowPlusing/resource/tree/master/OpenGL/threeLight)

三个发光小立方体充当灯具： vs_colorCube.txt  、 fr_colorCube.txt

只定义漫反射光:  vs_light.txt  、  fr_threelight_pureDiffuse.txt

只定义漫反射光和镜面反射光:   vs_light.txt  、  fr_threelight_DiffuseSpecular.txt

只定义镜面反射光:     vs_light.txt  、 fr_threelight_pureSpecular.txt

漫反射光、镜面反射光，以及环境光: vs_light.txt  、  fr_threelight.txt