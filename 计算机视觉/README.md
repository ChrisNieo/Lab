## 综述
CV太火了，甚至不想打字多介绍：

#### CV领域应用分类：

· 人脸应用

· 图像文字识别 (OCR)

· 目标检测

· 目标追踪

· 实例分割和语义分割

## 学习路线
### 入门
看完基础书籍理论后，基于具体框架（Keras，Pytorch）上手简单的CV任务，对【模型、优化方法、具体任务、数据集、指标】，有初步的理解。

模型：AlexNet、VGG、ResNET、DenseNet、GoogleNet...经典模型不多说了

优化方法：BatchNormalization、各种Relu、LossFunction...这类模型中可替换、可增删、可优化的模块、层。

具体任务：模型应用的任务基于的具体领域，比如医疗、视频捕捉，会有各自大同小异的特点和模式，需要多归纳总结。

数据集：ImageNet，Cifar .... 除了使用标注好的，能直接用的数据集，会自己标注、处理数据集也是很必要的，图像批处理技术（CV2库等）也需要学习。

指标：Accuracy、F1、敏感度...不同任务、领域有各自的指标，需要多归纳总结.

在实验和读论文时多围绕上述方向思考总结~

### -----------------------------------------------------------------------------------------------------------------------------

简单的代码:

keras 猫狗识别：https://blog.csdn.net/qq_34784753/article/details/84315706

keras + yolo 目标检测：https://blog.csdn.net/sinat_26917383/article/details/85614247

keras + fasterRCNN 目标检测：https://blog.csdn.net/sinat_26917383/article/details/85614247

keras + UNET 图像分割：https://blog.csdn.net/LawenceRay/article/details/97391350?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-5.edu_weight&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-5.edu_weight

开源的CV代码太-多-了，找来读读跑跑调调，开源框架的代码模块大同小异，尝试自己修改模型架构，学会搭建自己的模型。


### 模型
各种新的经典的有亮点的厉害的CV模型

### 医疗影像
实验室CV方向主要是解决医疗领域的问题,所以医疗影像独占一栏

### 可视化
通过可视化技术,解释模型的决策过程的方法


## 大佬和其他资料

计算机视觉应该怎样入门？https://www.zhihu.com/question/23902574/answer/922634999

