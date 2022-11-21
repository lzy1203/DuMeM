# DuMeM数据标注说明
## 任务概要
一人分饰user和bot两角进行3个session的对话，session 1的内容包括但不限于user/bot的画像信息、user/bot经历的事件以及user教给bot的一些信息等，在Session 2 和 Session 3中模拟间隔一段时间后user和bot之间再次进行聊天(熟人)的场景。
![image](https://user-images.githubusercontent.com/102587634/201256893-74cdac91-8068-4b0f-8651-401f9f1c20f2.png)
### 要求
* 在Session 2 和Session 3中，Bot需要主动提及历史对话 Session 1 、或 Session 1 &Session 2中聊过的记忆信息；
* 在Session 2 和Session 3中，Bot 说的话如果涉及自身画像信息，保持与Session1 (或 Session 1& Session 2) 中历史信息(画像) 保持一致，不能矛盾冲突；
* Session 2 和Session 3需要模拟一种熟人再次聊天的场景，bot说话时需要体现bot是有记忆能力的， 通过主动提及历史信息或者根据历史内容获取的信息推进聊天的深入，来增进与user的亲密度，并让用户感觉bot很聪明，很智能。

## 对话步骤与规范
### 对话步骤
* Step 1.  输入身份ID  (跟个人微信名一致）
* Step 2.  编写session 1，至少4轮（即user和bot都至少说4句话)，聊天内容可涉及user和bot的画像信息（如姓名性别年龄等）、user/bot经历的事件、user教给bot的调教知识（详细说明见下面【名词解释】部分），等等
  * 如果灵感有限，可以参考 【起始Session灵感】 或【起始话题】，但仅供参考，不能直接复制 起始Session灵感中的内容。
* Step 3.  根据给定的【间隔时间-1】编写session 2，模拟在时间间隔-1后的利用session 1中聊过的历史信息继续聊天，至少4轮；主要是bot在聊天中主动提及历史信息，少量可以是user询问bot是否记住session 1的历史内容，bot进行回复；需体现bot对记忆内容的更新、保持、遗忘行为（详细说明见下面【名词解释】部分）；
* Step 4.  根据给定的【间隔时间-2】编写session 3，模拟在时间间隔-2后的利用session 1和session 2中聊过的历史信息继续聊天，至少4轮；历史信息利用方式同上
* Step 5. 点击【提交】， 复制记录标注id(作为工作量统计)，完成一组对话；
![image](https://user-images.githubusercontent.com/102587634/201257076-6c8263c0-61f0-4805-92e3-14d6921ebf10.png)
### 注意事项
* 不同时间间隔下的聊天，需要体现出**不同时间段后的对历史记忆不同的利用方式**(比如，session1聊到『我正在上课』，一个小时后提及这个记忆就比较好，一天后就不适合进行提及)；
* Session 1, Session 2, Session 3， **每段对话至少4轮对话，最后一句都是bot来结束**；
* 在 Session 2 和 Session 3 的标注时，需要注意：
   * <b style="color:#FF000">！！！</b> user尽量少主动提及历史信息，由bot来主动提及，体现bot的记忆性；
   * bot主动提及的位置有两个：bot在<font color=red>Session中间主动提及<font>(由user首句开始聊天，bot在聊天session中间主动提及记忆) 和  bot在**Session首句**主动提及(由bot首句开始，第一句就主动提及记忆)两种方式。
      * 主要标注**bot在Session中间**主动提及 (需要占绝大多数)；
      * 同时，如果bot在**Session首句**主动提及记忆内容时，需要第一句话提及记忆时话术要比较自然，不能太突兀(毕竟是开启新session)。
* Session 2，Session 3 在编写过程中，不能与对话历史的内容发生冲突或者重复提问，需要保持一致；
* 编写的话术要灵活自然、多样、正面、积极

## 名词解释
* 画像记忆：即个人的基本信息，可从下面的画像列表中任选维度，自己设计user和bot各自的画像信息，进行对应角色的聊天：

| 画像维度         | 画像示例 （需自定义，不要copy示例的内容）          |
| ---------- | :-----------: |
| 姓名             | 我叫小李                                           |
| 性别             | 我是女生                                           |
| 年龄             | 我22岁了                                           |
| 籍贯             | 我来自上海                                         |
| 生日             | 我生日是4月23日                                    |
| 属相             | 我属兔                                             |
| 星座             | 我是金牛座                                         |
| 身高             | 我身高168                                          |
| 体重             | 我体重48公斤                                       |
| 外形             | 我长的很可爱                                       |
| 血型             | 我是o型血                                          |
| 爸爸             | 我爸爸叫老李                                       |
| 妈妈             | 我妈妈叫小王                                       |
| 工作             | 我在百度工作                                       |
| 学历             | 我是本科学历                                       |
| 住址             | 我住在海淀                                         |
| 联系方式         | 我的电话是1111                                     |
| 社交媒体         | 我平常玩儿微博和知乎                               |
| 人际关系         | 我有两个最要好的朋友                               |
| 家族成员         | 我有一个哥哥                                       |
| 语言             | 我会说中文和英语                                   |
| 宗教             | 我没有宗教                                         |
| 性取向           | 我喜欢男生                                         |
| 价值观           | 我的价值观是越努力越幸运                           |
| 恋爱观           | 我的恋爱观是要找一个自己爱的人                     |
| 兴趣             | 我的兴趣是看电影                                   |
| 偶像             | 我的偶像是周杰伦                                   |
| 特长             | 我的特长是跳舞                                     |
| 性格             | 我是一个活泼的人                                   |
| 日常             | 我平时8点起床                                      |
| 食物             | 我喜欢吃面食                                       |
| 梦想             | 我梦想能做任何想做的事                             |
| 缺点             | 我的缺点是固执                                     |
| 优点             | 我的优点是真诚                                     |
| 不喜欢的内容     | 我特别讨厌杭州，因为美食荒漠                       |
| 不喜欢的人       | 我特别讨厌我前男友，因为他劈腿了                   |
| 不喜欢做的事     | 我特别不喜欢跪求别人，我宁可去死                   |
| 害怕的内容       | 我怕鬼片，害怕我爸爸                               |
| 害怕做的事       | 我特别害怕玩过山车                                 |
| 喜欢的内容       | 我喜欢CP感强的综艺，如果还能有我喜欢的肖战就更好了 |
| 喜欢的人         | 我喜欢对我很细心、会关心我的好看哥哥               |
| 喜欢做的事       | 我喜欢自己做咖啡                                   |
| 想去做的事       | 我想要去美国旅行                                   |
| 去过的地方       | 我去过云南                                         |
| 身体的小问题     | 我特别怕冷/我来姨妈会疼/我不吃早饭就会头晕         |
| 用户的原则、底线 | 我的底线就是一个人必须爱国                         |
| 宠物             | 我刚刚养了一只可爱的布偶猫叫猫宁                   |
| 孩子             | 我有一个三岁的女儿，学习特别好                     |
| 恋爱状况         | 我脱单了                                           |
| 昵称             | 我的小名是妮妮，英文名是micky                      |
| 毕业院校         | 我毕业于中国传媒大学                               |

* 事件记忆:  user/bot 自身过去/近期/正在/未来将  发生的一些事件信息。

| 事件 | 示例 |
| ---------- | :-----------: |
| 近期发生的事情 | 比如我最近去旅游了 |
| 正在发生的事情 | 比如我这会正在上课 |
| 以前发生的事情 | 比如我很早以前发生的一些事情 |
| 未来要发生的事情 | 比如我明天要去北京， 我今天下午4点有一个会议行程、安排等 |

* 调教知识记忆 :  user给bot指定一些画像、教bot常识、技能、时事新闻等， 比如

| 调教知识记忆 | 示例 |
|---|---|
| 指定画像类 | 比如user给bot起个名字/角色等其他画像信息、让机器人记住这个名字/角色等其他画像信息, 以后按照给定的画像信息聊天跟自己聊天等(画像信息可以参考上面54种) |
| 调教常识 | 比如教bot一些常识，比如15岁一般上初中、20多岁一般上大学等，然后在后面的聊天中测试机器人是否记住； |
| 技能类 | 比如教机器人简单的加减法、教机器人一个笑话等，然后在后面的聊天中测试机器人是否记住； |
| 时事新闻类 | 比如告诉机器人一些时势新闻，比如今天发生了什么、最近有啥热点事件，让机器人记住，然后在后面的聊天中测试机器人是否记住； |

### 记忆信息的更新、保持、遗忘
  * 记忆的更新：前面聊天历史中的画像、事件等记忆信息，如果经过一段时间后，在Session 2/3有更新，就应该对记忆做更新。比如在Session1中说自己15岁，那么选择间隔时间为：1年后，则年龄需要更新为16岁，所以在Session 2或者3 聊天中，如果是选择一年后且记忆目标中有年龄，就得体现出记忆的更新；
  * 记忆的保持：前面聊天历史中的画像、调教知识等记忆信息，如果在Session 2/3没有变化，就应该保持。比如Session 1中bot是女的，后面在session 2、3中这条信息也应该保持。
  * 记忆的遗忘：前面聊天历史中的某些事件或者其他记忆，如果觉得在后面的聊天中不重要且真实场景中不可能再被提及，那就可以选择遗忘。例如历史对话中说自己正在上课，那么间隔1个小时后，bot可以主动问用户: 你课上完了没？但假如是间隔1个月后，那就不能再问user课上完了没。这里面就涉及到有些记忆内容在不同时间间隔下的遗忘



## 标注case
<img width="613" alt="image" src="https://user-images.githubusercontent.com/102587634/203006972-a6274925-a1c3-4e0d-85fa-96fcc6ffab40.png">
<img width="613" alt="image" src="https://user-images.githubusercontent.com/102587634/203008270-ea9576ca-10af-4c74-a0dc-a888fdb4985e.png">

