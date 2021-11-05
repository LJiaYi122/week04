# week04
 TCP/IP
 # week4学习的TCP/IP第一章网络基础知识笔记
## 1.计算机网络出现的背景：
1. **计算机的普及与多样化**
* 一、21世纪最伟大的发明是计算机
* 二、计算机应用：
  * 较易理解计算机设备:个人电脑、笔记本电脑、平板电脑、手机终端（智能手机）等便携设备
  * 较为隐藏的计算机设备：家用电器、音乐播放器、办公电器、汽车等设备、芯片由计算机控制
  * 计算机演变：性能逐年增强，价格逐年下降，机体规模逐渐变小
2. **从独立模式到网络互联模式**
* 一、独立模式也就是单机模式，随着不断发展，一个个计算机连接在一起，形成计算机网络，多台计算机可实现信息共享，能在两台相距较远的机器之间即时传递信息
* 二、计算机网络根据其规模可分为：WAN（广域网）、LAN（局域网）
3. **从计算机通讯到信息通讯**
* 一、私有网络：由管理员将特定的几台计算机相连在一起形成计算机网络
* 二、互联网：私有网络相互连接组成更大的私有网络————逐渐实现计算机之间的通信
4. **计算机网络的作用**
* 一、计算机网络好比一个人的神经系统。一个人身上的所有感觉都经神经传递到大脑，与之类似，世界各地的信息也通过网络传递到每个人的计算机中

## 2.计算机与网络发展的7个阶段：
1. **批处理**
* 一、所谓批处理，是指事先将用户程序和数据装入卡带或磁带，并由计算机按照一定的顺序读取，使用户所要执行的这些程序和数据能够一并批量得到处理的方式
* 二、这个时代的计算机主要用于大规模计算或处理，并不是普通人就能使用的工具
2. **分时系统**
* 一、分时系统（TSS）：指多个终端与同一个计算机连接，允许多个用户同时使用一台计算机的系统。
* 二、当时计算机造价昂贵，分时系统的产生实现了“一人一机”的目的，让用户感觉好像“完全是自己在使用一台计算机一样。”这也体现了分时系统的独占性
* 三、这个时代，小型机也随即产生，办公场所和工厂也逐渐引入计算机
3. **计算机之间的通信**
* 一、这时计算机体积趋于小型化，为了提高效率，人们开始研究计算机之间的通信的技术
* 二、计算机与计算机之间由通讯线路连接，人们可以通过此技术读取另一台计算机中的数据，从而极大地缩短了传送数据的时间
4. **计算机网络的产生**
* 一、到了80年代，一种能够互联多种计算机的网络随之诞生，它能够让各式各样的计算机相互连接，从大型的超级计算机到小型的个人电脑
* 二、窗口系统（在计算机中可以打开多个图形待处理的系统）的发明，拉进了人与网络之间的距离
5. **互联网的普及**
* 一、这时，专注于信息处理的公司和大学已为每一位员工或研究人员分配了一台计算机，形成了“一人一机”的环境
* 二、这种环境成本不菲，人们渴望连接不同厂商的计算机建立一个成本更低的网络环境，而连接异构型计算机的通信网络技术就是我们所看到的互联网技术
* 三、个人电脑在诞生之初可以说是一种单机模式的工具，而现在它则被更广泛地应用于互联网的访问。而且，无论相距多远，世界各地的人只要接入互联网，就可以通过个人电脑实现即时沟通与交流
6. **以互联网技术为中心的时代**
* 一、互联网的普及和发展对通讯领域产生了巨大的影响，许多技术都向互联网靠拢
7. **从“单纯建立连接”到“安全建立连接”**
* 一、互联网让世界各地人们通过计算机跨越国界自由连接在了一起，成为一个国家社会基础设施建设中最基础的要素之一
* 二、事物具有两面性，互联网的便捷性给人们生活带来了负面问题，计算机病毒侵害、信息泄露、网络欺诈等利用互联网的犯罪行为日益增多，所以人们不在满足与“单纯建立连接”，而是更为追求“安全建立连接”的目标
8. **手握金刚钻的TCP/IP**
* 一、互联网是由许多独立发展的网络通讯技术融合而成，使它们之间不断融合并实现统一的正是TCP/IP技术
* 二、TCP/IP是通讯协议的统称

## 3.协议：
1. **随处可见的协议**
* 一、在计算机网络与信息通信领域里，人们经常提及“协议”一词。互联网常用的具有代表性的协议有IP,TCP,HTTP等
* 二、“计算机网络体系结构”将这些网络协议进行了系统的归纳。TCP/IP就是IP,TCP,HTTP等协议的集合。可用于互联网和局域网
2. **协议的必要性**
* 一、简单来说，协议就是计算机与计算机之间通过网络实现通信时实现达成的一种“约定”
* 二、这种“约定”使那些由不同厂商的设备，不同的CPU以及不同的操作系统组成的计算机之间，只要遵循相同的协议就能够实现通信
3. **协议如同人与人的对话**
* 一、协议就好比是一种语言，两人之间谈话的协议（语言）不同，就无法将数据（所说的话）传递给对方
4. **计算机中的协议**
* 一、计算机没人智能，所以在设计计算机程序与硬件时，要充分考虑通讯过程中可能会遇到的各种异常以及对异常的处理。在实际遇到问题时，正在通讯的计算机之间也必须具备相应的设备和程序来应对异常
5. **分组交换协议**
* 一、分组交换是指将大数据分割为一个个的叫包（Packet）的较小单位进行传输的方法
* 二、这里所说的包，如同我们平常在邮局里见到的邮包。分组交换就是将大数据分装为一个个这样的邮包交给对方

## 4.协议由谁来规定：
1. **计算机通信的诞生及其标准化**
* 一、在计算机通信诞生之初，系统化和标准化并未得到重视，每家计算机厂商都出产各自的网络产品来实现计算机通信。对于协议的标准化，分层化等事宜没有特别强烈的意识
* 二、随着计算机重要性的不断提高，很多公司逐渐意识到兼容性的重要意义。人们开始着手研究使不同厂商生产的异构机型也能够互相通信的技术
2. **协议标准化**
* 一、为了实现协议的标准化，国际标准化组织（ISO）制定了一个OSI（开放式通信系统互联参考模型），本文讲解的TCP/IP协议作为互联网上的一种标准，也作为行业标准，俨然已成为全世界所广泛应用的通讯协议

## 5.协议分层与OSI参考模型：
1. **协议的分层**
* 一、OSI模型将通讯协议中必要的协议分为7层。通过这些分层，使得那些复杂的网络协议更加简单化
* 二、在分层中，每个分层都接收由它下一层所提供的特定服务，并且负责为自己的上一次提供特定的服务。上下层之间进行交互时所遵循的约定叫做“接口”，同一层之间的交互所遵循的约定叫做“协议”
2. **通过对话理解分层**
* 一、分层可以将每个分层独立使用，即使系统中某些分层发生变化，也不会波及整个系统，通过分层可以细分通讯功能
3. **OSI参考模型**
* 一、OSI参考协议是一个“模型”，它也只是对各层的作用做了一系列粗略的界定，并没有对协议和接口进行详细的定义。对学习和设计协议只起到一个引导的作用
4. **OSI参考模型中各个分层的作用**
* 一、应用层：为应用程序提供服务并规定应用层程序中通信相关的细节。包括文件传输，电子邮件，远程登录(虚拟终端)等协议
* 二、表示层：将应用处理的信息转换为适合网络传输的格式,或将来自下一层的数据转按为上层能够处理的格式。因此它主要负责数据格式的转换具体来说,就是将设备固有的数据格式转换为网络标准传输格式。不同设备对同一比特流解释的结果可能会不同。因此,使它们保持一致是这一层的主要作用
* 三、会话层：负责建立和断开通信连接（数据流动的運辑通路),以及数据的分割等数据传输相关的管理
* 四、传输层：起着可靠传输的作用。只在通信双方节点上进行处理,而无需在路由器上处理
* 五、网络层：将数据传输到目标地址。目标地址可以是多个网络通过路由器连接而成的某一个地址。因此这一层主要负责寻址和路由选择
* 六、数据链路层：负责物理层面上互连的、节点之间的通信传输。例如与1个以太网相连的2个节点之间的通信。将0、1序列划分为具有意义的数据桢传送给对端(数捆桢的生成与接收)
* 七、物理层：负责0、1比特流(0、1序列)与电压的高低、光的闪灭之间的互换

## 6.OSI参考模型通信处理举例：
1. **7层通信**
* 一、每个分层，在处理由上一层传过来的数据时可以附上当前分层的协议所必须的“首部”信息
* 二、接收端对收到的数据“首部”与“内容”的分离，再转发给上一分层，并最终将发送端的数据恢复为原状
2. **会话层以上的处理**
3. **传输层一下的处理**

## 7.传输方式的分类：
1. **面向有线连接与无线连接型**
* 一、网络与通信中可以根据其数据发送方法进行多种分类，下面我们来介绍几种。通过网络发送数据，大致可分为面向有连接与面向无连接两种类型
* 二、面向有连接型中，在发送数据之前，需要在收发主机之前连接一条通信线路。面向有连接型就好像人平常打电话，输入完对方电话号码播出之后，只有对方端拿起电话才是真正通话
* 三、面向无连接型，则不要求建立和断开连接。发送端可于任何时间发送数据，接收端则永远不知道自己会在何时从哪里接收数据，因此，接收端需要时常确认是否收到了数据。就好像邮差一样，负责处理邮件业务的营业员，不需要确认收件人的详细地址是否真的存在，也不需要确认收件人是否真的能收到包裹，只需要发件人有一个寄件地址就可以办理邮寄包裹的业务
2. **电路交换与分组交换**
* 一、目前，网络通信方式大致分为两种——电路交换和分组交换。
* 二、前者多用于过去的电话网，后者是一种较新的通信方式，TCP/IP协议就是采用了分组交换技术
* 三、在分组交换中,由分组交换机(路由器)连接通信线路
* 四、在电路交换中,计算机之间的传输速度不变
3. **根据接收端数量分类**
* 一、网络通信当中，也可以根据目标地址的个数及后续的行为对通信进行分类。如广播多播就是这种分类的产物：分为单播，广播，多播，任播
* 二、单播：比如早先的固定电话，1对1通信。
     广播：典型例子就是电视播放，将电视信号一齐发送非非特定的多个接受对象。
     多播：和广播类似，不同的是要限定某一组主机为接收端。
     任播：在特定的多台主机中选出一台作为接受端。

## 8.地址：
1. **地址的唯一性**
* 一、通讯过程中，发送端和接收端可以被视为通信主体。它们都能由一个所谓的“地址”的信息标识出来。当人们使用电话时，电话号码就相当于“地址”
* 二、一个地址必须明确地表示一个主体对象，在同一个通信网络中不允许由两个相同地址的通信主体存在，这就是地址的唯一性
2. **地址的层次性**
* 一、接收端设备可能不止一个，为此，可以对这些由多个设备组成的一组通信赋予同一个具有唯一特性的地址，当地址总数越来越多时，如何高效的从中找出通信的目标地址成为一个重要的问题。为此人们发现地址除了具有唯一性还需要具有层次性
* 二、其实电话和信件通信中就有了地址分层的概念。电话地址包含国家区号和国内区号，通信地址包含国名，省名，市名和区名等，正是有了这些层次分类才能更加快速的定位某一个地址MAC地址和IP地址在标识一个通信主体时虽然具有唯一性，但是它们当中只有IP地址具有层次性

## 9.网络的构成要素：
1. **通信媒介与数据链路**
* 一、计算机之间通过电缆相互连接，电缆有很多种，双绞线电缆，光纤电缆，同轴电缆，串行电缆等，根据数据链路（相互直连的设备之间进行通信所涉及的协议及其网络
* 二、为此，有众多介质与之对应）的不同选用的电缆类型也不尽相同，而媒介本身也可以被划分为电波，微波等不同类型的电磁波
2. **网卡**
* 一、任何一台计算机连接网络时，必须使用网卡（全称是网络接口卡）。网络接口卡（NIC）有时也被叫做网络适配器，网卡，LAN卡
3. **中继器**
* 一、中继器———是OSI模型的第一层，物理层面延长网络的设备。由电缆传来的电信号或光信号经由中继器的波形调整和放大再传给另一个电缆
* 二、中继器两端连接的是相同的通信媒介，但有的中继器也可以完成不同媒介之间的传递工作。中继器的网络距离并非无限延长，有些中继器可以提供多个端口服务。这种中继器被称作中继集线器或集线器。因此，集线器也可以看作是多口集线器，每个端口都可以成为一个中继器
4. **网桥/2层交换机**
* 一、网桥在OSI模型的第2层———数据链路层面上连接两个网络的设备，它能够识别数据链路层的数据帧并将这些数据帧临时储存于内存，再重新生成信号作为一个全新的帧转发给另一个网段
* 二、数据帧中有一个数据位叫做FCS,用以检测数据是否正确送达目的地，用以检测数据是否送达目的地。网桥通过检测这个值，将那些损坏的值丢弃。此外，网桥还能通过地址自学机制和过滤功能控制网络流量
* 三、有些网桥能够判断是否将数据报文转发给相邻的网段，这种网桥称为自学式网桥，以太网中使用的交换集线器现在基本也属于网桥的一种，交换集线器中连接电缆的每个端口都能提供类似网桥的功能
5. **路由器/3层交换机**
* 一、路由器是在OSI模型的第3层———网络层面连接两个网络，并对分组报文进行转发的设备。网桥是根据物理地址（MAC地址）进行处理，而路由器/3层交换机则是根据IP地址进行处理的。路由器可以连接到不同的数据链路
6. **4~7层交换机**
* 一、负责处理OSI模型中从传输层到数据层的数据。如果有TCP/IP分层模型，4到7层交换机就是以TCP等协议的传输层机器上面的应用层为基础，分析收发数据，并对其进行特定的处理
7. **网关**
* 一、网关是OSI模型中负责从传输层到应用层的数据进行转换和转发的设备
* 二、网关不仅转发数据还对数据进行转换，它通常会使用一个表示层或应用层网关，在两个不能进行直接通信的协议之间通信，最终实现两者之间的通信

## 10.现代网络实态：
1. **网络的构成**
* 一、高速公路的“骨干”或“核心”相当于计算机网络的中心，人们 通常选用高速路由器相互连接使之快速传递大量数据
* 二、网络中相应于高速公路出入口的部分被称为“边缘网络”，常用的设备有多功能路由器和3层交换机，高速公路出入口连接出国道，省道，从而可以直接通往市区街道对应计算机网络中连接“边缘网络”的部分叫做“接入层”或“汇聚层”
2. **互联网通信**
* 一、人们在连接互联网时，一般会选用互联网接入服务。联网之后，汇集到无线局域网路由器和最近交换器和最近交换机的通信会再次被连接到前面所提到的“接入层”，甚至还有可能通过“边缘网络”或“主干网”实现与目标地址间的通信
3. **移动通信**
* 一、手机开机就会和最近的基站发生无线通信，基站上有手机基站天线，基站本身也相当于网络的“接入层”。基站收集发通信请求被汇集到控制中心（“边缘网络”），之后会再被接入到互联通信控制中心的主干网
4. **从信息发布者的角度看网络**
* 一、网络信息传播的以往的主流做法是个人或企业自己制作网站（主页）部署到服务器中将所要发布的信息公之于众。现在，通过博客，托管主机的方式被更多人选择

































