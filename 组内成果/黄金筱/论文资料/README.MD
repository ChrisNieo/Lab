1. 论文用英语写的，有部分章节的中文版。因为不需要纠结真正的算法细节，所以大概看懂整体框架就可以。
2. 一共有两个数据集eclipse和gnome，用前缀区分，怕你混淆先给你一个数据集eclipse。
3. 论文整体目标：通过bug的文本信息和bug的修复路径（结构信息），对于新的bug，预测这个bug将被哪个节点修复。
4. 我的问题：希望可以用深度学习的方法在已有的网络上得到每个节点对应的向量表示。

数据集：
网络信息：
1. 数据集/bug_path/ee_tw.edges：无列名，共有4列，空格符号分割。每列含义：层号 起始节点 目标节点 权重
    解释一下：社交网络有两层，分别是email层和tossing层，email层表示从起始节点发一个邮件到目标节点，tossing层表示从起始节点抛一个bug到目标节点，权重表示行动（发邮件 or 抛bug）的次数。
2. 数据集/bug_path/eclipse_bugid_tossers_fixers.csv：有列名，共有3列，“,”分割。每列含义：bug的唯一标识，bug经过的节点，bug的修复者。“bug经过的节点”和“bug的修复者”是bug修复的整个路径，如第一条记录，228057号bug从27号节点开始，经过63号，最后被264号修复。如果tossers和fixers编号相同，则表示bug直接被tossers修复。

文本信息：
1. 数据集/bug_text/eclipse_class.txt：预测标签，也就是bug的分类，每个数字表示一类
2. 数据集/bug_text/eclipse_train.txt：训练集，无列名，共2列，tab分割。每列含义：bug的文本	bug被哪个节点修复（bug文本对应的class，即预测标签）
3. 数据集/bug_text/eclipse_test.txt：测试集
4. 数据集/bug_text/eclipse_dev.txt：验证集
