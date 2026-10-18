# 24维分类完善 v7

对照本地Benchmark Radar目录，维度覆盖从14项扩展到21项。成绩仍为23326条；仅更新分类，不增加或改写分数与日期。

覆盖包含部分匹配，不能视为24维已完全评测。分类证据来自项目描述与显式任务规则，来源数值证据等级不随分类升级。MMLU等总分仍不拆成医学、法律等分科分数。

|一级指标|二级指标|记录数|benchmark标签数|例子|
|---|---|---|---|---|
|大语言模型|医学知识|48|8|DermMCQA、HealthBench、HealthBench Consensus、HealthBench Hard、HealthBench Professional、MedXpertQA、PathMCQA、healthbench|
|大语言模型|工程与技术|3927|33|Aider-Polyglot、BigCodeBench、CodeForces、HumanEval、HumanEval Plus、HumanEval+、HumanEval-Mul、Humaneval|
|大语言模型|推理能力|6560|106|AIME、AIME 2024、AIME 2025、AIME 2026、ARC-AGI、ARC-AGI v2、ARC-AGI-3、ARC-C|
|大语言模型|教育与心理学|11|2|EQ-Bench、Social IQa|
|大语言模型|数学与定量计算能力|3469|45|AIME、AIME 2024、AIME 2025、AIME 2026、ArXivMath、Beyond AIME、FrontierMath、FrontierMath Tier 4 (v2)|
|大语言模型|法律与知识产权|54|6|Harvey LAB (Vals)、Harvey LAB-AA、Legal Agent Benchmark、PLawBench、PRBench-Legal、Uniform Bar Exam|
|大语言模型|自然科学|2067|30|ARC-C、ARC-E、BioMysteryBench、CritPT、CritPt、FrontierScience Olympiad、FrontierScience Research、GPQA|
|大语言模型|语言处理能力|1376|31|AA-LCR、AutoLogi、BoolQ、CommonSenseQA、Creative Writing v3、DROP、Global PIQA、GovReport|
|大语言模型|金融|47|10|BankerToolBench、Big Finance Bench、FinQA、FinSearchComp T2&T3、FinSearchComp-T3、Finance Agent、Finance Agent v1.1、Finance Agent v2|
|视觉-语言大模型|多图与跨模态整合|12|1|MuirBench|
|视觉-语言大模型|时序与视频理解|172|26|ActivityNet、CharadesSTA、EgoSchema、EgoSchema test、LVBench、LingoQA、LongVideoBench、MLVU|
|视觉-语言大模型|视觉内容生成与编辑|3|2|QwenSVG、SVG-Bench|
|视觉-语言大模型|视觉对话与交互|17|1|MM-MT-Bench|
|视觉-语言大模型|视觉感知与识别|114|10|CountBench、CountQA、ODinW、POPE、RealWorldQA、RefCOCO-avg、RefCOCOg、ScreenSpot|
|视觉-语言大模型|视觉推理|269|24|AI2D、BLINK、BabyVision、CharXiv-R、ChartQA、ChartQA test、ChartQAPro、FigQA|
|视觉-语言大模型|视觉文本理解|240|24|CC-OCR、CharXiv-D、ChartQA、ChartQA test、ChartQAPro、DUDE、DocVQA、DocVQA test|
|听觉-语言大模型|听觉内容推理|6|4|MMAU、MMAU Music、MMAU Sound、MMAU Speech|
|听觉-语言大模型|听觉内容理解|8|5|MMAU、MMAU Music、MMAU Sound、MMAU Speech、VoiceBench Avg|
|听觉-语言大模型|对话管理|0|0||
|听觉-语言大模型|文本到音频生成|0|0||
|听觉-语言大模型|语音翻译|21|5|CoVoST2、CoVoST2 de-en、CoVoST2 en-de、CoVoST2 en-zh、CoVoST2 zh-en|
|听觉-语言大模型|语音识别与转录|23|6|Common Voice 15、FLEURS、LibriSpeech dev-clean、LibriSpeech dev-other、LibriSpeech test-clean、LibriSpeech test-other|
|听觉-语言大模型|说话人分析与分割|0|0||
|听觉-语言大模型|音频分类与标签识别|2|2|Meld、VocalSound|

## 覆盖边界

音频对话管理不能仅凭文本代理任务或语音输入宣称已覆盖；NMOS含义不清，MusicCaps任务方向不清，不能当作文本到音频生成成绩。说话人分析与分割没有已匹配成绩。SVG生成仅部分覆盖视觉生成编辑，不能充当通用图像编辑。

审计清单保存每个benchmark的归类、匹配程度、目录描述和来源。历史快照重复记录不等于独立实验，多标签统计不相加作为总数。