# Luigi

## Background
The Luigi Mangione case involves the assassination of Brian Thompson, the CEO of UnitedHealthcare, which took place on December 4, 2024, in Midtown Manhattan, New York City. Luigi Mangione, a 26-year-old Ivy League graduate from the University of Pennsylvania, is the prime suspect in this high-profile murder. Thompson was shot in a targeted attack outside the New York Hilton Midtown hotel while on his way to the company’s annual investors' meeting. The gunman, identified as Mangione, used a 3D-printed "ghost gun" equipped with a silencer and fled the scene after the shooting. Evidence at the crime scene included shell casings inscribed with the words "deny," "delay," and "depose," a reference to the phrase "delay, deny, defend," often criticized as a tactic used by insurance companies to avoid paying claims.

Mangione was arrested five days later, on December 9, 2024, at a McDonald's in Altoona, Pennsylvania, following a nationwide manhunt. At the time of his arrest, he was found with a 3D-printed pistol matching the murder weapon, a silencer, fake IDs, and a handwritten note expressing hostility toward the health insurance industry and corporate greed. The note reportedly included phrases like "these parasites had it coming," suggesting a motive tied to frustration with the U.S. healthcare system. Mangione, born into a prominent Maryland family with ties to real estate and healthcare businesses, had no direct connection to UnitedHealthcare as a client but appeared driven by broader resentment toward the industry.

Legally, Mangione faces both state and federal charges. On December 17, 2024, a Manhattan grand jury indicted him on 11 state charges, including first-degree murder in furtherance of terrorism, second-degree murder, and weapons-related offenses. The terrorism charge stems from prosecutors’ assertion that the killing was intended to "intimidate or coerce a civilian population" and "evoke terror," as stated by Manhattan District Attorney Alvin Bragg. Federally, he faces four charges, including murder and stalking, which could make him eligible for the death penalty. Mangione pleaded not guilty to the state charges on December 23, 2024, during his arraignment in New York State Supreme Court. His attorney, Karen Friedman Agnifilo, has argued that the case has been politicized, citing conflicting legal theories between state and federal prosecutors and concerns over a fair trial due to public and official statements.

The case has sparked significant public reaction, with some online communities praising Mangione as a "folk hero" amid widespread anger toward the U.S. healthcare system. Hashtags like "#FreeLuigi" have gained traction, reflecting frustration over insurance practices, though officials, including NYPD Commissioner Jessica Tisch, have condemned such sentiments as "vile" and "reckless." Mangione’s next court appearance is scheduled for February 21, 2025, as the state and federal cases proceed in parallel, with the state trial expected to occur first. The assassination has also reignited debates about healthcare reform in the United States.

## Proposal

Research Proposal: Mapping the Emotional Landscape of Systemic Grievance: A Knowledge Graph Framework Integrating Political Emotions Theory for Analyzing Online Discourse
Authors: [Your Name] (PhD Candidate, Information Science), [Co-author's Name] (PhD Candidate, Political Science)
Target Venue: EMNLP 2025
1. Introduction & Motivation
The assassination of UnitedHealthcare CEO Brian Thompson by Luigi Mangione in December 2024, and the subsequent public reaction, provide a stark case study of the intersection between individual acts of violence, systemic societal grievances (specifically regarding the US healthcare system), and the complex emotional responses manifested in online discourse. While traditional sentiment analysis can gauge positivity or negativity, it often fails to capture the nuances of political emotions – such as anger, resentment, fear, sympathy, or moral outrage – that drive political attitudes and potentially collective action (Marcus, Neuman, & MacKuen, 2000; Jasper, 2011).1 The Mangione case, with reactions ranging from condemnation to labeling the suspect a "folk hero," highlights the need for more sophisticated methods to understand these underlying emotional currents.
This project proposes the development and evaluation of a novel computational framework that integrates Political Emotions Theory (PET) with Knowledge Graph (KG) technology to analyze large-scale social media data. We aim to move beyond simple sentiment analysis to model the complex web of entities (individuals, organizations, concepts), the specific political emotions directed towards them, and the narratives constructed within online discussions. Using the extensive Twitter dataset collected around the Mangione case (703,845 posts, Nov 2024 - Jan 2025), we will build and test a pipeline designed to operationalize PET concepts computationally. The goal is not merely to analyze this single event, but to create a reusable framework applicable to other instances of online discourse surrounding controversial events driven by perceived systemic failures or political grievances.
2. Theoretical Framework: Political Emotions Theory (PET)
Political Emotions Theory posits that emotions are not just individual psychological states but are socially constructed, politically relevant forces that shape public opinion, political judgment, and behavior. Key tenets relevant to this project include:
* Appraisal Theory: Emotions arise from individuals' assessments (appraisals) of events or situations concerning their goals, values, and well-being (Lazarus, 1991; Smith & Ellsworth, 1985).2 In the Mangione case, appraisals might relate to perceived injustices by the healthcare system, the appropriateness of violence, or the state of corporate power.
* Specific Emotions, Specific Effects: Different emotions have distinct political implications. Anger often motivates action against perceived injustice, fear can lead to demands for security or avoidance, sympathy can foster solidarity, and resentment can target specific groups or institutions (Weber, 2013; Nussbaum, 2016).3
* Collective Emotions: Emotions can be shared and amplified within groups, shaping collective identities and mobilizing collective action, even if virtually (von Scheve & Salmella, 2014).4 Online platforms like Twitter are key arenas for this process.
Our framework will aim to computationally identify and map these specific political emotions and their targets within the Twitter discourse, connecting them to the broader context of healthcare system critique.
3. Related Work
* Computational Analysis of Political Discourse: Existing work includes sentiment analysis, stance detection, topic modeling, and hate speech detection on social media (e.g., Mohammad, 2016; Vilares & He, 2017).5 However, few studies explicitly operationalize fine-grained political emotions based on PET.
* Emotion AI and NLP: Advances in NLP enable more nuanced emotion detection beyond basic sentiment (e.g., Plutchik's wheel, Ekman's basic emotions).6 We will leverage these but adapt them to the specific context of political emotions identified by PET scholars.
* Knowledge Graphs in Social Sciences: KGs have been used to model social networks, political events, and misinformation spread (e.g., Färber et al., 2018; Abu-Salih, 2021).7 Our work extends this by explicitly encoding political emotions and theoretical constructs from PET within the KG structure.
4. Research Questions
* RQ1: How can concepts from Political Emotions Theory (e.g., specific emotions like anger, resentment, sympathy; appraisal targets) be operationalized and computationally detected in short, informal Twitter posts related to a politically charged event?
* RQ2: What is the distribution and targeting of specific political emotions (beyond simple sentiment) expressed in the Twitter discourse surrounding the Luigi Mangione case? (e.g., Anger towards UHC, Sympathy towards Mangione, Resentment towards the System).
* RQ3: How can a Knowledge Graph effectively model the relationships between key entities (Mangione, Thompson, UHC, Healthcare System, Government), expressed political emotions, and associated narrative elements (e.g., "delay, deny, depose," "folk hero," "systemic failure") within this discourse?
* RQ4: What insights does the KG-PET framework reveal about the structure and dynamics of political emotion expression in this context, compared to traditional sentiment analysis or topic modeling? (e.g., identifying clusters of emotional narratives, tracking shifts over time).
* RQ5: How generalizable is the proposed framework for analyzing political emotions in online discourse related to other events characterized by systemic grievances?
5. Proposed Methodology: A KG-PET Pipeline
We propose a multi-stage pipeline:
* Stage 1: Data Preparation & Annotation:
    * Utilize the collected 703,845 Twitter posts.
    * Manually annotate the sampled 1,000 posts based on a PET-informed coding scheme. This scheme will include labels for:
        * Fine-grained Emotions: Anger, Resentment, Fear, Disgust, Sympathy, Contempt, Moral Outrage, Hope, etc. (Allowing multi-label).
        * Emotion Target: Mangione, Thompson, UHC, Healthcare System, Government, Media, Other Users, Abstract Concepts (e.g., violence, corporate greed).
        * Stance/Appraisal: Pro-/Anti-Mangione's actions, Pro-/Anti-System critique, Justification/Condemnation of violence.
    * This annotated dataset is crucial for training and evaluating subsequent models.
* Stage 2: Emotion & Target Classification:
    * Fine-tune pre-trained language models (e.g., BERT, RoBERTa) on the annotated dataset for multi-label political emotion classification and target identification. Explore sequence-to-sequence or joint modeling approaches.
* Stage 3: Entity & Concept Recognition:
    * Use Named Entity Recognition (NER) tools, potentially fine-tuned, to identify key actors (Mangione, Thompson), organizations (UHC, UPenn), locations (NYC, Altoona), and potentially keywords representing core concepts ("ghost gun," "delay deny depose," "healthcare reform," "terrorism charge").
* Stage 4: Relation Extraction:
    * Develop or adapt relation extraction techniques (rule-based, pattern-based, or model-based using dependency parsing or LLMs) to identify links between:
        * User/Post -> expresses -> Emotion
        * Emotion -> targets -> Entity/Concept
        * Entity -> associated_with -> Concept/Narrative Element (e.g., Mangione -> associated_with -> "folk hero" narrative)
        * Post -> discusses -> Topic (derived via topic modeling or keywords)
* Stage 5: Knowledge Graph Construction:
    * Define a KG schema (ontology) based on PET and the specifics of the case. Nodes will represent entities (Persons, Organizations, Locations), Concepts (Healthcare System, Terrorism, Corporate Greed), Emotions (Anger, Sympathy), and potentially individual Posts/Users. Edges will represent the extracted relations (expresses_emotion, targets_entity, critiques_system, supports_narrative, etc.).
    * Populate the KG by applying the trained models (Stage 2, 3, 4) to the larger dataset and mapping the outputs to the defined schema.
* Stage 6: KG Analysis & Framework Validation:
    * Query the KG to answer RQs 2, 3, and 4. Analyze paths, central nodes, community structures (e.g., clusters of users sharing similar emotional responses towards specific targets), and emergent narrative structures.
    * Visualize subgraphs representing specific emotional dynamics (e.g., the network of anger directed at UHC and the healthcare system).
    * Compare insights gained from the KG-PET framework against baseline analyses (e.g., simple sentiment distribution, basic topic modeling) to demonstrate added value (RQ4).
    * Evaluate the framework's components (emotion classification accuracy, relation extraction F1-score) and qualitatively assess the coherence and explanatory power of the generated KG.
6. Expected Contributions
* Methodological: A novel, reproducible framework (the KG-PET pipeline) for computationally modeling and analyzing political emotions in large-scale online text, operationalizing Political Emotions Theory.
* Empirical: A nuanced, data-driven analysis of the complex emotional landscape surrounding the Mangione case, revealing the specific political emotions driving online reactions and their connection to systemic healthcare grievances.
* Theoretical: Demonstration of how computational methods can enrich Political Emotions Theory by enabling large-scale analysis and potentially revealing patterns not easily observable through traditional qualitative methods. Contribution to understanding online mobilization and polarization.
* Interdisciplinary: A strong example of bridging Information Science (NLP, KG, Data Science) and Political Science (Political Theory, Public Opinion).
7. Plan & Feasibility
* Data: Already collected and sampled for annotation.
* Expertise: Combines Information Science (NLP/KG methods) and Political Science (PET expertise).
* Tools: Leverage existing NLP libraries (Hugging Face Transformers, spaCy) and KG platforms (Neo4j, RDFLib).
* Timeline: Feasible for EMNLP 2025 submission deadline (assuming ~May/June 2025 deadline requires significant progress by early 2025). Manual annotation is a bottleneck but achievable with 1000 posts.
8. Conclusion
This project addresses a critical gap in understanding the role of political emotions in shaping online discourse around significant socio-political events. By developing a KG-PET framework and applying it to the rich dataset of the Luigi Mangione case, we aim to provide both methodological innovation for computational social science and crucial insights into the emotional dynamics underlying public responses to systemic issues like healthcare access and corporate accountability. The focus on building a framework ensures the contribution extends beyond the specific case study, offering a valuable tool for future research.
