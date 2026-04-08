---
layout: default
title: RESOURCEFUL-2026
---
{% if jekyll.environment  == "production" %}
        {% assign basepath = "." %}
        {%else%}
        {% assign basepath = "" %}
        {% endif %}

# Accepted materials

## Oral talks

  *  <font size="4"> <b> Lost in Translation: Repurposing Semantic Similarity Benchmarks for Evaluating Lexical-Semantic Consistency in LLM-Based Machine Translation </b> </font>  
  [slides](x)  
  <span style="color:gray"> Ye, Quin and Bloem, Jelke </span>  
  <button onclick="toggleAbstract('abstract1')">Show abstract</button>  
  <div id="abstract1" class="abstract" style="display:none;">We propose and demonstrate a repurposing of the lexical similarity benchmark Multi-SimLex and the SimLex-999 family of resources for assessing the cross-lingual lexical-semantic consistency of multilingual large language models. While originally gathered for evaluating word embedding models, the parallel nature of the word pairs enables their use in machine translation settings. Using a manually verified subset of 500 word pairs from the Multi-SimLex dataset, we evaluate models’ ability to assess semantic similarity and perform translation between English and Mandarin through zero-shot prompting. We compare BLOOMZ and GPT-4’s similarity ratings against human-annotated benchmarks and examine translation consistency using our and other metrics, with GPT-4 showing stronger human alignment. As SimLex-999 and Multi-SimLex together cover a range of at least 25 languages, this approach has the potential to be extended to many language pairs including ones that don’t involve English, though it requires some manual checks.</div>

  *  <font size="4"> <b> Bridging the Low Resource Gap in Historical Cryptology: A Multilingual Diachronic Synthetic Dataset for Reproducible Cryptanalysis </b></font>
  [slides](x)  
  <span style="color:gray"> Bruton, Micaella and Beloucif, Meriem and Megyesi, Beáta </span>  
  <button onclick="toggleAbstract('abstract2')">Show abstract</button>  
  <div id="abstract2" class="abstract" style="display:none;">Many NLP tasks suffer from limited aligned supervision in the target domain. Historical cipher decryption represents an extreme case: aligned plaintext–ciphertext pairs are scarce, access to decrypted archives is restricted, and prior work often relies on synthetic data that is neither released nor evaluated for realism. This limits reproducibility and obscures whether models trained on synthetic benchmarks transfer to archival conditions. We introduce HistCiph, the first publicly available multilingual collection of historically grounded plaintext–ciphertext datasets for classical ciphers. Spanning ten languages (Czech, Dutch, English, French, Hungarian, Icelandic, Italian, Polish, Spanish, Swedish) and multiple centuries, the collection combines diachronically balanced historical plaintext with independently generated homophonic substitution keys and controlled transcription noise. Synthetic generation is explicitly constrained by documented properties of historical ciphers, including multi-homophone allocation and variable-length codes. We validate the datasets using information-theoretic diagnostics—entropy, redundancy, frequency masking, and unicity distance—showing that ciphertext distributions approach theoretical bounds while preserving cross-linguistic variation. HistCiph provides a reproducible benchmark for neural decryption and alignment, and illustrates a principled framework for empirically grounded synthetic data generation in low-resource NLP.</div>

  *  <font size="4"> <b> Cultural Grounding in Swedish: Extending an Everyday Knowledge Benchmark for LLMs </b> </font>
  [slides](x)  
  <span style="color:gray"> Beloucif, Meriem and Sjons, Johan </span>  
  <button onclick="toggleAbstract('abstract3')">Show abstract</button>  
  <div id="abstract4" class="abstract" style="display:none;">Benchmarks for evaluating Large Language Models (LLMs) on everyday knowledge across cultures and languages are increasingly used to assess cultural competence and contextual understanding. However, many multilingual extensions rely primarily on translated question–answer pairs, limiting their ability to capture locally grounded variation. In this work, we present a Swedish extension of an existing cross-cultural everyday knowledge benchmark, in which questions are translated into Swedish and answers are collected individually from five participants with diverse social and professional backgrounds. This design enables us to capture situated, naturally produced responses from a specific participant group rather than transferred or translated answer templates. We document the translation protocol, participants, and agreement analysis, and examine variation across participants as a signal of culturally contingent knowledge. We evaluate several state-of-the-art multilingual and instruction-tuned LLMs against the aggregated human responses and analyze model performance. Our results reveal that while models often approximate prototypical answers, they struggle with culturally specific nuances and intra-cultural variation. The Swedish extension provides a resource for studying culturally grounded evaluation and highlights the importance of human-generated local answers when benchmarking LLMs across languages.</div>
          
  *  <font size="4"> <b> Entity Linking for Faroese Using Large Language Models with Web Search </b> </font>
  [slides](x)  
  <span style="color:gray"> Simonsen, Annika and Debess, Iben Nyholm and Einarsson, Hafsteinn </span>  
  <button onclick="toggleAbstract('abstract4')">Show abstract</button>  
  <div id="abstract5" class="abstract" style="display:none;">
    Entity linking connects text mentions to knowledge bases. For low-resource languages, entity linking has typically not been a research priority, as named entity recognition and knowledge base creation must first be addressed. We present the first study of entity linking for Faroese, a North Germanic language with approximately 70,000 speakers. Unlike traditional systems that rely on separate candidate retrieval and ranking components, we employ an end-to-end approach using GPT-5 with integrated web search. Our method prompts the model to directly identify and link named entities to Wikipedia pages through a three-tier fallback strategy: Faroese Wikipedia, English Wikipedia, and finally any available Wikipedia. We evaluate our approach on 1,010 manually annotated examples from a Faroese NER dataset, analyzing entity mentions across Person, Location, Organization, and Miscellaneous types. Human evaluation shows our system achieves 87.5% precision and 87.3% recall, with particularly strong performance on locations (93-95% precision, 92-95% recall). Persons are more challenging (86-88% precision, 72-83% recall). The majority of links (76.5%) point to Faroese Wikipedia, demonstrating the model’s ability to leverage language-specific knowledge bases. A Wikipedia API search baseline without any LLM achieves F1 = 0.57–0.60 on the same evaluation data, confirming that the LLM’s contextual reasoning provides substantial gains over simple search. We validate our approach across three models (GPT-5, Gemini 3 Flash, GPT-5.4 Mini), achieving F1 scores of 0.74–0.87 and confirming that the method generalizes across providers. This work establishes initial performance benchmarks for Faroese entity linking and demonstrates the viability of LLM-based approaches for low-resource languages.
  </div>

  *  <font size="4"> <b> From Polyester Girlfriends to Blind Mice: Creating the First Pragmatics Understanding Benchmarks for Slovene </b> </font>
  [slides](x)  
  <span style="color:gray"> Brglez, Mojca and Vintar, Špela </span>  
  <button onclick="toggleAbstract('abstract5')">Show abstract</button>  
  <div id="abstract6" class="abstract" style="display:none;">
    Large language models are demonstrating increasing capabilities, excelling at benchmarks once considered very difficult. As their capabilities grow, there is a need for more challenging evaluations that go beyond surface-level linguistic competence. The latter involves not only syntax and semantics but also pragmatics, i.e., understanding situational meaning shaped by context and linguistic and cultural norms. To contribute to this line of research, we introduce SloPragEval and SloPragMega, the first pragmatics understanding benchmarks for Slovene, comprising 405 multiple-choice questions. We discuss the difficulties of translation, describe the campaign to establish a human baseline, and report pilot evaluations with LLMs. Our results indicate that current models have substantially improved in their understanding of nuanced language but may still fail to infer implied speaker meaning in non-literal utterances, especially those that are culture-specific. We also observe a significant gap between proprietary and open-source models. Finally, we argue that benchmarks targeting nuanced language understanding and knowledge of the target culture must be designed with care, preferably constructed from native data, and validated with human responses.
  </div>

  *  <font size="4"> <b> SdQuAD: A Benchmark Question Answering Dataset for Low-resource Sindhi Language </b> </font>
  [slides](x)  
  <span style="color:gray"> Ali, Wazir and Rafay, Muhammad and Ali, Nadia and Rehman, Amar </span>  
  <button onclick="toggleAbstract('abstract6')">Show abstract</button>  
  <div id="abstract7" class="abstract" style="display:none;">
    Question answering (QA) datasets are crucial for developing and evaluating monolingual and multilingual language models, yet low-resource languages like Sindhi lack open-source QA resources. We introduce SdQuAD, a novel open-source textual QA dataset for the low-resource Sindhi language, comprising more than 14K QA pairs curated and annotated by native speakers using the Label Studio. Sourced from diverse domains, including news, history, science, geography, business, and tourism, SdQuAD supports both extractive and abstractive QA tasks while capturing Sindhi’s linguistic diversity. We assess annotation quality using span-level agreement and evaluate extractive performance with Exact Match (EM), F1 score, and a TF-IDF baseline. Additionally, we fine-tune mBERT, XLM-RoBERTa, and mT5 models on SdQuAD, benchmarking their performance to demonstrate the dataset’s utility.
  </div>

  *  <font size="4"> <b> LLMs as Assistants for Data Annotation: Addressing Disagreement and Supporting Expert Processes </b> </font>
  [slides](x)  
  <span style="color:gray"> Andrade, Mark and Hefernan, Bláithín and Walsh, Abigail and Castilho, Sheila </span>  
  <button onclick="toggleAbstract('abstract7')">Show abstract</button>  
  <div id="abstract8" class="abstract" style="display:none;">
    This paper investigates the potential of Large Language Models to assist human annotation pipelines, with a particular focus on supporting the development of expert-informed annotation guidelines for document-level content categorisation. We present three experiments exploring distinct roles for LLMs in annotation: as annotators, as domain experts assisting in disagreement resolution, and as analysts of annotator discussions. Using GPT-4.5 and Claude Sonnet 4, we evaluate LLM-generated annotation guidelines for a document-level classification tasks in terms of coverage, applicability, and usefulness. Preliminary results are mixed-to-positive, with evidence that LLMs can provide useful support across different stages of the annotation pipeline, particularly when supplied with rich contextual information such as prior human annotations and annotator discussions.
  </div>

  *  <font size="4"> <b> Annotation Quality in Aspect-Based Sentiment Analysis: A Case Study Comparing Experts, Students, Crowdworkers, and Large Language Models </b> </font>
  [slides](x)  
  <span style="color:gray"> Donhauser, Niklas and Fehle, Jakob and Hellwig, Nils Constantin and Weinberger, Markus and Kruschwitz, Udo and Wolff, Christian </span>  
  <button onclick="toggleAbstract('abstract8')">Show abstract</button>  
  <div id="abstract8" class="abstract" style="display:none;">
    Aspect-Based Sentiment Analysis (ABSA) enables fine-grained opinion analysis by identifying sentiments toward specific aspects or targets within a text. While ABSA has been widely studied for English, research on other languages such as German remains limited, largely due to the lack of high-quality annotated datasets. This paper examines how different annotation sources influence the development of German ABSA. To this end, an existing dataset is re-annotated by experts to establish a ground truth, which serves as a reference for evaluating annotations produced by students, crowdworkers, Large Language Models (LLMs), and experts. Annotation quality is compared using Inter-Annotator Agreement (IAA) and its impact on downstream model performance for different ABSA subtasks. The evaluation focuses on Aspect Category Sentiment Analysis (ACSA) and Target Aspect Sentiment Detection (TASD). We apply State-of-the-Art (SOTA) methods for ABSA, including BERT-, T5-, and LLaMA-based approaches to assess performance differences, spanning fine-tuning and in-context learning with instruction prompts. The findings provide practical insights into trade-offs between annotation reliability, and efficiency, offering guidance for dataset construction in under-resourced Natural Language Processing (NLP) scenarios.
  </div>

## Posters

  *  <font size="4"> <b> WikiQA-IS: Assisted Benchmark Generation and Automated Evaluation of Icelandic Cultural Knowledge in LLMs </b> </font>  
  <span style="color:gray"> Arnardóttir, Þórunn and Bjartur Einarsson, Elías and Ingvarsson Juto, Garðar and Páll Helgason, Þorvaldur and Einarsson, Hafsteinn </span>  
  <button onclick="toggleAbstract('abstract3')">Show Abstract</button>
  <div id="abstract3" class="abstract" style="display:none;">This paper presents WikiQA-IS, a novel question-answering dataset focusing on Icelandic culture and history, along with an automated pipeline for dataset generation and evaluation. Leveraging GPT-4 to create questions and answers based on Icelandic Wikipedia articles and news sources, we produced a high-quality corpus of 2,000 question-answer pairs. We introduce an automatic evaluation method using GPT-4o as a judge, which shows strong agreement with human evaluations. Our benchmark reveals varying performances across different language models, with closed-source models generally outperforming open-weights alternatives. This work contributes a resource for evaluating language models' knowledge of Icelandic culture and offers a replicable framework for creating similar datasets in other cultural contexts.</div>

  *  <font size="4"> <b> Universal Dependencies Treebank for Uzbek </b> </font>
  [poster](./slides/akhundjanova-poster.pdf)  
  <span style="color:gray"> Akhundjanova, Arofat and Talamo, Luigi </span>  
  <button onclick="toggleAbstract('abstract9')">Show Abstract</button>  
  <div id="abstract9" class="abstract" style="display:none;">We present the first Universal Dependencies treebank for Uzbek, a low-resource language from the Turkic family. The treebank contains 500 sentences (5850 tokens) sourced from the news and fiction genres and it is annotated for lemmas, part-of-speech (POS) tags, morphological features, and dependency relations. We describe our methodology for building the treebank, which consists of a mix of manual and automatic annotation and discuss some constructions of the Uzbek language that pose challenges to the UD framework.</div>

  *  <font size="4"> <b> DUDU: A Treebank for Ottoman Turkish in UD Style </b> </font>
  [poster](./slides/yilandiloglu-poster.pdf)  
  <span style="color:gray"> Yılandiloğlu, Enes and Siewert, Janine </span>  
  <button onclick="toggleAbstract('abstract10')">Show Abstract</button>  
  <div id="abstract10" class="abstract" style="display:none;">This paper introduces a recently released Ottoman Turkish (ota) treebank in Universal Dependencies (UD) style, DUDU. The DUDU Treebank consists of 1,064 automatically annotated and manually corrected sentences. The texts were manually collected from various academic or literary sources available on the Internet. Following preprocessing, the sentences were annotated using a MaCHAMP-based neural network model utilizing the large language model (LLM) architecture and manually corrected. The treebank became publicly available with the 2.14 release, and future steps involve expanding the treebank with more data and refining the annotation scheme. The treebank is the first and only treebank that utilizes the IJMES transliteration alphabet. The treebank not only gives insight on Ottoman Turkish lexically, morphologically, and syntactically, but also provides a small but robust test set for future computational models for Ottoman Turkish.</div>

  *  <font size="4"> <b> A Simple Audio and Text Collection-Annotation Tool Targeted to Brazilian Indigenous Language Native Speakers </b> </font>  
  <span style="color:gray"> Polleti, Gustavo Padilha and Cozman, Fabio and Gerardi, Fabricio </span>  
  <button onclick="toggleAbstract('abstract11')">Show Abstract</button>
  <div id="abstract11" class="abstract" style="display:none;">In this paper we present an audio and text annotation tool for native speakers, with a particular focus on Brazilian indigenous languages. Our tool simplifies the process of language resource annotation and employs gamefication techniques typically found in language learning games. Then we describe the annotation tool and present preliminary results for the Bororo language. We discuss the limitations of our tool, highlighting ethical and practical implementation concerns.</div>

  *  <font size="4"> <b> Fine-Tuning Cross-Lingual LLMs for POS Tagging in Code-Switched Contexts </b> </font>  
  <span style="color:gray"> Absar, Shayaan </span>  
  <button onclick="toggleAbstract('abstract12')">Show Abstract</button>
  <div id="abstract12" class="abstract" style="display:none;">Code-switching (CS) involves speakers switching between two (or potentially more) languages during conversation and is a common phenomenon in bilingual communities. The majority of NLP research has been devoted to mono-lingual language modelling. Consequentially, most models perform poorly on code-switched data. This paper investigates the effectiveness of Cross-Lingual Large Language Models on the task of POS (Part-of-Speech) tagging in code-switched contexts, once they have undergone a fine-tuning process. The models are trained on code-switched combinations of Indian languages and English. This paper also seeks to investigate whether fine-tuned models are able to generalise and POS tag code-switched combinations that were not a part of the fine-tuning dataset. Additionally, this paper presents a new metric, the S-index (Switching-Index), for measuring the level of code-switching within an utterance.</div>

  *  <font size="4"> <b> First Steps in Benchmarking Latvian in Large Language Models </b> </font>
  [poster](./slides/skadina-poster.pdf)  
  <span style="color:gray"> Skadina, Inguna and Bakanovs, Bruno and Darģis, Roberts </span>  
  <button onclick="toggleAbstract('abstract13')">Show Abstract</button>  
  <div id="abstract13" class="abstract" style="display:none;">The performance of multilingual large language models (LLMs) in low-resource languages, such as Latvian, has been under-explored. In this paper, we investigate the capabilities of several open and commercial LLMs in the Latvian language understanding tasks. We evaluate these models across several well-known benchmarks, such as the Choice of Plausible Alternatives (COPA) and Measuring Massive Multitask Language Understanding (MMLU), which were adapted into Latvian using machine translation. Our results highlight significant variability in model performance, emphasizing the challenges of extending LLMs to low-resource languages. We also analyze the effect of post-editing on machine-translated datasets, observing notable improvements in model accuracy, particularly with BERT-based architectures. We also assess open-source LLMs using the Belebele dataset, showcasing competitive performance from open-weight models when compared to proprietary systems. This study reveals key insights into the limitations of current LLMs in low-resource settings and provides datasets for future benchmarking efforts.</div>

  *  <font size="4"> <b> On the Usage of Semantics, Syntax, and Morphology for Noun Classification in IsiZulu </b> </font>  
  <span style="color:gray"> Sayed, Imaan and Mahlaza, Zola and van der Leek, Alexander and Mopp, Jonathan and Keet, C. Maria </span>  
  <button onclick="toggleAbstract('abstract14')">Show Abstract</button>
  <div id="abstract14" class="abstract" style="display:none;">There is limited work aimed at solving the core task of noun classification for Nguni languages. The task focuses on identifying the semantic categorisation of each noun and plays a crucial role in the ability to form semantically and morphologically valid sentences. The work by Byamugisha (2022) was the first to tackle the problem for a related, but non-Nguni, language. While there have been efforts to replicate it for a Nguni language, there has been no effort focused on comparing the technique used in the original work vs. contemporary neural methods or a number of traditional machine learning classification techniques that do not rely on human-guided knowledge to the same extent. We reproduce Byamugisha (2022)’s work with different configurations to account for differences in access to datasets and resources, compare the approach with a pre-trained transformer-based model, and traditional machine learning models that relyon less human-guided knowledge. The newly created data-driven models outperform the knowledge-infused models, with the best performing models achieving an F1 score of 0.97.</div>

  *  <font size="4"> <b> VerbCraft: Morphologically-Aware Armenian Text Generation Using LLMs in Low-Resource Settings </b> </font>  
  <span style="color:gray"> Avetisyan, Hayastan and Broneske, David </span>  
  <button onclick="toggleAbstract('abstract15')">Show Abstract</button>
  <div id="abstract15" class="abstract" style="display:none;">Understanding and generating morphologically complex verb forms is a critical challenge in Natural Language Processing (NLP), particularly for low-resource languages like Armenian. Armenian's verb morphology encodes multiple layers of grammatical information, such as tense, aspect, mood, voice, person, and number, requiring nuanced computational modeling. We introduce VerbCraft, a novel neural model that integrates explicit morphological classifiers into the mBART-50 architecture. VerbCraft achieves a BLEU score of 0.4899 on test data, compared to the baseline's 0.9975, reflecting its focus on prioritizing morphological precision over fluency. With over 99\% accuracy in aspect and voice predictions and robust performance on rare and irregular verb forms, VerbCraft addresses data scarcity through synthetic data generation with human-in-the-loop validation. Beyond Armenian, it offers a scalable framework for morphologically rich, low-resource languages, paving the way for linguistically informed NLP systems and advancing language preservation efforts.</div>

  *  <font size="4"> <b> Post-OCR Correction of Historical German Periodicals using LLMs </b> </font>  
  <span style="color:gray"> Danilova, Vera and Aangenendt, Gijs </span>  
  <button onclick="toggleAbstract('abstract16')">Show Abstract</button>
  <div id="abstract16" class="abstract" style="display:none;">
    Optical Character Recognition (OCR) is critical for accurate access to historical corpora, providing a foundation for processing pipelines and the reliable interpretation of historical texts. Despite advances, the quality of OCR in historical documents remains limited, often requiring post-OCR correction to address residual errors. Building on recent progress with instruction-tuned Llama 2 models applied to English historical newspapers, we examine the potential of German Llama 2 and Mistral models for post-OCR correction of German medical historical periodicals. We perform instruction tuning using two configurations of training data, augmenting our small annotated dataset with two German datasets from the same time period. The results demonstrate that German Mistral enhances the raw OCR output, achieving a lower average word error rate (WER). However, the average character error rate (CER) either decreases or remains unchanged across all models considered. We perform an analysis of performance within the error groups and provide an interpretation of the results.
  </div>

  *  <font size="4"> <b> From Words to Action: A National Initiative to Overcome Data Scarcity for the Slovene LLM </b> </font>
  [poster](./slides/arhar-holdt-poster.pdf)  
  <span style="color:gray"> Holdt, Špela Arhar and Antloga, Špela and Munda, Tina and Pori, Eva and Krek, Simon </span>  
  <button onclick="toggleAbstract('abstract17')">Show Abstract</button>  
  <div id="abstract17" class="abstract" style="display:none;">
    Large Language Models (LLMs) have demonstrated significant potential in natural language processing, but they depend on vast, diverse datasets, creating challenges for languages with limited resources. The paper presents a national initiative that addresses these challenges for Slovene. We outline strategies for large-scale text collection, including the creation of an online platform to engage the broader public in contributing texts and a communication campaign promoting openly accessible and transparently developed LLMs.
  </div>

  *  <font size="4"> <b> Assessing the Similarity of Cross-Lingual Seq2Seq Sentence Embeddings Using Low-Resource Spectral Clustering </b> </font>  
  <span style="color:gray"> Moll, Nelson and Rabbani, Tahseen </span>  
  <button onclick="toggleAbstract('abstract18')">Show Abstract</button>
  <div id="abstract18" class="abstract" style="display:none;">
    In this work, we study the cross-lingual distance of machine translations through alignment of seq2seq representations over small corpora. First, we use the M2M100 model to collect sentence-level representations of The Book of Revelation in several languages. We then perform unsupervised manifold alignment (spectral clustering) between these collections of embeddings. As verses between translations are not necessarily aligned, our procedure falls under the challenging, but more realistic non-correspondence regime. The cost function associated with each alignment is used to rank the relative (machine) similarity of one language to another. We then perform correspondent alignment over another cluster of languages, this time using FLORES+ parallel NLLB model embeddings. Our experiments demonstrate that the representations of closely-related languages group closely, and are cheap to align (requiring <1000 sentences) via our strategy.
  </div>

  *  <font size="4"> <b> "I Need More Context and an English Translation": Analysing How LLMs Identify Personal Information in Komi, Polish, and English </b> </font>  
  <span style="color:gray"> Ilinykh, Nikolai and Szawerna, Maria Irena </span>  
  <button onclick="toggleAbstract('abstract19')">Show Abstract</button>
  <div id="abstract19" class="abstract" style="display:none;">
    Automatic identification of personal information (PI) is particularly difficult for languages with limited linguistic resources. Recently, large language models (LLMs) have been applied to various tasks involving low-resourced languages, but their capability to process PI in such contexts remains under-explored. In this paper we provide a qualitative analysis of the outputs from three LLMs prompted to identify PI in texts written in Komi (Permyak and Zyrian), Polish, and English. Our analysis highlights challenges in using pre-trained LLMs for PI identification in both low- and medium-resourced languages. It also motivates the need to develop LLMs that understand the differences in how PI is expressed across languages with varying levels of availability of linguistic resources.
  </div>

  *  <font size="4"> <b> Federated Meta-Learning for Low-Resource Translation of Kirundi </b> </font>  
  <span style="color:gray"> Sang, Kyle Rui and Rabbani, Tahseen and Zhou, Tianyi </span>  
  <button onclick="toggleAbstract('abstract20')">Show Abstract</button>
  <div id="abstract20" class="abstract" style="display:none;">
    In this work, we reframe multilingual neural machine translation (NMT) as a federated meta-learning problem and introduce a translation dataset for the low-resource Kirundi language. We aggregate machine translation models locally trained on varying (but related) source languages to produce a global meta-model that encodes abstract representations of key semantic structures relevant to the parent languages. We then use the Reptile algorithm and Optuna fine-tuning to fit the global model onto a target language. The target language may live outside the subset of parent languages (such as closely-related dialects or sibling languages), which is particularly useful for languages with limitedly available sentence pairs. We first develop a novel dataset of Kirundi-English sentence pairs curated from Biblical translation. We then demonstrate that a federated learning approach can produce a tiny 4.8M Kirundi translation model and a stronger NLLB-600M model which performs well on both our Biblical corpus and the FLORES-200 Kirundi corpus.
  </div>

  *  <font size="4"> <b> Second language Korean Universal Dependency treebank v1.2: Focus on Data Augmentation and Annotation Scheme Refinement </b> </font>
  [slides](./slides/sung-shin-poster.pdf)  
  <span style="color:gray"> Sung, Hakyung and Shin, Gyu-Ho </span>  
  <button onclick="toggleAbstract('abstract21')">Show Abstract</button>  
  <div id="abstract21" class="abstract" style="display:none;">
    We expand the second language (L2) Korean Universal Dependencies (UD) treebank with 5,454 manually annotated sentences. The annotation guidelines are also revised to better align with the UD framework. Using this enhanced treebank, we fine-tune three Korean language models—Stanza, spaCy, and Trankit—and evaluate their performance on in-domain and out-of-domain L2-Korean datasets. The results show that fine-tuning significantly improves their performance across various metrics, thus highlighting the importance of using well-tailored L2 datasets for fine-tuning first-language-based, general-purpose language models for the morphosyntactic analysis of L2 data.
  </div>
  <button onclick="toggleDisplay('video1')">Watch presentation video</button>
  <div id="video1" class="video" style="display:none;">
  <iframe 
    src="https://drive.google.com/file/d/1o1BO4B8dmOESO9sxLLqcLzIxoPubXPOq/preview"
    width="640"
    height="480"
    allow="autoplay"
  ></iframe>
  </div>

  *  <font size="4"> <b> Recommendations for Overcoming Linguistic Barriers in Healthcare: Challenges and Innovations in NLP for Haitian Creole </b> </font>  
  <span style="color:gray"> Mompelat, Ludovic </span>  
  <button onclick="toggleAbstract('abstract22')">Show Abstract</button>
  <div id="abstract22" class="abstract" style="display:none;">
    Haitian Creole, spoken by millions in Haiti and its diaspora, remains underrepresented in Natural Language Processing (NLP) research, limiting the availability of effective translation tools. In Miami, a significant Haitian Creole-speaking population faces healthcare disparities exacerbated by language barriers. Existing translation systems fail to address key challenges such as linguistic variation within the Creole language, frequent code-switching, and the lack of standardized medical terminology. This work proposes a structured methodology for the development of an AI-assisted translation and interpretation tool tailored for patient-provider communication in a medical setting. To achieve this, we propose a hybrid NLP approach that integrates fine-tuned Large Language Models (LLMs) with traditional machine translation methods. This combination ensures accurate, context-sensitive translation that adapts to both formal medical discourse and conversational registers while maintaining linguistic consistency. Additionally, we discuss data collection strategies, annotation challenges, and evaluation metrics necessary for building an ethically designed, scalable NLP system. By addressing these issues, this research provides a foundation for improving healthcare accessibility and linguistic equity for Haitian Creole speakers.
  </div>
  <button onclick="toggleDisplay('video2')">Watch presentation video</button>
  <div id="video2" class="video" style="display:none;">
  <iframe 
    src="https://drive.google.com/file/d/1GM7zDRkP1ZUp7x98RCjRPRwL8RPvkX6L/preview"
    width="640"
    height="480"
    allow="autoplay"
  ></iframe>
  </div>

*  <font size="4"> <b> Interpreting the UAS and the LAS of the parsing of Old English with Universal Dependencies </b> </font>  
   <span style="color:gray"> Martin Arista, Javier and Elvira Ojanguren López, Ana and Domínguez Barragán, Sara </span>  
   [Download Paper]({{ basepath }}/papers/interpreting-the-uas-and-the-las.pdf)
   <button onclick="toggleAbstract('abstract23')">Show Abstract</button>
   <div id="abstract23" class="abstract" style="display:none;">
     This paper interprets, from a linguistic point of view, the Unlabelled Attachment Score (UAS) and Labelled Attachment Score (LAS) metrics obtained in the Universal Dependencies parsing of Old English. The study assesses the performance of three distinct training methods based on the Natural Language Processing library spaCy: a baseline pipeline, a pretrained model, and a transformer-based model (MobileBERT). Using datasets ranging from 1,000 to 20,000 words, the best-performing model (pretrained model with 20,000 words) achieved 83.2% UAS and 74.2% LAS. The model performs better at identifying structural relations than at labeling specific dependency relations. There is a consistent 9 point gap between UAS and LAS across the different structural levels, including the word, the phrase, the clause, and the complex sentence. While the model shows high accuracy in morphologically marked local relations and morphological feature recognition (often over 90%), its accuracy is lower with long-distance dependencies and complex syntactic structures. Particularly problematic areas include non-projective dependencies, fixed expressions, copulative constructions, and double object constructions. The conclusion is reached that improving parsing accuracy will require larger training datasets and a fine-grained analysis of complex syntactic relations that is compatible with the strong performance reached in morphological feature recognition.
   </div>

  *  <font size="4"> <b> Beyond a Means to an End: A Case Study in Building Phonotactic Corpora for Central Australian Languages </b> </font>
  [slides](./slides/muradoglu-poster.pdf)  
  <span style="color:gray"> Muradoglu, Saliha and Gray, James and Simpson, Jane Helen and Proctor, Michael and Harvey, Mark </span>  
  <button onclick="toggleAbstract('abstract24')">Show Abstract</button>  
  <div id="abstract24" class="abstract" style="display:none;">
    Linguistic datasets are essential across fields: computational linguists use them for NLP development, theoretical linguists for statistical arguments supporting hypotheses about language, and documentary linguists for preserving examples and aiding grammatical descriptions. Transforming raw data (e.g., recordings or dictionaries) into structured forms (e.g., tables) requires non-trivial decisions within processing pipelines. This paper highlights the importance of these processes in understanding linguistic systems. Our contributions include: (1) an interactive dashboard for four central Australian languages with custom filters, and (2) demonstrating how data processing decisions influence measured outcomes.
  </div>
  <button onclick="toggleDisplay('video3')">Watch presentation video</button>
  <div id="video3" class="video" style="display:none;">
  <iframe 
    src="https://drive.google.com/file/d/1tBPM1z4sEL1imTXOQ_gFtlnCaej5iBCN/preview"
    width="640"
    height="480"
    allow="autoplay"
  ></iframe>
  </div>

  *  <font size="4"> <b> Investigating Gender Bias for Turkish in Multilingual LLMs </b> </font>  
  <span style="color:gray">Özçelik, Irem and Kurfali, Murathan </span>  
     [Download Paper]({{ basepath }}/papers/investigating-gender-bias-for-turkish.pdf)
  <button onclick="toggleAbstract('abstract25')">Show Abstract</button>
  <div id="abstract25" class="abstract" style="display:none;">
    In this study, we examine patterns of gender bias in Large Language Models (LLMs) for Turkish by comparing models of different sizes and architectures. To capture subtle forms of bias, including the double bind effect, we created a culturally relevant dataset consisting of professions, personal traits, and their combinations. Our findings reveal that gender bias persists across the models, although variations in bias patterns suggest ongoing efforts to mitigate it.
  </div>

  *  <font size="4"> <b> Towards an acoustically-validated phonetic corpus of spoken Swedish </b> </font>  
  <span style="color:gray">O'Regan, Jim and Edlund, Jens </span>  
     [Download Paper]({{ basepath }}/papers/towards-an-acoustically-validated-phonetic.pdf)
  <button onclick="toggleAbstract('abstract26')">Show Abstract</button>
  <div id="abstract26" class="abstract" style="display:none;">
    In this document, we describe ongoing work towards the creation of a phonetically transcribed corpus of spoken Swedish, with aims towards creating a pronunciation dictionary that takes into account dialectal variation. Using speeches from the Swedish Riksdag (Parliament), we use the output of a phonetic recognition system to validate pronunciations for a variety of Swedish dialects.
  </div>

<script>
function toggleAbstract(id) {
    var abstract = document.getElementById(id);
    if (abstract.style.display === "none") {
        abstract.style.display = "block";
    } else {
        abstract.style.display = "none";
    }
}
</script>

<script>
  function toggleDisplay(id) {
    var el = document.getElementById(id);
    if (el.style.display === "none" || el.style.display === "") {
      el.style.display = "block";
    } else {
      el.style.display = "none";
    }
  }
</script>
