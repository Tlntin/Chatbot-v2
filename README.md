# 聊天机器人

聊天机器人的 PyTorch 实现。


## 依赖

- Python 3.6.8
- PyTorch 1.3.0

## 数据集

11w青云语料

## 用法

### 数据预处理
提取训练和验证样本：
```bash
$ python extract.py
$ python pre_process.py
```

### 训练
```bash
$ python train.py
```

要想可视化训练过程，在终端中运行：
```bash
$ tensorboard --logdir path_to_current_dir/logs
```

### Demo
下载 [预训练模型](https://github.com/foamliu/Scene-Classification/releases/download/v1.0/model.85-0.7657.hdf5) 然后执行:

```bash
$ python demo.py
```

下面第一行是问句（数据集），第二行是人工答句（数据集），之后一行是机器（本模型）答句（实时生成）。

<pre>

< 我还以为你喜欢黄色
= 菲菲不在的可能性，那是相当小
> 拉倒吧
< 你今天干嘛了
= 不知道呢
> 不干嘛，叫一下-
< 有，太有了他俩偷偷摸摸，亲亲我我
= 额，菲菲可不是随便亲别人的哦
> 又是亲爱的，这叫法早就落伍了
< 臭美
= 嘻嘻，爱美之心人皆有之
> 你说的什么哦？换种说法行不
< 你有屁屁吗
= 姐不但有车，还是自行的
> 你想點
< ぉかぁぅおぁ
= {face:8}好无聊哦,我都快睡着了，聊的什么呀
> 现在的生活太感性，情绪不停泛滥，身心具疲
< 傻唧唧
= 在你脸上
> 你笨蛋
< 不要嘴硬啦，抱抱
= 轻点，别抱这么大力嘛
> 轻点，别抱这么大力嘛
< 只要你懂你自己
= 去就去、反正到了我再扣你！！！
> 听不懂就算啦，只能说你笨
< 真心话大冒险
= 好呀
> 你在逃避


</pre>