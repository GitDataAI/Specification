# Introduction 介绍

CoopHive Whitepaper  
https://128082701-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FeMLzhCiCaqREpBzj5FrG%2Fuploads%2F8TI1KZ9TC985EPsuEF8k%2FCoopHive%20Whitepaper%20v1.pdf?alt=media&token=8aa93189-121a-42a8-8154-dc09730f4f25

In the rapidly evolving world of modern technology, the significance of distributed computing has become clear. This field, which had modest origins as the focus of a small subset of computer science research and development, is now poised to impact humanity more in the next few years than in all of computing history combined.
介绍

在快速发展的现代技术世界中，分布式计算的重要性变得越来越明显。这个领域最初只是计算机科学研究和开发的一个小子集，现在已经准备好在未来几年对人类的影响超过所有计算历史的总和。

We are at a pivotal moment in history. The emergence of generative AI marks a paradigm shift, reshaping how we utilize technology and interact with our everyday realities. The extraordinary becomes ordinary with each passing day, and we stand at the brink of a new digital renaissance.

我们正处于历史的关键时刻。生成式人工智能的出现标志着范式的转变，重塑了我们如何利用技术并与日常现实互动。随着时间的流逝，不平凡变得平凡，我们正站在新的数字复兴的边缘。

Data is the new oil, and as with all resources, it is a double-edged sword. On the one hand, imagine a world where the collective power of individuals, organizations, and their computers across the globe is harnessed to fuel generative AI systems, crafting realities beyond our wildest imaginations, freeing us from mundane labor, increasing agricultural and industrial output while simultaneously reducing environmental footprints, curing diseases, avoiding catastrophes, and a plethora of other seemingly unattainable goals.

数据是新的石油，和所有资源一样，它是一把双刃剑。一方面，想象一个世界，在这个世界上，个人、组织和他们的计算机在全球范围内的集体力量被用来推动人工智能系统，创造超出我们最疯狂想象的现实，将我们从平凡的劳动中解放出来，在增加农业和工业产出的同时减少环境足迹，治愈疾病，避免灾难，以及许多其他看似无法实现的目标。

However, the future is not necessarily so bright. Humanity is faced with vested interests, some of them companies, some of them governments, and some of them individuals, who would rather concentrate this power themselves. And this only if AI does not become cognizant and takes matter into its own hands.

然而，未来未必如此光明。人类面临着既得利益，其中一些是公司，一些是政府，还有一些是个人，他们宁愿自己集中这种权力。而这只有在人工智能没有意识到并掌握自己的情况下才会发生。

For this reason, it is necessary to have resilient infrastructures for coordinating distributed computing resources. The base of this is the actual distribution of computing work, which continues to be a developing field, and has resulted in the construction of novel and innovative distributed computing platforms like Bacalhau, a key technology in CoopHive’s stack. However, until now, most distributed computing technologies assumed that the entity submitting jobs also controlled the machines on which those jobs were being run. This excluded the possibility of utilizing idle computing resources owned by others, which are a massive, mostly untapped resource, just waiting to be unleashed. Furthermore, since these computing resources are owned by many different individuals and entities, they require a substrate on which they can coordinate and collaborate.


由于这个原因，有必要有弹性的基础设施来协调分布式计算资源。其基础是计算工作的实际分布，这是一个不断发展的领域，并导致了新型和创新的分布式计算平台的构建，如CoopHive堆栈中的关键技术Bacalhau。然而，到目前为止，大多数分布式计算技术都假定提交作业的实体也控制运行这些作业的机器。这排除了利用其他人拥有的空闲计算资源的可能性，这些资源是大量的，大部分未开发的资源，只是等待释放。此外，由于这些计算资源由许多不同的个人和实体拥有，因此它们需要一个可以在其上进行协调和协作的基础。

The nature of this problem calls out for the construction of a computational resource marketplace as its solution. CoopHive is precisely this. In its simplest description, it is a two-sided marketplace for compute that is robust, extensible, and capable of coordinating complex computational tasks.

这个问题的本质要求构建一个计算资源市场作为其解决方案。CoopHive正是如此。最简单的描述是，它是一个健壮的、可扩展的、能够协调复杂计算任务的双边计算市场。

However, CoopHive’s applications go far beyond this limited description. Artificial intelligence, zero-knowledge proofs, blockchain bridges, sensor and user data, digital twins, supply chain management, hardware profiling, privacy, compute sharing, and public goods computing are just some of the fields where CoopHive can dramatically shift the economic and computational foundations of our world. At the core of CoopHive lies deep thinking about incentives around verifiability of computational workloads, and cooperation within, and across, multi-stakeholder networks. CoopHive is not just about harnessing idle computational resources; it is about empowering a global community to contribute to and benefit from its collective computational power.


然而，CoopHive的应用程序远远超出了这个有限的描述。人工智能、零知识证明、区块链桥梁、传感器和用户数据、数字孪生、供应链管理、硬件分析、隐私、计算共享和公共产品计算只是CoopHive可以极大地改变我们世界的经济和计算基础的一些领域。CoopHive的核心在于深入思考围绕计算工作负载可验证性的激励机制，以及多方利益相关者网络内部和之间的合作。CoopHive不仅仅是利用空闲的计算资源;它是关于赋予全球社区力量，使其能够为集体计算能力做出贡献并从中受益。

# Distributed Computing Background 分布式计算背景

Distributed computing has become a critical backbone of our technological landscape, driven by the need for scalability, efficiency, and the harnessing of vast computational resources. This necessity arises from the limitations of vertically scaled monolithic systems. The demand for distributed computing is further fueled by the increasing complexity and scale of modern workloads, as well as the distributed nature of a large part of data generation.

分布式计算已经成为我们技术领域的关键支柱，它是由对可伸缩性、效率和对大量计算资源的利用的需求驱动的。这种必要性源于垂直扩展的单片系统的局限性。现代工作负载的复杂性和规模的增加，以及大部分数据生成的分布式特性，进一步推动了对分布式计算的需求。

## Why is distributed computing necessary? 为什么分布式计算是必要的?

The pivotal reason for embracing distributed computing lies in its inherent scalability and cost-effectiveness. Vertically scaling individual machines provides some gains, but costs can quickly spiral out of control; distributed execution was explored because monolithic systems were hitting real-world limitations.

采用分布式计算的关键原因在于其固有的可伸缩性和成本效益。垂直扩展单个机器提供了一些收益，但成本可能很快就会失控;分布式执行的探索是因为单片系统在现实世界中受到了限制。

Distributed execution not only offers superior scalability, but also proves to be more economically viable. Parallelism across distributed systems provides efficiency and redundancy at scale. As data is increasingly generated and stored across networks of edge devices and cloud servers, distributed computing aligns with the natural architecture of modern data distribution.

分布式执行不仅提供了优越的可伸缩性，而且在经济上也更加可行。跨分布式系统的并行性提供了大规模的效率和冗余。随着数据越来越多地在边缘设备和云服务器网络上生成和存储，分布式计算与现代数据分布的自然架构保持一致。

Further, parallelism across distributed systems provides efficiency and redundancy at scale. Workloads like training machine learning models benefit from parallel execution across clusters of commodity machines. By sharing the memory, disk, and networking throughput across many physical devices, it is possible to get significantly higher aggregate performance than all but the most expensive hardware.

此外，跨分布式系统的并行性提供了大规模的效率和冗余。像训练机器学习模型这样的工作负载受益于跨商用机器集群的并行执行。通过在许多物理设备之间共享内存、磁盘和网络吞吐量，可以获得比除了最昂贵的硬件之外的所有硬件都高得多的聚合性能。

Additionally, data is increasingly generated and stored across networks of edge devices and cloud servers. Moving all this data to a single bucket or data lake consumed an enormous amount of time and bandwidth. It makes more sense to take advantage of the distributed architecture already in place, by processing data locally, where it is generated.

此外，越来越多的数据通过边缘设备和云服务器网络生成和存储。将所有这些数据移动到单个存储桶或数据湖会消耗大量的时间和带宽。通过在数据生成的地方本地处理数据，利用现有的分布式体系结构更有意义。

## A Short History of Distributed Computing 分布式计算简史

Technology has been in pursuit of distributed workloads since the invention of the ENIAC in the 1940’s – one computer in one room is about as centralized as you can get. Mainframes became minicomputers, minicomputers became microcomputers, and microcomputers became microprocessors wired together. The ARPANet and the advent of a network created the possibility of one job, many machines.

自20世纪40年代ENIAC发明以来，技术一直在追求分布式工作负载——一个房间里的一台计算机几乎是集中式的。大型机变成了小型机，小型机变成了微型计算机，微型计算机变成了连接在一起的微处理器。阿帕网和网络的出现创造了一项工作，许多机器的可能性。

### Phase 0: The Move to Commodity Compute 阶段0:转向商品计算

The first moves towards broadly used distributed compute took off in the late 1990s, with the canonical example being the launch of commodity distributed computing with Google.

向广泛使用的分布式计算迈出的第一步是在20世纪90年代末，典型的例子是谷歌推出的商品分布式计算。

Previously, the majority of machines and deployments required vertical scaling, where increasing the amount of compute required increasingly higher costs. Beyond cost, vertical scaling often created single points of failure. If a single machine had a hardware outage (it happens!), or needed rebooting for OS upgrades, or a datacenter went offline, the entire system could fail.

以前，大多数机器和部署需要垂直扩展，其中增加计算量需要越来越高的成本。除了成本之外，垂直扩展通常会造成单点故障。如果一台机器出现硬件中断(这种情况时有发生!)，或者需要重新启动以进行操作系统升级，或者数据中心脱机，那么整个系统可能会失败。

Google, and other commodity compute users, recognized the advantages in cost, performance, and uptime when they incorporated an expectation of failure into their system design. Servers would always fail, so by spreading their services across more servers, there was a greater chance they could stay operational during an outage.

Google和其他商品计算用户在将故障预期纳入系统设计时，认识到在成本、性能和正常运行时间方面的优势。服务器总是会出现故障，因此通过将其服务分散到更多服务器上，它们在停机期间保持运行的可能性更大。

### Phase 1 - Virtualization Takes Hold 阶段1——虚拟化占据主导地位

If adding a single piece of hardware could provide improved uptime and performance, perhaps virtualizing that machine and simulating many machines would yield even further benefits. Enter virtual machines (VMs).

如果添加单个硬件可以改善正常运行时间和性能，那么虚拟化该机器并模拟许多机器可能会产生更多的好处。输入虚拟机。

Virtualizing machines enabled separation between the hardware platform and the operating system, and a new level of resource utilization. Applications could now be deployed in a defined and repeatable way to clusters of machines. Due to the virtualization of the machine, each physical machine could be much more tightly packed with applications (including redundant ones to reduce downtime). While virtualization has been around for more than half a century, its mainstream adoption really took off around the early 2000s with the introduction of VMWare ESX and GSX.

虚拟化机器支持硬件平台和操作系统之间的分离，并将资源利用率提高到一个新的水平。应用程序现在可以以一种定义好的、可重复的方式部署到机器集群中。由于对机器进行了虚拟化，每台物理机器都可以被应用程序(包括冗余的应用程序以减少停机时间)紧密地打包在一起。虽然虚拟化已经存在了半个多世纪，但随着VMWare ESX和GSX的推出，它的主流应用真正开始起飞是在21世纪初。

Virtualization was a step up from the isolated systems of the previous phase, offering better resource utilization, isolation, and load balancing. A single bad application was less likely to bring down an entire cluster, and, by abstracting away hardware, cleaner portability and configuration was possible. There were also groundbreaking new technologies such as live migration, which significantly reduced downtime due to server issues and planned upgrades. However, these VMs were still localized, limiting the true potential of distributed computing architectures. Worse, applications were often still restricted to a single machine (virtual or otherwise), limiting the ability to take advantage of the distributed topology.

虚拟化是对上一阶段孤立系统的升级，提供了更好的资源利用、隔离和负载平衡。单个错误的应用程序不太可能拖垮整个集群，而且，通过抽象硬件，更清晰的可移植性和配置成为可能。还有一些突破性的新技术，如实时迁移，可以显著减少由于服务器问题和计划升级而导致的停机时间。然而，这些虚拟机仍然是本地化的，限制了分布式计算架构的真正潜力。更糟糕的是，应用程序通常仍然局限于单个机器(虚拟或其他)，限制了利用分布式拓扑的能力。

### Phase 2 - Distribution Via Platforms 第二阶段-通过平台分发

The MapReduce paper was seminal in rethinking what an application platform could provide to simplify the concepts and utilization of distributed machines. Behind a single interface, developers could now schedule and build distributed workloads at the application level, with a limited need to dive deeper than top level structures. MapReduce inspired popular frameworks like Hadoop and Spark, and enabled massive amounts of data to be processed in parallel across a network of machines.

MapReduce论文在重新思考应用程序平台可以提供什么来简化分布式机器的概念和使用方面具有开创性意义。在单一接口背后，开发人员现在可以在应用程序级别调度和构建分布式工作负载，而不需要深入研究顶层结构。MapReduce启发了Hadoop和Spark等流行框架，并使大量数据能够在机器网络上并行处理。

Platforms like this represented a huge leap in scalability and performance, but even with this level of distribution, computing tasks were still confined to a single data center. They also required adopting a new architecture, new SDKs, and often, entire rewrites of applications, in order to take advantage of the technology.

这样的平台代表了可伸缩性和性能的巨大飞跃，但即使有了这种级别的分布，计算任务仍然局限于单个数据中心。它们还需要采用新的体系结构、新的sdk，并且经常需要完全重写应用程序，以便利用该技术。


### Phase 3 - It’s In The Clouds 第三阶段:在云端

Containerized workloads, popularized by Docker, revolutionized the way applications are developed, deployed, and managed. This revolution has been bolstered by sophisticated orchestration systems like Kubernetes and Mesosphere, enhancing orchestration and scaling to unprecedented levels. This wave of technologies, traditionally called Cloud Native Compute and rolled up into the Cloud Native Computing Foundation, has profoundly reshaped the landscape of cloud computing.

由Docker推广的容器化工作负载彻底改变了应用程序的开发、部署和管理方式。像Kubernetes和Mesosphere这样复杂的编排系统支持了这场革命，将编排和扩展提升到了前所未有的水平。这一波技术，传统上被称为云原生计算(Cloud Native Compute)，并被纳入云原生计算基金会(Cloud Native Computing Foundation)，已经深刻地重塑了云计算的格局。

These cloud-native platforms make the adoption of distributed computing technologies much more straightforward because encapsulation of applications and their dependencies have been built into the packaging. Additionally, with the declarative nature of both containers and cloud-native orchestrators, the ability to abstract jobs from underlying APIs and systems has never been easier. This allows for significantly improved utilization by dynamically moving the application to the environments that are best suited for the application and have the capacity to run it.

这些云原生平台使得分布式计算技术的采用更加直接，因为应用程序及其依赖关系的封装已经内置到封装中。此外，由于容器和云原生编排器的声明性，从底层api和系统中抽象作业的能力从未如此简单过。通过将应用程序动态移动到最适合该应用程序并有能力运行它的环境中，可以显著提高利用率。

However, despite their remarkable capabilities, most distributed computing platforms still operate primarily within a single zone or region. Although they do offer some cross-region support, being based on a centralized platform will always require significant work to support distributed and unreliable networks.

然而，尽管它们具有非凡的能力，大多数分布式计算平台仍然主要在单个区域或区域内运行。尽管它们确实提供了一些跨区域的支持，但是基于集中式平台总是需要大量的工作来支持分布式和不可靠的网络。

# Modern Challenges of Distributed Computing 分布式计算的现代挑战

Despite the significant strides made in distributed computing, modern challenges persist:

尽管在分布式计算方面取得了重大进展，但现代挑战仍然存在:

- Reliability: Loosely coupled components fail unpredictably. Lack of redundancy means few or single points of failure.
- Scaling Issues: Optimally placing computations near relevant data is difficult. Adding nodes creates bottlenecks.
- Data Locality: Jobs and queries require expensive cross-network data shuffling.
- Fault Tolerance: Partial failures can cascade, causing widespread outages.
- Slow processing: Distributed data dependencies stall workflows. Lack of parallelism wastes resources.
- Compliance risks: Sensitive data spread across systems multiplies security concerns.
- Latency: Synchronous calls between distributed modules incur delays.
- Orchestration: Deploying updates across disparate systems is complex and risky.


- 可靠性: 松散耦合的组件不可预测地失效。缺乏冗余意味着很少或单点故障。
- 缩放问题：在相关数据附近最佳地放置计算是困难的。增加节点会产生瓶颈。
- 数据局部性：作业和查询需要昂贵的跨网络数据变换。
- 容错：部分故障可以级联，导致大范围的中断。
- 处理缓慢：分布式的数据依赖关系使工作流程停滞。缺乏并行性会浪费资源。
- 合规风险：敏感数据跨系统传播会增加安全问题。延迟:分布式模块之间的同步调用会导致延迟。
- 编排：跨不同系统部署更新既复杂又有风险。

Being truly distributed means re-thinking how an application and platform interacts with the network. Reviewing the Fallacies of Distributed Computing, the fallacies listed then, three decades ago, are as true today as they have ever been:

实现真正的分布式意味着重新思考应用程序和平台如何与网络交互。回顾分布式计算的谬论，三十年前列出的谬论在今天仍然是正确的:

The network is reliable;
Latency is zero;
Bandwidth is infinite;
The network is secure;
Topology doesn't change;
There is one administrator;
Transport cost is zero;
The network is homogeneous.


网络可靠;
延迟为零;
带宽是无限的;
网络是安全的;
拓扑结构不变;
有一个管理员;
运输成本为零;
网络是同质的。

Worker nodes needing to check in with a centralized task manager, unreliable networks, widely varying latency, and challenging networking can exacerbate scheduling problems very quickly. In order to realize the dream of truly distributed computing, a robust platform needs to tackle these challenges head-on.

需要向集中式任务管理器签入的工作节点、不可靠的网络、大范围变化的延迟以及具有挑战性的网络会很快加剧调度问题。为了实现真正的分布式计算的梦想，一个健壮的平台需要直面这些挑战。


# Bacalhau

Bacalhau is a distributed computing platform designed to address these modern challenges.

Bacalhau是一个分布式计算平台，旨在解决这些现代挑战。

Bacalhau’s tenets are the following:

- Familiar - Should feel very similar to existing applications and platforms. If you use Kubernetes, Spark, Docker, Python, etc., then Bacalhau should feel like a familiar friend.
- Resilient - Supporting distributed networks means a very different approach to resilience - particularly a first-class support for a network that could disappear at any time. Bacalhau must support these kinds of topologies natively.
- Efficient - Applications can take advantage of idle compute, move jobs to where there are optimization opportunities, and observe and respond to dynamic network topologies, all without the user having to take any actions beyond detailing the requirements for their job.
- Distributed-Native - The platform should feel both familiar, and represent distributed concepts as first class elements. Targeting datasets, managing permissions, navigating multi-location shards, and many more features should be as easy as building locally. 

- 熟悉——应该感觉与现有的应用程序和平台非常相似。如果你使用Kubernetes、Spark、Docker、Python等，那么Bacalhau应该是你熟悉的朋友。
- 弹性——支持分布式网络意味着一种非常不同的弹性方法——特别是对随时可能消失的网络的一流支持。Bacalhau必须本地支持这些类型的拓扑。
- 高效——应用程序可以利用空闲计算，将作业移动到有优化机会的地方，并观察和响应动态网络拓扑，所有这些都无需用户采取任何行动，只需详细说明其作业的需求。
- 分布式原生-平台应该让人感觉熟悉，并将分布式概念表示为一流元素。定位数据集、管理权限、导航多位置碎片以及更多功能应该像本地构建一样简单。


Bacalhau, builds in the expectation that machines, applications, and networks are unreliable, and as a result yields better scaling and reliability. In the same way that:

Bacalhau，建立在机器、应用程序和网络不可靠的预期基础上，因此产生了更好的可伸缩性和可靠性。以同样的方式:


- Commodity compute allowed people to go beyond a single large machine;
- VMs allowed people to go beyond a physical cluster;
- Data clusters allowed people to go beyond clusters of VMs;
- And containers allowed people to go beyond a cluster of VMs;

- 商品计算允许人们超越单个大型机器;
- 虚拟机允许人们超越物理集群;
- 数据集群允许人们超越虚拟机集群;
- 容器允许人们超越虚拟机集群;

Bacalhau allows scaling beyond a single cloud zone to accommodate where the data and compute are located, and make truly global deployments a reality. In doing so, Bacalhau helps make cross-region compute possible.

Bacalhau允许扩展到单个云区域之外，以适应数据和计算所在的位置，并使真正的全球部署成为现实。这样做，Bacalhau有助于使跨区域计算成为可能。

Bacalhau is poised to propel distributed computing to new heights by seamlessly integrating into existing workflows, enhancing resilience, optimizing efficiency, ensuring verifiability, and embracing the inherently distributed nature of modern computational networks. As the technological landscape continues to evolve, Bacalhau stands at the forefront, offering a robust answer to the challenges that have long hindered the full realization of distributed computing's potential.

Bacalhau准备通过无缝集成到现有工作流程，增强弹性，优化效率，确保可验证性，并拥抱现代计算网络固有的分布式特性，将分布式计算推向新的高度。随着技术领域的不断发展，Bacalhau站在了最前沿，为长期以来阻碍分布式计算潜力充分实现的挑战提供了一个强有力的答案。


# Applications 应用程序

## Artificial Intelligence 人工智能

### Inference  推理

Artificial Intelligence, especially generative AI, has exploded in the past year, and interest in combining blockchain technology and AI has surged. CoopHive offers a convenient and flexible way for developers to incorporate AI inference into their workflows, as well as a user-friendly interface for the general public to access low-cost inference. However, the possibilities go far beyond AI inference.

人工智能，尤其是生成式人工智能，在过去的一年里出现了爆炸式增长，人们对区块链技术和人工智能结合的兴趣激增。CoopHive为开发人员提供了一种方便灵活的方式，将人工智能推理纳入他们的工作流程，以及一个用户友好的界面，供公众访问低成本的推理。然而，这种可能性远远超出了人工智能推理。

### Cooperative AI 协作人工智能

CoopHive enables the development of trustless, cooperative AI systems by enabling multiple autonomous agents to collaborate on complex tasks. CoopHive's shared ledger can facilitate coordination and communication among distributed AI nodes, enhancing the overall efficiency and reliability of cooperative AI. The emerging field of cooperative AI exemplifies the possibilities enabled by having a shared data structure that enables and can enforce credible commitments.

CoopHive通过使多个自主代理能够协作完成复杂任务，从而实现无需信任的协作AI系统的开发。CoopHive的共享账本可以促进分布式AI节点之间的协调和沟通，提高协作AI的整体效率和可靠性。协作人工智能这一新兴领域体现了通过共享数据结构实现并执行可信承诺所带来的可能性。

### Federated Learning 联邦学习

Federated learning is a process by which training or inference of AI models is split across many different nodes, with potentially different owners and heterogeneous hardware. While the research field dedicated to federated learning is relatively new, the industry implementations are even newer, yet have enormous potential in the coming decades. Many applications of federated learning require consensus over outputs of models and aggregation of information of those outputs - a task well suited for blockchains, and a protocol like CoopHive.

联邦学习是一个过程，通过这个过程，人工智能模型的训练或推理被分散到许多不同的节点上，这些节点可能有不同的所有者和异构的硬件。虽然致力于联邦学习的研究领域相对较新，但行业实现甚至较新，但在未来几十年内具有巨大的潜力。联邦学习的许多应用需要对模型的输出和这些输出的信息聚合达成共识——这是一项非常适合区块链和CoopHive这样的协议的任务。

### Model Verification 模型验证

CoopHive can be used to validate the integrity and provenance of AI models and ensure they have not been compromised.

CoopHive可以用来验证人工智能模型的完整性和来源，并确保它们没有被破坏。


## Zero Knowledge Proofs

The explosive growth of blockchains in the past decade has prompted and massively accelerated the research and development of zero-knowledge proofs (ZKP). ZKPs are a cryptographic way of proving that a computation was done correctly without revealing some private input called a witness. Much of the focus of ZKP development for blockchains has been focused on zk-rollups for L2s on Ethereum, privacy-preserving transactions, and the like. However, most blockchain zk-coprocessors are still in their infancy. Bacalhau already supports Filecoin data onboarding, which is the single largest use of ZKPs in the world in terms of computational power and financial payments, and has recently become a major provider of data onboarding services.

在过去的十年里，区块链的爆炸式增长推动并极大地加速了零知识证明(ZKP)的研究和发展。zkp是一种证明计算是正确完成的加密方式，而不会泄露一些称为见证人的私人输入。区块链的ZKP开发的大部分重点都集中在以太坊上的L2s的zk-rollup，隐私保护交易等。然而，大多数区块链zk协处理器仍处于起步阶段。Bacalhau已经支持Filecoin数据载入，这是世界上zkp在计算能力和金融支付方面的最大单一用途，并且最近成为数据载入服务的主要提供商。

### Developer Workflows 开发人员工作流程

CoopHive intends to support arbitrary deterministic compute, and would allow developers to more easily incorporate ZK computations into their workflows, without having to make the entirety of their computations be zk-compatible, which would incur substantial overhead. The ability to develop sophisticated computational workflows is critical to the long-term success of blockchains as a technology, and just like with AI compute, having the ability to incorporate zk-computations into computational workflows enables Web3 developers to create much more complex programs than they were able to previously.

CoopHive打算支持任意确定性计算，并允许开发人员更容易地将ZK计算合并到他们的工作流中，而不必使他们的整个计算与ZK兼容，这将产生大量的开销。开发复杂的计算工作流的能力对于区块链作为一种技术的长期成功至关重要，就像人工智能计算一样，将zk计算纳入计算工作流的能力使Web3开发人员能够创建比以前更复杂的程序。

### Marketplace Uses 市场用例

There are many applications for ZKPs within CoopHive itself. For example, compute nodes could prove their hardware capabilities in zero-knowledge without revealing sensitive details. Once privacy-preserving transactions can be easily integrated into smart contracts, payments and collateralization details can be used to keep transaction data private (although it is worth mentioning that many of the benefits here can also be accomplished with payment channels). Mediation protocols can be made privacy-preserving by having the mediating node(s) remain private, and using MPC to disassociate the outcome of the mediation protocol from the inputs of the mediating nodes.

在CoopHive本身中有许多zkp的应用程序。例如，计算节点可以在不泄露敏感细节的情况下证明其零知识硬件能力。一旦保护隐私的交易可以很容易地集成到智能合约中，支付和抵押细节就可以用来保持交易数据的私密性(尽管值得一提的是，这里的许多好处也可以通过支付渠道来实现)。通过让中介节点保持私有，并使用MPC将中介协议的结果与中介节点的输入分离，可以使中介协议保持隐私性。


### Zero-Knowledge Machine Learning 零知识机器学习

Zero-knowledge machine learning (ZKML) allows a compute node to prove that they ran a specific AI model without revealing the model weights and/or the inputs.

零知识机器学习(ZKML)允许计算节点在不透露模型权重和/或输入的情况下证明它们运行了特定的AI模型。

## Bridges 桥梁

Bridges have been the topic of much attention in the blockchain world for a number of years. Cross-chain interoperability is a challenging task, as exemplified by the many hacks of such protocols. As a distributed computing standard, Bacalhau can provide a unified codebase upon which to build bridge protocols. Likewise, since CoopHive contracts are written in Solidity, they can be deployed on any EVM-compatible chain, further enabling cross-chain interoperability. Bridges built on top of Bacalhau and CoopHive can complement existing bridge protocols, including ambitious ones like zkBridge, as well as provide a platform for developers to build their own.

多年来，桥一直是区块链世界中备受关注的话题。跨链互操作性是一项具有挑战性的任务，正如对此类协议的许多黑客攻击所证明的那样。作为一种分布式计算标准，Bacalhau可以提供一个统一的代码库，在此基础上构建桥接协议。同样，由于CoopHive合约是用Solidity编写的，因此它们可以部署在任何evm兼容的链上，从而进一步实现跨链互操作性。建立在Bacalhau和CoopHive之上的桥可以补充现有的桥协议，包括像zkBridge这样雄心勃勃的协议，同时也为开发者提供了一个平台来构建自己的桥。

### Streamlining Off-Chain Storage Streamlining 链下存储

A number of blockchains and scaling solutions do not have native storage protocols for off-chain data. Bacalhau has the native ability to take IPFS CIDs as inputs, meaning it can provide arbitrary compute over arbitrary data in a totally distributed manner.

许多区块链和扩展解决方案没有链下数据的本地存储协议。Bacalhau具有将IPFS cid作为输入的原生能力，这意味着它可以以完全分布式的方式对任意数据提供任意计算。

### Oracles 预言机

CoopHive compute nodes can act as oracles, accessing real-world data from other blockchains and triggering cross-chain actions based on the data that they read. This would allow developers to create their own custom oracle protocols, and more easily incorporate them into their software workflows.

CoopHive计算节点可以充当预言机，访问来自其他区块链的真实数据，并根据它们读取的数据触发跨链操作。这将允许开发人员创建他们自己的自定义oracle协议，并更容易地将它们合并到他们的软件工作流中。

## Sensor Data 传感器数据

### Environmental Data 环境数据

Practitioners who use diverse sensor data, such as weather, air quality, and satellite imagery, and compute over it locally, can leverage CoopHive's ability to tap into idle computing resources and GPUs. This makes it feasible to perform complex calculations swiftly, with the added assurance of blockchain security for automatic cross-checking of results for accuracy and anomalies.

使用各种传感器数据(如天气、空气质量和卫星图像)并在本地进行计算的从业者可以利用CoopHive的能力来利用闲置的计算资源和gpu。这使得快速执行复杂计算变得可行，并增加了区块链安全性的保证，可以自动交叉检查结果的准确性和异常情况。

### Drone Data 无人机数据

For instance, environmental data gathered by drones, which is critical for tracking climate change, mitigating natural disasters, and coordinating search and rescue operations, can be processed on the fly. CoopHive makes it practical to perform machine learning inference or training that was previously too costly or slow directly on the blockchain. Now, with sufficient processing power, drones can compute data locally and then send only what is needed to centralized servers or distributed ledgers. In the context of distributed ledgers, which are particularly relevant when drones have different owners, CoopHive's platform facilitates consensus on the state of observations, ensuring trust and verifiability.

例如，无人机收集的环境数据可以在飞行中处理，这些数据对于跟踪气候变化、减轻自然灾害和协调搜救行动至关重要。CoopHive可以直接在区块链上执行以前过于昂贵或缓慢的机器学习推理或训练。现在，有了足够的处理能力，无人机可以在本地计算数据，然后只将需要的数据发送到集中服务器或分布式账本。在分布式账本的背景下，当无人机拥有不同的所有者时，这一点尤为重要，CoopHive的平台促进了对观察状态的共识，确保了信任和可验证性。

### Carbon Credits 碳信用额

In a carbon credit application, data stored on the blockchain or decentralized storage systems could be employed to quantify the results of carbon sequestration projects, subsequently translating them into verifiable carbon credits. This computational capacity could also empower community currency initiatives, using CoopHive to validate land conditions through satellite imagery or monitor environmental health via IoT sensors. The resulting land cover change maps could then yield valuable insights into the success of community development efforts, thereby contributing to both climate action and community development by providing the computational backbone for Web3-based solutions.

在碳信用申请中，可以使用存储在区块链或分散存储系统上的数据来量化碳封存项目的结果，随后将其转化为可验证的碳信用。这种计算能力还可以为社区货币倡议提供支持，使用CoopHive通过卫星图像验证土地状况，或通过物联网传感器监测环境健康状况。由此产生的土地覆盖变化图可以为社区发展工作的成功提供有价值的见解，从而通过为基于web3的解决方案提供计算骨干，为气候行动和社区发展做出贡献。

### Wildlife Monitoring 野生动物监测

Sensors capturing data on wildlife movement, habitat conditions, and biodiversity can be valuable for environmental research. CoopHive can automatically coordinate and reward environmental signals related to wildlife conservation, habitat preservation, and ecological modeling, enabling the tokenization of environmental assets and progressing the incorporation of environmental damage into traditional economic flows.

捕捉野生动物运动、栖息地条件和生物多样性数据的传感器对环境研究很有价值。CoopHive可以自动协调和奖励与野生动物保护、栖息地保护和生态建模相关的环境信号，实现环境资产的代币化，并推进将环境损害纳入传统经济流。

### Agriculture and Water Resource Management 农业与水资源管理

Like with carbon credits and wildlife monitoring, CoopHive can contribute to agriculture and water resource management by analyzing data from sensors, drones, and satellites. It can help provide consensus over, and reward, different cultivation strategies, irrigation schedules, soil management strategies, reforestation initiatives, and water use as measured from water distribution systems, reservoirs, and treatment plants.

与碳信用额度和野生动物监测一样，CoopHive可以通过分析来自传感器、无人机和卫星的数据，为农业和水资源管理做出贡献。它有助于就不同的种植策略、灌溉计划、土壤管理策略、再造林计划以及从配水系统、水库和处理厂衡量的用水情况达成共识，并给予奖励。

### Weather Forecasting 天气预报

Consensus over weather data gathered from sensors, like temperature, atmospheric pressure, and wind patterns can be fed into cryptoeconomic systems that adjust their functionalities based on weather conditions.

对从传感器收集的天气数据(如温度、大气压和风的模式)的共识可以输入加密经济系统，该系统可以根据天气条件调整其功能。

### Energy Management 能源管理

Data from energy meters, smart grids, and renewable energy sources can support decentralized decision-making for energy optimization, demand forecasting, and the efficient management of power resources. In fact, as a two-sided marketplace, a modified and generalized CoopHive could also support peer-to-peer energy trading.

来自电表、智能电网和可再生能源的数据可以支持能源优化、需求预测和有效管理电力资源的分散决策。事实上，作为一个双边市场，经过改进和推广的CoopHive也可以支持点对点能源交易。

## User Data 用户数据

Most consumers today do not directly profit from their data - at best, they receive free services in return for giving up their data. While this is slowly changing due to regulation, businesses have been slow to design their profit models to enable their users to profit from their own data.

今天的大多数消费者并没有直接从他们的数据中获利——他们最多只能通过放弃数据获得免费服务。虽然由于监管的原因，这种情况正在慢慢改变，但企业在设计盈利模式、让用户从自己的数据中获利方面一直进展缓慢。

### Collaborative Filtering 协同过滤

Related to federated learning, CoopHive can orchestrate the use of mobile user data to construct collaborative filtering for recommendation algorithms. If done in a privacy-preserving way, this would allow users to benefit from their data without giving it up, and allow developers to construct recommendation products that return a portion of the revenue back to consumers, a form of data cooperatives. A natural application is for social media analytics, which can be valuable for businesses and marketers aiming to understand and engage with their audience.

与联邦学习相关，CoopHive可以编排移动用户数据的使用，为推荐算法构建协同过滤。如果以一种保护隐私的方式进行，这将允许用户在不放弃数据的情况下从他们的数据中受益，并允许开发人员构建推荐产品，将部分收入返还给消费者，这是一种数据合作的形式。社交媒体分析是一个很自然的应用，这对企业和营销人员来说很有价值，他们的目标是了解和吸引他们的受众。

### Location-Based Services 基于位置的服务

Similarly to sensor data, verifiably crowd-sourcing information in real-time opens up many possibilities in traffic control, public transport congestion, mesh networks, and many other areas. For example, there has been much research in cooperatively owned and blockchain-governed self-driving cars that substantially reduce overall costs for consumers. Combining location-based user data with sensor data, such as data coming from traffic cameras, can help significantly improve vehicle routing. Developers who want to build privacy-respecting apps related to navigation, local business recommendations, and geofencing for personalized alerts can utilize GPS and other location data from mobile devices. Likewise, they can utilize mobile network data to optimize the use of mesh networks. This includes network performance analysis, predictive maintenance, and resource allocation for improved connectivity.

与传感器数据类似，可验证的实时众包信息在交通控制、公共交通拥堵、网状网络和许多其他领域开辟了许多可能性。例如，在合作拥有和区块链管理的自动驾驶汽车方面已经有很多研究，这些研究大大降低了消费者的总体成本。将基于位置的用户数据与传感器数据(如来自交通摄像头的数据)相结合，可以显著改善车辆路线。想要构建与导航、本地商业推荐和个性化警报地理围栏相关的尊重隐私的应用程序的开发人员可以利用来自移动设备的GPS和其他位置数据。同样，他们可以利用移动网络数据来优化网状网络的使用。这包括网络性能分析、预测性维护和改善连接性的资源分配。

### Public Health 公共卫生

Aggregated and anonymized mobile user data can be valuable, especially during public health emergencies. CoopHive can enable developers to construct trustworthy, yet privacy-preserving contact tracing, contributing to tasks such as monitoring the spread of diseases and predicting outbreaks, in a verifiable and traceable manner.

汇总和匿名的移动用户数据可能很有价值，特别是在突发公共卫生事件期间。CoopHive可以使开发人员以可验证和可追溯的方式构建可信且保护隐私的接触追踪，有助于监测疾病传播和预测疫情爆发等任务。

## Digital Twins 数字双生

Digital twins are virtual representations of physical objects, processes, or systems, and are projected to become much more prevalent in the coming years, scaling to an industry in the tens of billions of dollars. CoopHive offers a unique environment for the construction and simulation of digital twins, since especially for cyber-physical systems, the network itself can be comprised of real-life counterparts of elements of the\digital twins (e.g. compute nodes, sensors, video cameras, mobile devices, cars, etc.). This integration can provide feedback loops for self-improving and self-reinforcing systems.

数字孪生是物理对象、过程或系统的虚拟表示，预计在未来几年将变得更加普遍，规模将达到数百亿美元。CoopHive为数字双胞胎的构建和模拟提供了一个独特的环境，因为特别是对于网络物理系统，网络本身可以由数字双胞胎元素的现实对应部分组成(例如计算节点，传感器，摄像机，移动设备，汽车等)。这种整合可以为自我完善和自我强化的系统提供反馈循环。

## Supply Chain 供应链

Supply chain management has long been considered a valuable use-case for blockchains. With CoopHive, the tracking of goods along the supply chain can be augmented with more sophisticated computations, such as data analytics, which brings much more value to blockchain-based tracking of goods.

长期以来，供应链管理一直被认为是区块链的一个有价值的用例。有了CoopHive，供应链上的货物跟踪可以通过更复杂的计算来增强，比如数据分析，这为基于区块链的货物跟踪带来了更多的价值。

Smart contracts enable automated and secure execution of agreements within the supply chain by facilitating trustless and transparent transactions, automating payment processes, and enforcing contractual terms.

智能合约通过促进无信任和透明的交易、自动化支付流程和执行合同条款，实现供应链内协议的自动化和安全执行。

## End-to-End Traceability 端到端的跟踪能力

The blockchain-based tamper-proof record of transactions enables end-to-end traceability of each transaction and movement of goods, ensuring provenance. This facilitates real-time inventory management, cold-chain (environmental) monitoring, and monitoring factors such as lead times, quality, and reliability. This can help users optimize supplier selection, identify potential risks, and enhance collaboration with each other to improve their supply chain resilience.

基于区块链的防篡改交易记录实现了对每笔交易和货物流动的端到端可追溯性，确保了来源。这有助于实时库存管理，冷链(环境)监控，以及监控交货时间，质量和可靠性等因素。这可以帮助用户优化供应商选择，识别潜在风险，并加强彼此之间的协作，以提高他们的供应链弹性。

## Risk Management  风险管理

Since CoopHive jobs can act like oracles, they can provide automated analysis of data related to geopolitical events, market fluctuations, and other risk factors that impact the supply chain, allowing stakeholders to implement strategies for resilience. Additionally, the constant updating of the record facilitates automatic negotiation of prices and movement of goods, where and when it is desirable.

由于CoopHive作业可以像神谕一样运作，它们可以提供与地缘政治事件、市场波动和其他影响供应链的风险因素相关的数据自动分析，从而使利益相关者能够实施弹性策略。此外，记录的不断更新促进了价格的自动谈判和货物的移动，在需要的时间和地点。

## Coordination  协调

The tamper-proof record, plus real-time data sharing, synchronization of plans, and collaborative decision-making facilitates collaborative forecasting and planning among supply chain partners. Similarly to sensor and mobile user data, processing real-time data on traffic, weather, and vehicle conditions helps to optimize delivery routes, thereby reducing transportation costs and improving on-time deliveries.

防篡改记录，加上实时数据共享、计划同步和协作决策，促进了供应链合作伙伴之间的协作预测和规划。与传感器和移动用户数据类似，处理有关交通、天气和车辆状况的实时数据有助于优化配送路线，从而降低运输成本并提高准时交货率。

## Hardware Profiling 硬件配置

Hardware profiling plays an important role in the tech and software engineering industries. CoopHive enables the creation of the largest and most robust hardware profiling database in the world, since it adds an incentivization to participate, rather than relying on volunteer contributions for the data. Such a database can be used by scientists, researchers, consumers, hardware enthusiasts, and tech companies, large and small, to better enable their purchasing choices, use their hardware more efficiently, and make more informed choices when choosing which compute nodes to select for jobs.

硬件分析在技术和软件工程行业中起着重要的作用。CoopHive能够创建世界上最大和最强大的硬件分析数据库，因为它增加了参与的激励，而不是依赖于志愿者对数据的贡献。科学家、研究人员、消费者、硬件爱好者和大大小小的技术公司都可以使用这样的数据库，以便更好地支持他们的购买选择，更有效地使用硬件，并在为工作选择哪个计算节点时做出更明智的选择。

### Performance Optimization

By analyzing hardware profiles across distributed nodes, developers can identify potential compatibility issues and optimize performance. This is beneficial for industries that require specialized hardware setups, such as scientific research, where specific configurations are needed. This information is also valuable for optimizing software applications and ensuring they meet performance expectations for embedded systems or mobile devices, where it can aid in resource management, allowing developers to optimize apps for different devices, screen sizes, and processing power.

通过分析跨分布式节点的硬件配置文件，开发人员可以识别潜在的兼容性问题并优化性能。这对于需要专门硬件设置的行业(例如需要特定配置的科学研究)是有益的。这些信息对于优化软件应用程序并确保它们满足嵌入式系统或移动设备的性能期望也很有价值，它可以帮助资源管理，允许开发人员针对不同的设备、屏幕尺寸和处理能力优化应用程序。

### Energy Efficiency 能源效率

By analyzing the energy consumption patterns of different hardware configurations, organizations can design and implement energy-efficient computing solutions. This is particularly relevant in data centers and large-scale computing environments.

通过分析不同硬件配置的能耗模式，组织可以设计和实现节能计算解决方案。这在数据中心和大规模计算环境中尤为重要。

### Gaming 游戏

In the gaming industry, an extensive hardware profiling database can help to optimize game performance and hardware purchases. Hardware data collected from highly heterogeneous gaming setups can be used to guide the development of games that deliver optimal performance on various platforms.

在游戏行业中，广泛的硬件分析数据库可以帮助优化游戏性能和硬件购买。从高度异构的游戏设置中收集的硬件数据可以用于指导在各种平台上提供最佳性能的游戏开发。

## Privacy 隐私

The issue of private computations is especially tricky in permissionless and trustless distributed computing environments. While TEEs and homomorphic encryption provide solutions to this problem, they are not fully mature technologies capable of providing the same level of efficiency and trust as centralized cloud providers. For the time being, CoopHive will optionally use symmetric/asymmetric encryption in order to assure clients that only compute providers can see their data, unless the latter decides to leak it. For coordination problems that can use local computation over local data, ZKPs can be used, as described earlier. However, CoopHive still has a number of privacy-oriented applications.

在无许可和无信任的分布式计算环境中，私有计算的问题尤其棘手。虽然tee和同态加密为这个问题提供了解决方案，但它们并不是完全成熟的技术，无法提供与集中式云提供商相同级别的效率和信任。目前，CoopHive将选择使用对称/非对称加密，以确保客户端只有计算提供商可以看到他们的数据，除非后者决定泄漏它。对于可以在本地数据上使用本地计算的协调问题，可以使用zkp，如前所述。然而，CoopHive仍然有许多面向隐私的应用程序。

### Secure Multi-Party Computation (SMPC)  安全多方计算(SMPC)

CoopHive's compute-sharing capabilities can facilitate secure multi-party computation, where parties jointly compute a function over their inputs while keeping those inputs private. MPC was discussed earlier in the context of verifiable computing, but since CoopHive can execute arbitrary computations, it can also be used for MPC.

CoopHive的计算共享功能可以促进安全的多方计算，各方根据他们的输入共同计算一个函数，同时保持这些输入的私有。前面在可验证计算的背景下讨论了MPC，但由于CoopHive可以执行任意计算，因此它也可以用于MPC。

### Private Data Markets and Data DAOs  私有数据市场和数据DAO

Like with federated learning, users can share access to their data for specific computations without revealing the raw data itself. This decentralized approach ensures privacy and gives users control over their data.

与联合学习一样，用户可以共享对特定计算的数据访问，而不会泄露原始数据本身。这种分散的方法确保了隐私，并让用户控制自己的数据。

An oft-cited example application is healthcare data. Patients can come together to form data DAOs, where they can collectively sell access to their private data without revealing it. This allows individuals and healthcare institutions to jointly analyze anonymized patient data while keeping individual records secure. Likewise, researchers working with private datasets, such as social scientists and economists, can also benefit by running computations over users’ private data without revealing anything about it.

一个经常被引用的示例应用程序是医疗保健数据。患者可以聚集在一起组成数据dao，在那里他们可以集体出售对他们私人数据的访问，而不会泄露这些数据。这允许个人和医疗机构共同分析匿名患者数据，同时保证个人记录的安全。同样，研究私人数据集的研究人员，如社会科学家和经济学家，也可以通过在不透露任何信息的情况下对用户的私人数据进行计算而受益。

### Decentralized Private Messaging  去中心化私人消息传递

CoopHive can augment protocols that support decentralized private messaging platforms with arbitrary compute, including AI inference.

CoopHive可以通过任意计算(包括AI推理)增强支持去中心化私人消息传递平台的协议。

## Compute Sharing and Cooperatives 计算共享和协作

Following up on hardware profiling, it is clear that some machines are better suited for some tasks than others. Machines can cooperate by pooling their resources in order to derive higher revenue for all, and in the case of public good computing, can balance their preferences over projects with their machines' capabilities.

在硬件分析之后，很明显，有些机器比其他机器更适合某些任务。机器可以通过集中它们的资源来合作，以便为所有人带来更高的收入，并且在公益计算的情况下，可以平衡它们对项目的偏好和它们的机器能力。

Applications include scientific research collaborations, where projects around the world can lend each other their spare computing resources, effectively forming a compute sharing cooperative. Likewise, individuals or institutions requiring large amounts of compute for rendering and animation can share their spare capacity, keeping track of their contributions on the blockchain, perhaps even creating a community token.

应用程序包括科学研究合作，世界各地的项目可以相互借用他们的备用计算资源，有效地形成一个计算共享合作社。同样，需要大量计算来渲染和动画的个人或机构可以分享他们的空闲容量，跟踪他们在区块链上的贡献，甚至可以创建一个社区令牌。

## Public Goods Computing 公共产品计算

Prior distributed computing projects such as BOINC demonstrated the popularity and feasibility of volunteer computing for scientific projects, which are effectively a public good. Early cryptocurrencies such as Gridcoin attempted to crypto-economically incentivize participation in BOINC, and while achieving many successes (for example, having among the most nodes and being the most decentralized cryptocurrencies, as well as having an organic and passionate community), did not achieve their long-term goals, including increasing participation in volunteer scientific computing. However, with modifications and improvements, the pitfalls of prior approaches can be avoided, and their original missions driven forward.

先前的分布式计算项目，如BOINC，证明了科学项目志愿计算的普及和可行性，这实际上是一种公共产品。早期的加密货币，如Gridcoin，试图以加密经济的方式激励参与BOINC，虽然取得了许多成功(例如，拥有最多的节点，成为最分散的加密货币，以及拥有一个有机和充满激情的社区)，但没有实现他们的长期目标，包括增加志愿者科学计算的参与。然而，通过修改和改进，可以避免先前方法的陷阱，并推动其原始任务向前发展。


The space of scientific projects that can benefit from CoopHive’s marketplace and coordination mechanisms is vast. To give a few examples, climate modeling and environmental simulations, drug discovery, genomic data analysis, disaster response (e.g. helping discover the structure of Covid-19’s spike protein), and astronomical data processing. To explore some of the possibilities, see BOINC’s past accomplishments.

可以从CoopHive的市场和协调机制中受益的科学项目空间是巨大的。举几个例子，气候建模和环境模拟、药物发现、基因组数据分析、灾难响应(例如帮助发现Covid-19刺突蛋白的结构)和天文数据处理。要探索一些可能性，请参阅BOINC过去的成就。


# Revenue and Profit 收入和利润

## Fee-based Model 基于收费的模式

The simplest way to generate revenue is to take a fee for every job executed by the network (which can optionally be waived for public goods projects). This has a number of advantages over launching a network token, namely that it maintains the CoopHive's chain-agnosticism, makes it clear to each L1/L2 that the project only increases demand for its native coin/token, and avoids complicated regulatory issues.

产生收入的最简单方法是对网络执行的每项工作收取费用(对于公共产品项目，可以选择免除费用)。与启动网络代币相比，这有许多优势，即它保持了CoopHive的链不可知论性，使每个L1/L2清楚地知道该项目只会增加对其原生代币/代币的需求，并避免了复杂的监管问题。

## Liquidity Providers in DeFi Protocols  DeFi协议中的流动性提供者

If the revenues from fees aren't sold or invested in some other way, an immediate way to put them to use is by providing liquidity to DeFi protocols.

如果费用收入没有出售或以其他方式投资，那么直接使用它们的方法是为DeFi协议提供流动性。

## Value Services Layers 价值服务层

As with any platform that provides compute, it is possible to build revenue-generating businesses on top of CoopHive. For example, abstracting away from users who would otherwise not use CoopHive the process of using private keys, purchasing tokens, and using those tokens to pay for services.

与任何提供计算的平台一样，在CoopHive之上建立能够产生收入的业务是可能的。例如，从那些不使用CoopHive的用户那里抽象出使用私钥、购买令牌以及使用这些令牌支付服务的过程。

随着网络的成熟，网络将积累许多不同的加密货币和代币的储备。由于之前的努力引导广泛采用，并使Bacalhau/CoopHive成为标准的分布式计算平台，资本储备和深厚的内部知识将使网络能够开始投资建立在协议之上的分布式计算项目。因此，Bacalhau/CoopHive可以为Web3创业公司提供类似的投资和服务，就像亚马逊和谷歌为使用他们平台的创业公司提供免费的计算积分一样。

社区和用户所有权

一个真正去中心化的协议将属于它的利益相关者——依赖其服务的社区和用户。因此，从长远来看，协议的所有权有必要变得广泛分散。在协议的发展过程中，这仍然提供了巨大的财务机会，但为了忠于其原则，所有权必须变得分散。

## Investing in Distributed Computing Projects  投资分布式计算项目

As the network matures, the network will accrue reserves of many different cryptocurrencies and tokens. Due to prior efforts to bootstrap widespread adoption and make Bacalhau/CoopHive the standard distributed computing platform, the capital reserves and deep in-house knowledge will enable the network to begin investing in distributed computing projects built on top of the protocol. Thus, in a manner similar to how Amazon and Google invest in, and give free computing credits to, startups which use their platforms, Bacalhau/CoopHive can provide similar investments and services to Web3 startups.

随着网络的成熟，网络将积累许多不同的加密货币和代币的储备。由于之前的努力引导广泛采用，并使Bacalhau/CoopHive成为标准的分布式计算平台，资本储备和深厚的内部知识将使网络能够开始投资建立在协议之上的分布式计算项目。因此，Bacalhau/CoopHive可以为Web3创业公司提供类似的投资和服务，就像亚马逊和谷歌为使用他们平台的创业公司提供免费的计算积分一样。

## Community and User Ownership 社区和用户所有权

A truly decentralized protocol would be owned by its stakeholders - the communities and users who rely on its services. Thus, over the long-term, it would be necessary for ownership over the protocol to become widely dispersed. This still presents a massive financial opportunity during the growth of the protocol, but in order to stay true to its principles, ownership would have to become distributed.

一个真正去中心化的协议将属于它的利益相关者——依赖其服务的社区和用户。因此，从长远来看，协议的所有权有必要变得广泛分散。在协议的发展过程中，这仍然提供了巨大的财务机会，但为了忠于其原则，所有权必须变得分散。