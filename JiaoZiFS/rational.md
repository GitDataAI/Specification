# 我们为什么要做JiaoZiFS？

## 从谷歌说起


Booking.com is the world’s largest online travel agent where millions of guests find their accommodation and millions of accommodation providers list their properties including hotels, apartments, bed and breakfasts, guest houses, and more. During the last years we have applied Machine Learning to improve the experience of our customers and our business. While most of the Machine Learning literature focuses on the algorithmic or mathematical aspects of the field, not much has been published about how Machine Learning can deliver meaningful impact in an industrial environment where commercial gains are paramount. We conducted an analysis on about 150 successful customer facing applications of Machine Learning, developed by dozens of teams in Booking.com, exposed to hundreds of millions of users worldwide and validated through rigorous Randomized Controlled Trials. Following the phases of a Machine Learning project we describe our approach, the many challenges we found, and the lessons we learned while scaling up such a complex technology across our organization. Our main conclusion is that an iterative, hypothesis driven process, integrated with other disciplines was fundamental to build 150 successful products enabled by Machine Learning.

现在的机器学习美其名被叫成较为“科学”的方式。然而若无法有一个有效、可信赖的方法论告诉我们做了某些改变跟不做改变的差别是什么，那其实这整个过程就只是一个用复杂演算法包装的瞎蒙。


存储为何对AI至关重要 - 华尔街见闻
https://wallstreetcn.com/articles/3709991


Hidden technical debt in machine learning systems - Google Search
https://www.google.com/search?q=Hidden+technical+debt+in+machine+learning+systems&oq=Hidden+technical+debt+in+machine+learning+systems&gs_lcrp=EgZjaHJvbWUyCggAEEUYFhgeGDkyCAgBEAAYFhgeMggIAhAAGBYYHjIICAMQABgWGB4yCAgEEAAYFhgeMggIBRAAGBYYHjIGCAYQRRg8MgYIBxBFGDzSAQgxOTc3ajBqOagCALACAQ&sourceid=chrome&ie=UTF-8#ip=1

机器学习系统中隐藏的技术债务第 28 届神经信息处理系统国际会议论文集 - 第 2 卷
https://dl.acm.org/doi/10.5555/2969442.2969519

吹毛求疵的机器学习技术债务 - matthewmcateer.me
https://matthewmcateer.me/blog/machine-learning-technical-debt/

A Review on Hidden Debts in Machine Learning Systems | IEEE Conference Publication | IEEE Xplore
https://ieeexplore.ieee.org/document/8753081

Machine Learning: Hidden Technical Debts and Solutions | by Kb Pachauri | Towards Data Science
https://towardsdatascience.com/machine-learning-hidden-technical-debts-and-solutions-407724248e44

Hidden Technical Debt in Machine Learning Systems [NeurIPS 2015] | by Joanna | Medium
https://medium.com/@jchen001/hidden-technical-debt-in-machine-learning-systems-neurips-2015-5092302417b6

[2103.10510] Hidden Technical Debts for Fair Machine Learning in Financial Services
https://arxiv.org/abs/2103.10510

43146.pdf
https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43146.pdf

管理机器学习系统的技术债务|作者：约翰·梁 |走向数据科学
https://towardsdatascience.com/managing-the-technical-debts-of-machine-learning-systems-5b85d420ab9d

机器学习系统中的隐藏技术负债 (Hidden Technical Debt in Machine Learning Systems) - YouTube
https://www.youtube.com/watch?v=ReUD8ecFGCU

机器学习系统中的技术债务|作者：克里斯蒂安·卡斯特纳中等的
https://ckaestne.medium.com/technical-debt-in-machine-learning-systems-62035b82b6de

hidden technical debt in machine learning systems - Google Search
https://www.google.com/search?sca_esv=12ccb0fb0fe1b570&sxsrf=ACQVn0-8xDThssvU9dLuwkt4XQi9emeEFw:1712037180878&q=hidden+technical+debt+in+machine+learning+systems&uds=AMwkrPsv-QteW-ESt7uFcY5D8eMfB5TuM4LjWQ6JBpFRynQP0ivV2JfqddldMvMun5eCAlaM7b3W-jtLp-hGbTKRzmWWre3_UVZlqmOOxdznnxNvcoECCEIYa8hyJOMOUhkkJenZt2C3CIv2yrgZoPas9xHiBSsU-YnF4-KnuDPlJpMlvS-EQua80_LvsKCAe8PYA1lBUBpVg4Iv7p5VjvyZO6NEjxiasihGFPBUnrfyPuBp0crmmN4Ubzo3xx2cDTcdX_FL9_4UrXazNuO4OYdZ-5mUAaJaGmMUDCb_9_BBKLOKifKDwHYZ_xz25m2kIA98FVnWgbL3HPweYq8DiNWtGe6RvKDdCg&udm=2&prmd=ivnsbmtz&sa=X&sqi=2&ved=2ahUKEwjIm4jA66KFAxWHsVYBHcMmBKsQtKgLegQIExAB&biw=1812&bih=1087&dpr=2#vhid=JtQEQ4-jD7ujjM&vssid=mosaic

文章评论：谷歌机器学习系统中隐藏的技术债务
https://laszlo.substack.com/p/article-review-hidden-technical-debt

Rules of Machine Learning:  |  Google for Developers
https://developers.google.com/machine-learning/guides/rules-of-ml/?authuser=0

MLOps：机器学习中的持续交付和自动化管道 |云架构中心|谷歌云
https://cloud.google.com/architecture/mlops-continuous-delivery-and-automation-pipelines-in-machine-learning?authuser=0

The Challenges of Bringing Machine Learning to the Masses | PPT
https://www.slideshare.net/AliceZheng3/the-challenges-of-bringing-machine-learning-to-the-masses

(1) 5 Things I wish I knew before becoming a Data Scientist | LinkedIn
https://www.linkedin.com/pulse/5-things-i-wish-knew-before-becoming-data-scientist-samanvay-karambhe/

(1) GitData Labs: Company Page Admin | LinkedIn
https://www.linkedin.com/company/100954765/admin/notifications/all/

(1) Alan Ransil | LinkedIn
https://www.linkedin.com/in/alan-ransil-53573873/

(1) Feed | LinkedIn
https://www.linkedin.com/feed/

机器学习中的技术债务 |作者：Maksym Zavershynskyi |走向数据科学
https://towardsdatascience.com/technical-debt-in-machine-learning-8b0fae938657

Machine Learning in Production: From Models to Systems | by Christian Kästner | Medium
https://ckaestne.medium.com/machine-learning-in-production-from-models-to-systems-e1422ec7cd65

Christian Kästner – Medium
https://ckaestne.medium.com/

Machine Learning that Matters
https://arxiv.org/pdf/1206.4656.pdf

Designing Machine Learning System Book Note | by noplaxochia | Medium
https://medium.com/@wangdk93/designing-machine-learning-system-book-note-f68d7d475a10

Designing Machine Learning Systems - An Iterative Process for Production-Ready Applications(1).pdf - Google Drive
https://drive.google.com/file/d/1HIO9l8yScq-rLj82E9N62JqzHD53HUyq/view

Roadmap to Learn AI in 2024. A free curriculum for hackers and… | by Benedict Neo | bitgrit Data Science Publication | Feb, 2024 | Medium
https://medium.com/bitgrit-data-science-publication/a-roadmap-to-learn-ai-in-2024-cc30c6aa6e16

Machine Learning Model Serving Framework | by Abonia Sojasingarayar | Medium
https://medium.com/@abonia/machine-learning-model-serving-framework-13945633ecf3

A Guide to MLOps with Airflow and MLflow | by Yesmine Rouis | TheFork Engineering Blog | Medium
https://medium.com/thefork/a-guide-to-mlops-with-airflow-and-mlflow-e19a82901f88

Automating the ML Pipeline. This chapter discusses automating some… | by Christian Kästner | Medium
https://ckaestne.medium.com/automating-the-ml-pipeline-eb0f570b4fc9

Model Quality: Measuring Prediction Accuracy | by Christian Kästner | Medium
https://ckaestne.medium.com/model-quality-measuring-prediction-accuracy-38826216ebcb

Thinking like a Software Architect | by Christian Kästner | Medium
https://ckaestne.medium.com/thinking-like-a-software-architect-121ea6919871

Scaling Data Storage and Data Processing and Machine Learning in Production Systems | by Christian Kästner | Medium
https://ckaestne.medium.com/scaling-ml-enabled-systems-b5c6b1527bc

Versioning, Provenance, and Reproducibility in Production Machine Learning | by Christian Kästner | Medium
https://ckaestne.medium.com/versioning-provenance-and-reproducibility-in-production-machine-learning-355c48665005

seai/lectures/01_introduction/intro.md at F2022 · ckaestne/seai
https://github.com/ckaestne/seai/blob/F2022/lectures/01_introduction/intro.md

Machine Learning in Production: From Models to Products | by Christian Kästner | Medium
https://ckaestne.medium.com/machine-learning-in-production-book-overview-63be62393581

ckaestne (Christian Kästner)
https://github.com/ckaestne

Christian Kästner :: CMU
https://www.cs.cmu.edu/~ckaestne/

Hidden Technical Debt in Machine Learning Systems
https://proceedings.neurips.cc/paper_files/paper/2015/file/86df7dcfd896fcaf2674f757a2463eba-Paper.pdf

hilda_modeldb.pdf
http://people.csail.mit.edu/matei/papers/2016/hilda_modeldb.pdf

Beginning MLOps with Mlflow: Deploy Models in AWS Sagemaker, Google Cloud, and Microsoft Azure a book by Sridhar Alla and Suman Kalyan Adari
https://bookshop.org/p/books/beginning-mlops-with-mlflow-deploy-models-in-aws-sagemaker-google-cloud-and-microsoft-azure-sridhar-alla/15272424

oa.upm.es/37429/1/INVE_MEM_2014_195476.pdf
https://oa.upm.es/37429/1/INVE_MEM_2014_195476.pdf

Artificial intelligence faces reproducibility crisis | Science
https://www.science.org/doi/full/10.1126/science.359.6377.725

《模型成效》从Booking.com的150个机器学习专案学习模型上线的6个重点| by JimmyWu | Medium
https://medium.com/@jimmywu0621/%E6%A8%A1%E5%9E%8B%E6%88%90%E6%95%88-%E5%BE%9Ebooking-com%E7%9A%84150%E5%80%8B%E6%A9%9F%E5%99%A8%E5%AD%B8%E7%BF%92%E5%B0%88%E6%A1%88%E5%AD%B8%E7%BF%92%E6%A8%A1%E5%9E%8B%E4%B8%8A%E7%B7%9A%E7%9A%846%E5%80%8B%E9%87%8D%E9%BB%9E-50e25db88902

150 Successful Machine Learning Models: 6 Lessons Learned at Booking.com
https://blog.kevinhu.me/2021/04/25/25-Paper-Reading-Booking.com-Experiences/bernardi2019.pdf

X
https://twitter.com/ercwl/status/1773796070012649569

bittensor (@bittensor_) / X
https://twitter.com/bittensor_

Bittensor
https://bittensor.com/

opentensor/prompting: SN1: An incentive mechanism for internet-scale conversational intelligence
https://github.com/opentensor/prompting

JiaoziFS
https://cloud.jiaozifs.com/repositories

bug: Invalid input of repository config · Issue #158 · GitDataAI/jiaozifs-ui
https://github.com/GitDataAI/jiaozifs-ui/issues/158

bci/acc：与超级人工智能竞争的务实之路特伦特·麦康纳 | 作者：特伦特·麦康纳中等的
https://medium.com/@trentmc0/bci-acc-a-path-to-balance-ai-superintelligence-80bb6f32e39c

去中心化通用市场协议
https://www.coophive.network/

CoopHive Whitepaper
https://128082701-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FeMLzhCiCaqREpBzj5FrG%2Fuploads%2F8TI1KZ9TC985EPsuEF8k%2FCoopHive%20Whitepaper%20v1.pdf?alt=media&token=8aa93189-121a-42a8-8154-dc09730f4f25

Introduction | CoopHive
https://docs.co-ophive.network/

Whitepaper | CoopHive
https://docs.co-ophive.network/coophive/whitepaper

activeloopai/deeplake: Database for AI. Store Vectors, Images, Texts, Videos, etc. Use with LLMs/LangChain. Store, query, version, & visualize any AI data. Stream data in real-time to PyTorch/TensorFlow. https://activeloop.ai
https://github.com/activeloopai/deeplake

Activeloop | Deep Lake | Data Lake for Deep Learning
https://www.activeloop.ai/

数据布局 | v3.8.27 |深湖
https://docs.activeloop.ai/technical-details/data-layout

存储为何对AI至关重要 - 华尔街见闻
https://wallstreetcn.com/articles/3709991

What is an AI Data Pipeline? Why does Storage Matter? | Pure Storage Blog
https://blog.purestorage.com/perspectives/bytes-ai-data-lifecycle/#:~:text=To%20innovate%20and%20improve%20AI,non%2Ddisruptively%20to%20grow%20capacity

(1) Why storage matters for AI - Solidigm | LinkedIn
https://www.linkedin.com/pulse/why-storage-matters-ai-solidigm-gina-rosenthal-lhdhf/

www.backchina.com
https://www.backchina.com/blog/383112/article-384378.html

Impact-of-AI-Final.pdf
https://www.snia.org/sites/default/files/ESF/Impact-of-AI-Final.pdf

Meeting-the-Storage-Needs-of-AI-1.pdf
https://tech-prospect.com/reports/wp-content/uploads/2021/10/Meeting-the-Storage-Needs-of-AI-1.pdf

以数据为中心的AI 吴恩达 - Google Search
https://www.google.com/search?q=%E4%BB%A5%E6%95%B0%E6%8D%AE%E4%B8%BA%E4%B8%AD%E5%BF%83%E7%9A%84AI+%E5%90%B4%E6%81%A9%E8%BE%BE&sca_esv=9532ceb1aaa73555&sxsrf=ACQVn0-Q6yvuU23l9Y8h22hPOtDD6iCszg%3A1712043048721&ei=KLQLZrLSK-6m2roPzs6yyAo&ved=0ahUKEwiyhomugaOFAxVuk1YBHU6nDKkQ4dUDCBA&uact=5&oq=%E4%BB%A5%E6%95%B0%E6%8D%AE%E4%B8%BA%E4%B8%AD%E5%BF%83%E7%9A%84AI+%E5%90%B4%E6%81%A9%E8%BE%BE&gs_lp=Egxnd3Mtd2l6LXNlcnAiIeS7peaVsOaNruS4uuS4reW_g-eahEFJIOWQtOaBqei-vkgAUABYAHAAeACQAQCYAQCgAQCqAQC4AQPIAQCYAgCgAgCYAwCSBwCgBwA&sclient=gws-wiz-serp#ip=1

以数据为中心的人工智能在信号处理中的应用
https://www.matlabexpo.com/content/dam/mathworks/mathworks-dot-com/images/events/matlabexpo/cn/2022/data-centric-ai-for-signal-processing-applications.pdf

Data-Centric AI 以数据为中心的人工智能 - 知乎
https://zhuanlan.zhihu.com/p/664453370

Data-centric AI之特征工程(第一讲) | 亚马逊AWS官方博客
https://aws.amazon.com/cn/blogs/china/feature-engineering-of-the-final-version-of-data-centric-ai-lecture-1/

吴恩达：未来十年，人工智能将向以数据为中心转变_AI&大模型_Eliza Strickland_InfoQ精选文章
https://www.infoq.cn/article/8yvigg4lxce96fctjgy6

吴恩达新动作：建立全新机器学习资源Hub，「以数据为中心的AI」大本营_NeurIPS_交流_Anima
https://www.sohu.com/a/523394636_610300

New Tab
chrome://newtab/

下一代 AutoAI：从模型为中心，到数据为中心 | 雷峰网
https://www.leiphone.com/category/academic/iqFiicnCgT5OO8dS.html