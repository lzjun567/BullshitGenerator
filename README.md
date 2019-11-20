# 狗屁不通文章生成器

本项目是从原作者@menzi11的项目中衍生过来的，本代码更加简洁，总代码不到10行。

### 用途

狗屁不通文章生成器仅用在凑字数等非正式场景


### 实现原理


显示准备好data.json 素材,里面的结构是字典



```python
{
    "famous":[
    "爱迪生a，天才是百分之一的勤奋加百分之九十九的汗水。b",
    "查尔斯·史a，一个人几乎可以在任何他怀有无限热忱的事情上成功。b",
    ....
    ],
    "bosh":[
    "现在, 解决x的问题, 是非常非常重要的. 所以, ",
    "我们不得不面对一个非常尴尬的事实, 那就是, ",
    ....
    ],
    "after":[
    "这不禁令我深思. ",
    "带着这句话, 我们还要更加慎重的审视这个问题: ",
   ....

    ],
    "before":[
    "曾经说过",
    "在不经意间这样说过",
    ....
    ]
}
```


famous 是名人语录, 里面的关键字"a"和"b" 将分别被 before 和 after 中的内容替换,这样是的句子具有逻辑性.bosh 是一句废话, 关键字"x"将用标题替换.

一篇文章的构成就是不断随机区famous和bosh列表的元素,最后拼接成一篇文章.





### 如何使用

```
from bullshit import generator
content = generator("我爱Python")
print(content)
```
输出

```
一般来说, 问题的关键究竟为何? 既然如何,
对我个人而言，我爱Python不仅仅是一个重大的事件，还可能会改变我的人生.
我爱Python, 到底应该如何实现. 生活中, 若我爱Python出现了, 我们就不得不考虑它出现了的事实. 从这个角度来看, 易卜生说过一句富有哲理的话, 伟大的事业，需要决心，能力，组织和责任感。我希望诸位也能好好地体会这句话. 我们不妨可以这样来想: 我们不妨可以这样来想: 奥斯特洛夫斯基曾经提到过, 共同的事业，共同的斗争，可以使人们产生忍受一切的力量。　这不禁令我深思. 在这种困难的抉择下, 本人思来想去, 寝食难安.问题的关键究竟为何? 带着这些问题, 我们来审视一下我爱Python. 我爱Python似乎是一种巧合，但如果我们从一个更大的角度看待问题，这似乎是一种不可避免的事实.
现在, 解决我爱Python的问题, 是非常非常重要的. 所以, 对我个人而言，我爱Python不仅仅是一个重大的事件，还可能会改变我的人生. 现在, 解决我爱Python的问题, 是非常非常重要的. 所以,

这样看来, 在这种不可避免的冲突下，我们必须解决这个问题. 既然如何, 要想清楚, 我爱Python, 到底是一种怎么样的存在. 既然如此, 总结的来说, 经过上述讨论, 我爱Python因何而发生?总结的来说, 就我个人来说, 我爱Python对我的意义, 不能不说非常重大. 而这些并不是完全重要, 更加重要的问题是, 问题的关键究竟为何? 笛卡儿曾经提到过, 我的努力求学没有得到别的好处，只不过是愈来愈发觉自己的无知。这句话语虽然很短, 但令我浮想联翩. 我认为, 我爱Python, 发生了会如何, 不发生又会如何. 经过上述讨论,
在这种困难的抉择下, 本人思来想去, 寝食难安.我爱Python, 到底应该如何实现. 我爱Python, 到底应该如何实现.

```

指定内容长度

```
content = generator("我爱Python", length=1000)
print(content)
```

输出
```
要想清楚, 我爱Python, 到底是一种怎么样的存在. 我们都知道, 只要有意义, 那么就必须慎重考虑.了解清楚我爱Python到底是一种怎么样的存在, 是解决一切问题的关键.
从这个角度来看, 一般来说, 带着这些问题, 我们来审视一下我爱Python. 我们不得不面对一个非常尴尬的事实, 那就是, 吉姆·罗恩在不经意间这样说过, 要么你主宰生活，要么你被生活主宰。这句话把我们带到了一个新的维度去思考这个问题: 我爱Python, 到底应该如何实现. 每个人都不得不面对这些问题.  在面对这种问题时, 问题的关键究竟为何? 可是，即使是这样，我爱Python的出现仍然代表了一定的意义. 我们一般认为, 抓住了问题的关键, 其他一切则会迎刃而解.了解清楚我爱Python到底是一种怎么样的存在, 是解决一切问题的关键.我认为, 了解清楚我爱Python到底是一种怎么样的存在, 是解决一切问题的关键.我爱Python, 到底应该如何实现. 我爱Python的发生, 到底需要如何做到, 不我爱Python的发生, 又会如何产生. 现在, 解决我爱Python的问题, 是非常非常重要的. 所以, 我们不妨可以这样来想: 现在, 解决我爱Python的问题, 是非常非常重要的. 所以, 我爱Python, 到底应该如何实现. 马克思说过一句富有哲理的话, 一切节省，归根到底都归结为时间的节省。这启发了我. 我们不妨可以这样来想: 我爱Python似乎是一种巧合，但如果我们从一个更大的角度看待问题，这似乎是一种不可避免的事实. 问题的关键究竟为何? 歌德曾经说过一句富有哲理的话，流水在碰到底处时才会释放活力。带着这句话, 我们还要更加慎重的审视这个问题: 我们不得不面对一个非常尴尬的事实, 那就是, 我们不得不面对一个非常尴尬的事实, 那就是, 我爱Python, 到底应该如何实现. 一般来讲, 我们都必须务必慎重的考虑考虑. 我们都知道, 只要有意义, 那么就必须慎重考虑.总结的来说,
我们一般认为, 抓住了问题的关键, 其他一切则会迎刃而解.
这种事实对本人来说意义重大, 相信对这个世界也是有一定意义的.既然如何, 就我个人来说, 我爱Python对我的意义, 不能不说非常重大. 我爱Python, 发生了会如何, 不发生又会如何. 莎士比亚说过一句著名的话, 意志命运往往背道而驰，决心到最后会全部推倒。这句话语虽然很短, 但令我浮想联翩.

```