# Chinese Socio-cultural Norm Base

Social norms are guiding principles for personal conduct in social interactions, emphasizing respect, cooperation, and appropriate behavior, crucially contributing to healthy relationships, effective communication, and individual social integration. This paper proposes a novel framework for extracting Chinese social-cultural norms and constructs the first publicly accessible Chinese Social-Culture Norm Base (ChineseNormBase). We employ socially-aware dialogues enriched with essential meta-information as the primary data source for our framework. These dialogues are input into a prompt incorporating dialogue content and ontology information. With the prompt, the GPT-3 model is able to generate high-quality social-cultural norms. Additionally, comprehensive experiments have been conducted to showcase the practical utility of our dataset as a supplementary source of knowledge, particularly for dialogues-related tasks. Moreover, we outline how our knowledge base is transformed into a bipartite graph, revealing latent yet significant structural insights. 



# dataset
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
