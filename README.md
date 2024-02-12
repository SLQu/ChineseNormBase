# Chinese Socio-cultural Norm Base
Sociocultural norms serve as guiding principles for personal conduct in social interactions, emphasizing respect, cooperation, and appropriate behavior, which is able to benefit tasks including conversational information retrieval, contextual information retrieval and retrieval-enhanced machine learning. 
We propose a scalable approach for constructing a Sociocultural Norm (SCNs) Base using Large Language Models (LLMs) for socially aware dialogues. We construct a comprehensive and publicly accessible Chinese Sociocultural NormBase ChineseNormBase.
Our approach utilizes socially-aware dialogues, enriched with contextual frames, as the primary data source. 
This enables extracting of high-quality and nuanced natural-language norm statements, leveraging the pragmatic implications of utterances with respect to the situation. 
As real dialogue annotated with gold frames are not readily available, we propose using synthetic data. 
Our empirical results show: (i) the quality of the SCNs derived from synthetic data is comparable to that from real dialogues annotated with gold frames, and (ii) the quality of the SCNs  extracted from real data, annotated with either silver (predicted) or gold frames, surpasses that without the frame annotations.
We further show the effectiveness of the extracted SCNs in a RAG-based (Retrieval-Augmented Generation) model to reason about multiple  downstream dialogue tasks. 

<div align="center">
<img src=doc/norm_extraction.png />  
<!-- <img src=doc/norm_extraction.png width=350 height=250 />   -->
</div>

# dataset
We choose SocialDial dataset as source of sociocultural frame based dialogues. SocialDial comprises a total of 6,433 instances of multi-round dialogues. We extracted relevant Scn statements based on the dialogues of SocialDial following the methodology illustrated in Figure 1.
Each dialogue underwent this extraction process twice, extracting
140,669 Scn statements
On average, each dialogue is associated with approximately 15.01 socioculture norm statements, and each socioculture norm statement appears in 1.09 dialogues on average. Furthermore, the average length of a socioculture norm statement, including punctuation, is 19.20 tokens.


# Dataset Download
You can directly download the data in our repo. And we have added "social_cultural_norms".


# todo
requirement for git
- 关于这个关于数据集的描述建议放到git那个readme的文件里
- 在paper正文这一部分的后面加上一句 For more information about the dataset, please refer to https://anonymous.4open.science/r/ChineseNormBase-7E26
- git的readme 文件里面除了放这个，再增加一些统计信息，譬如有多少种norm， formality， location，topic。。。。以及分别是什么
- 在git除了readme和json文件，再增加一个file可以叫exploratory data analysis. 里面可以放5.2的内容加上之前作为图分析的内容
- 如果可能在git页面上再加一个文件，叫provenance，大概介绍一下这个数据集是从哪个数据集抽取过来的，大概的过程是什么。简单介绍就行
关于git页面的更改你可以放到论文提交后，交完论文后有机会早点弄好
