# OpenDomainDialogCorpus_CN
Open domain Chinese dialogue corpus and datasets.

根据一些论文和其他repo收录整理了若干中文开放域对话数据集，仅供学习交流使用。<br>

<table class="docutils">
<tbody>
  <th width="80"> 数据集 </th><th width="80"> 描述 </th><th width="100"> 单轮/多轮 </th><th width="250"> 格式 </th><th width="250"> 规模 </th><th width="60"> 年份 </th><th width="120"> 提出论文 </th><th width="80"> 相关地址 </th>
  
  <tr><td> Douban Conversaion Corpus </td><td> 来自豆瓣数据，常用 </td><td> 多轮 </td><td><details><summary> 点我 </summary> test集合包含1000组数据，每组数据由10个labeled context-response pair构成，10个数据标签可能均为0，可能具有多个（2-3）标签为1的数据。所有文本为已分词格式。 </details></td><td> <img src=https://github.com/Aman-4-Real/OpenDomainDialogCorpus_CN/blob/main/pics/douban.png width="300px" /> </td><td> 2017 </td><td><details><summary> 点我 </summary> Sequential Matching Network: A New Architecture for Multi-turn Response Selection in Retrieval-Based Chatbots. Yu Wu, Wei Wu, Chen Xing, Ming Zhou, Zhoujun Li. ACL 2017. </details></td><td> <a href="https://github.com/MarkWuNLP/MultiTurnResponseSelection" target="_blank">Here</a> </td></tr>
  
  <tr><td> Noah NRM Data / STC@NTCIR13 </td><td> 来自微博，常用 </td><td> 单轮 </td><td><details><summary> 点我 </summary> 相关下载链接已失效。找到的 NTCIR13 数据集中，训练集v1.0为excel表格，包含11535个query-response pair（768个unique query），分别带有差(-1)中(0)好(1)的来自三个judge的标签，需要自行对齐标签预处理。</details></td><td> 4,435,959 Pairs / post 219,905 / responses 4,308,211 / 平均每个post，20条response </td><td> 2015 </td><td><details><summary> 点我 </summary> Neural Responding Machine for Short-Text Conversation. Lifeng Shang, Zhengdong Lu, and Hang Li. ACL 2015. </details></td><td> <a href="https://gist.github.com/AndrewShang/8a14e78f5eb03a0fb91248540041cc7d#file-gistfile1-txt" target="_blank">Here</a>，更推荐<a href="https://github.com/codemayq/chinese_chatbot_corpus" target="_blank">后者</a> </td></tr>
  
  <tr><td> STC Data </td><td> 来自微博，常用 </td><td> 单轮 </td><td><details><summary> 点我 </summary> post 和 response 的 id 相对应，1个post30个response，需要自行预处理得到对应文本。带有1，2的标注，分别表示恰当和一般。 </details></td><td> 
Retrieval_Repository<br>
    #posts              38,016<br>
    #responses          618,104<br>
    #original_pairs     618,104<br>
Labeled_Data<br>
    #posts              422<br>
    #responses          12,402<br>
    #labeled_pairs      12,402<br>
 </td><td> 2013 </td><td><details><summary> 点我 </summary> A Dataset for Research on Short-Text Conversation. Hao Wang, Zhengdong Lu, Hang Li, Enhong Chen. EMNLP 2013. </details></td><td> <a href="http://data.noahlab.com.hk/conversation/" target="_blank">Here</a> </td></tr>

  <tr><td> LCCC </td><td> 主要微博，混合（见论文P4） </td><td> 多轮 </td><td><details><summary> 点我 </summary> json文件可以直接读取，需要自己构造正负例，单个session轮数较少 </details></td><td> <img src=https://github.com/Aman-4-Real/OpenDomainDialogCorpus_CN/blob/main/pics/lccc.png width="300px" /> </td><td> 2020 </td><td><details><summary> 点我 </summary> A large-scale chinese short-text conversation dataset. Wang Y, Ke P, Zheng Y, et al. NLPCC 2020. </details></td><td> <a href="https://github.com/thu-coai/CDial-GPT#Dataset-zh" target="_blank">Here</a> </td></tr>
  
  <tr><td> PchatbotW </td><td> 来自微博 </td><td> 单轮 </td><td><details><summary> 点我 </summary> 50G的 PchatbotW.release_ver 文本文件，直接读取，包含 5,319,596 个 posts 和 139,448,339 个 responses，需要自己构造检索子数据集。 </details></td><td> <img src=https://github.com/Aman-4-Real/OpenDomainDialogCorpus_CN/blob/main/pics/pchatbotw.png width="300px" /> </td><td> 2020 </td><td><details><summary> 点我 </summary> A large-scale chinese short-text conversation dataset. Wang Y, Ke P, Zheng Y, et al. NLPCC 2020. </details></td><td> <a href="https://github.com/thu-coai/CDial-GPT#Dataset-zh" target="_blank">Here</a> </td></tr>
  
  <tr><td> RRS </td><td> 根据 <a href="https://aclanthology.org/D19-1191/">Restoration200K</a> 数据集构建 </td><td> 多轮 </td><td><details><summary> 点我 </summary> 1000个sessions，每个10个candidates包含1个正例9个负例。txt文件直接读取处理即可。 </details></td><td> <img src=https://github.com/Aman-4-Real/OpenDomainDialogCorpus_CN/blob/main/pics/rrs.png width="300px" /> </td><td> 2021 </td><td><details><summary> 点我 </summary> Exploring Dense Retrieval for Dialogue Response Selection[J]. Lan T, Cai D, Wang Y, et al. arXiv preprint arXiv:2110.06612, 2021. </details></td><td> <a href="https://github.com/gmftbyGMFTBY/SimpleReDial-v1" target="_blank">Here</a> </td></tr>
  
  <tr><td> 小黄鸡 </td><td> 原人人网项目语料 </td><td> 单轮 </td><td><details><summary> 点我 </summary> 包含分词和未分词版本，需要预处理 </details></td><td> ~45w </td><td> / </td><td> / </td><td> <a href="https://github.com/aceimnorstuvwxz/dgk_lost_conv/tree/master/results" target="_blank">Here</a> </td></tr>
  
  <tr><td> 青云语料 </td><td> 来自聊天机器人交流群 </td><td> 单轮 </td><td><details><summary> 点我 </summary> csv文件，post和resp用 '|' 分隔，需要预处理 </details></td><td> ~11w </td><td> / </td><td> / </td><td> <a href="https://github.com/codemayq/chinese_chatbot_corpus" target="_blank">Here</a> </td></tr>
  
  <tr><td> 贴吧语料 </td><td> 来自贴吧回帖 </td><td> 多轮 </td><td><details><summary> 点我 </summary> 文本文件，post和resp用 \t 分隔，包含305w个单轮，需要自己恢复成多轮和构造对应数据 </details></td><td> ~305w (单轮) </td><td> / </td><td> / </td><td> <a href="https://github.com/codemayq/chinese_chatbot_corpus" target="_blank">Here</a> </td></tr>
  
</tbody></table>

<br><br>

**References & Useful Links**:

[1] <a href="https://ai.tencent.com/ailab/nlp/dialogue/#datasets">Dialogue Research-Tencent AI Lab</a><br>
[2] <a href="https://ai.baidu.com/broad/introduction">Baidu AI Dataset</a><br>
[3] <a href="https://docs.google.com/spreadsheets/d/1SJ4XV6NIEl_ReF1odYBRXs0q6mTkedoygY3kLMPjcP8/pubhtml">Dialogue datasets</a><br>
[4] <a href="https://github.com/candlewill/Dialog_Corpus">candlewill/Dialog_Corpus</a><br>
[5] <a href="https://github.com/codemayq/chinese_chatbot_corpus">codemayq/chinese_chatbot_corpus</a><br>
[6] <a href="https://github.com/EVASHINJI/Dialog-Datasets">EVASHINJI/Dialog-Datasets</a><br>
[7] <a href="https://github.com/EVASHINJI/Dialog-Datasets">EVASHINJI/Dialog-Datasets</a><br>

ENJOY.





