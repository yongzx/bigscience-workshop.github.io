# BigScience – Working Groups

## Collaborative tasks

The workshop involves a set of **collaborative tasks** conducted along the year and aimed at creating, sharing and evaluating a large multilingual dataset and a large language model as tools for research. The collaborative tasks are quite large since they involve several millions GPU hours on a supercomputer.

The goal of the collaborative tasks is in particular to collaboratively create and share several **artifacts** as tools for the research community:

* A **Multilingual Dataset** for Research (possibly full-open-access, possibly behind an authentication access portal to follow GdPR and data privacy legislations => to be defined by the organization committee in charge of this artifact)
* A **large Language Model** for Research (possibly full-open-access, possibly behind a researcher’s authentication access portal like the dataset => to be defined by the organization committee in charge of this artifact)
* **Software tools** created to complete the shared tasks, e.g. dataset filtering, model off-loading, etc (under very permissive licence, e.g. Apache2 => to be by the organization committee in charge of this artifact)
* Extensive **documentation** of the evaluation results, protocols, approach, datasets, and tools developed in the course of the project for future reconduction


## Table of Content


- [Overview: how to participate, what roles](#overview-how-to-participate-what-roles)
  - [More details on the role of the co-chairs](#more-details-on-the-role-of-the-co-chairs)
- [Working Groups](#working-groups) (Note that Chairs are evolving)
- [Workshop organization](#workshop-organization) - Chairs:  Matthias Gallé, Angela Fan, Suzana Ilić
- [Dataset creation](#dataset-creation) - Area-Chair: Yacine Jernite
  - [Data Governance and Archival Strategies](#data-governance-and-archival-strategies) - Chairs: Yacine Jernite, Huu Nguyen, Meg Mitchell
  - [Data Sourcing and Representativeness](#data-sourcing-and-representativeness) - Chairs: Angie McMillan-Major, Pedro Ortiz Suárez, Zeerak Waseem
  - [Data Tooling: from Data Sources to Training Dataset](#data-tooling-from-data-sources-to-training-dataset) - Chairs: Colin Raffel, Albert Villanova, Sampo Pyysalo, Filip Ginter
- [Modeling approach](#modeling-approach) - Area-Chairs: Victor Sanh, Stephen Bach
  - [Modeling: Architecture and Scaling](#modeling-architecture-and-scaling) - Chairs: Julien Launay, Iz Beltagy
  - [Modeling: Metadata](#modeling-metadata) - Chairs: Timo Schick, Nora Kassner
  - [Modeling: Multilinguality](#modeling-multilinguality) - Chairs: Vassilina Nikoulina, Hady Elsahar
  - [Modeling: Prompt engineering](#modeling-prompt-engineering)
  - [Modeling: Retrieve](#modeling-retrieve) - Chair: Nils Reimers
- [Tokenization](#tokenization) - Chairs: Benoît Sagot, Samson Tan
- [Evaluation](#evaluation) - Chairs: Aurélie Névéol, Dan Garrette, Ellie Pavlick, Marine Carpuat, Thomas Scialom, Sebastian Gehrmann, Verena Rieser
  - [Evaluation: Extrinsic Evaluation](#evaluation-extrinsic-evaluation) - Chairs: Thomas Scialom, Verena Rieser, Ehud Reiter
  - [Evaluation: Intrinsic Evaluation](#evaluation-intrinsic-evaluation) - Chairs: Sebastian Gehrmann
  - [Evaluation: Few-Shot Generalization](#evaluation-few-shot-generalization) - Chairs: Ellie Pavlick
  - [Evaluation: Bias, Fairness, and Social Impact](#evaluation-bias-fairness-and-social-impact) - Chairs: Aurelie Neveol
  - [Evaluation: Multilinguality](#evaluation-multilinguality) - Chairs: Dan Garrette & Marine Carpuat
- [Interpretability and interaction/visualization](#interpretability-and-interactionvisualization) - Chair: Hendrik Strobelt, Ryan Teehan
- [Engineering/scaling](#engineeringscaling) - Chairs: Yozh (jheuristic), Max Ryabinin
- [Collaborations with education and research communities](#collaborations-with-education-and-research-communities) - Chairs: Dieuwke Hupkes, François Yvon
- [Carbon footprint](#carbon-footprint) - Chairs: Anne-Laure Ligozat, Canwen Xu, Sasha Luccioni
- [[Meta-Group] Social Impact Across Groups](#meta-group-social-impact-across-groups) - Chair: Karen Fort, Michael McKenna
- [Sharing and accessibility of model and dataset](#sharing-and-accessibility-of-model-and-dataset) - Chair: Thomas Wolf
- [Challenges in the biomedical domain](#challenges-in-the-biomedical-domain) - Chairs: Antoine Neuraz, Jason Fries



## Overview: how to participate, what roles

BigScience is a research workshop and is open to researchers, i.e. people affiliated with a research organization (in academia or industry) and whose day work is for instance (at least in part) to publish papers in peer-review venues, as well as to people whose technical and professional expertise bears relevance to the social aspects of the project.

The organization of the research workshop is not a good place to learn about AI or find mentors as we do not have an internal mentoring program. It’s also not per-se a community for general AI or AGI discussions.

If you are interested in learning about AI/ML or already working on Machine Learning, AI and NLP side projects, note that we plan to organize events for the AI/ML enthusiast community and the general public. You can fill out the following [Google Form](https://docs.google.com/forms/d/e/1FAIpQLSe3gYSfNX6aKFwDVKdp-42w2kAldasdFjMJnHCUTdlgo-5lqQ/viewform) and join the mailing list to be informed about these upcoming public events

You can generally participate in the project as:

* **Advisor (_Everyone is advisor by default when joining_)**
    * _role_: give general scientific/organization advice
    * _time commitment_: light - reading a newsletter every 2 weeks - giving feedback/advice
* **Participant** in a Working Group
    * _role_: joining one of the working groups of the OC (see list below): advising/designing/building the collaborative task (building the dataset/model/tools) or advising/designing/organizing the live events
    * _time commitment_: medium - depend on the chosen task (see details of the working groups below)
* **Chair/co-chair** of a Working Group
    * _role_: the chair(s) is supposed to provide at least the minimal amount of work necessary for having a very bare-bone version of the task. If other members are active in the WG, the chair(s) can mostly coordinate the effort and organise the decision process.
    * _time commitment_: more significant - also depend on the chosen WG
* **Workshop attendant** joining the collaborative task or events (**_To be defined later_**)
    * _role_: participating in the collaborative task in a guided way following guidelines setup by the OC (helping build the dataset, helping build the tools)
    * _time commitment_: up to the attendant - following guidelines of the OC/WG


# <span style="text-decoration:underline;"> 
</span>

### More details on the role of the co-chairs

Each working group has at least one chair (ideally more than 1 person). Here are some details on the chair role and selection.

**The chairs role:**

* chairs are supposed to coordinate the effort in each working group and organise the decision process while letting working group members feel welcome to raise ideas and propose things
* if no-one is active in the working group, chairs are supposed to do at least the minimal amount of work necessary for having a bare-bone version of the task (aka a minimal "fallback", e.g. gathering Common Crawl for the dataset working groups)
* chairs are in charge of making regular summary of the work to share with all and participate in all-chairs-sync meetings
* chairs are in charge of maintaining the on-boarding ressource to have people join the working group
* chairs are responsible to ensure respectful and open discussions in their WG. As such, they should in particular ensure that the [code of conduct](https://docs.google.com/document/d/1EQk7rreycFOafnahL5Go50POxzZ5qocwWYPtCbGtP2M/edit?usp=sharing) is respected.

For the **selection process**, we are trying to have something quite bottom-up keeping in mind that chair’s role are quite essential to the success of the project so there is a validation step and we (Thomas Wolf in particular) may ask people to not join as chairs or step down if there seems to be a discrepancy between the requirements of the role and the current investment of a candidate. Here is the general selection process

* generally asking for self-propositions for chairs or co-chairs in the current document,
* if no one show up the organization working group will reach out to specific people with related skill and interest in participating,
* when additional people want to be chairs, the current chairs should have a voice to agree or not to the additional chairs,
* when a decision needs to be made to select a chair, the Workshop Organization working group will vote a decision,
* in all this process goodwill is assumed and there should be an effort to listen to all arguments but the pragmatic success of the project is also considered more important than specific people interest (in other words “wanting to be a chair does not guarantee that you will be a chair and there will be a certain degree of arbitrariness”, I’m sorry in advance).


## Working Groups

Find a list of all collaborators [here](collaborators.md).

# Workshop organization

### Scope

This working group is in charge with generally defining how the collaboration could be structured (as a workshop) and organizing the live events and activities not directly related to the collaborative tasks during the one year duration of the workshop as well as communication tools (newsletters, forum, etc).


### Resources - onboarding - documentation

Folder on the google drive: [Organization](https://drive.google.com/drive/folders/1DkTnYMhha3H8NrAFQkoq-MvZUc5SPHcJ?usp=sharing)

This folder includes past newsletters summarizing the evolution of the project as well as general organizational documents and documents related to the live events and other activities not directly related to the collaborative tasks.


### Current members:

Matthias Gallé, Angela Fan, Y-Lan Boureau, Hendrik Strobelt, Verena Rieser, Thomas Wolf, Victor Sanh, Yacine Jernite, Suzana Ilic, Sebastian Gehrmann, Ellie Pavlick, Shubham Agarwal, Meheresh Masanpally


### Current chair(s)

Angela Fan, Matthias Gallé and Suzana Ilić


### Current status

This working group is leading organizational aspects of BigScience, discussing the general workshop setup, inviting members to the workshop, discussing with (public and private) compute providers, setting up events and collaborations.


# Dataset creation


### Scope

The Dataset Creation effort is concerned with the creation of a large multilingual dataset. It is further split into 3 distinct working groups:

- [Data Governance and Archival Strategies](#data-governance-and-archival-strategies)
- [Data Sourcing and Representativeness](#data-sourcing-and-representativeness)
- [Data Tooling: from Data Sources to Training Dataset](#data-tooling-from-data-sources-to-training-dataset)

### Resources - onboarding - documentation

* Folder on the google drive: [Dataset documents](https://drive.google.com/drive/folders/1tpXx_vP_m6pfbTEKJ5MCQ-N3Sid4fHjL?usp=sharing)
* Entry document: [BigScience Data Section](https://docs.google.com/document/d/1BIIl-SObx6tR41MaEpUNkRAsGhH7CQqP_oHQrqYiH00/edit?usp=sharing)

### Current Area Chair(s)

Yacine Jernite

# Data Governance and Archival Strategies

### Scope

This working group is tasked with exploring questions about how data is gathered and managed, choosing the right metadata and indexing and documentation structure, and developing protocols to ensure that data is used while respecting the rights and for the benefit of the data subjects.

* Defining a management and ownership structure for the dataset
* Scoping out legal concerns and societal impact of data choices
* Providing recommendations for how the above should affect the indexing, metadata, sourcing, and data maintenance infrastructure

### Resources - onboarding - documentation

Entry document: [Dataset Org: Data Governance and Archival Strategies](https://docs.google.com/document/d/1BIIl-SObx6tR41MaEpUNkRAsGhH7CQqP_oHQrqYiH00/edit#heading=h.phj215kefz6k)


### Current members

Karën Fort, Guillaume Klein, Samson Tan, Jordi Armengol-Estapé, Yacine Jernite, Félicien Vallet, Luca Soldaini, Alison Callahan, Madhulika Srikumar, Stella Biderman, Alicia Nobles, Anouk Ruhaak, Zeerak Waseem, Huu Nguyen, Jesse Dodge, Gérard Dupont, Shanya Sharma, Maraim Masoud, Benoît Sagot, Marta Villegas, Nicolas Hervé, Pedro Ortiz Suárez, Filip Ginter, Sebastian Nagel, Trieu Le, Michael McKenna


### Current chair(s)

Huu Nguyen, Yacine Jernite, Meg Mitchell


### Current status

Scoping out further collaborative tasks within the group.


# Data Sourcing and Representativeness


### Scope

This working group is responsible for helping define language choices and local and global representativeness criteria, analysing the diversity of existing text sources for each region in terms of social contexts represented, and finding diverse sources of text to meet these criteria, including both online and offline text in all available media.



* Defining frameworks for analysing representativeness and diversity across regions
* Exploring different modes of data collection from web crawling to participatory methods and collaboration with existing data organizations
* Choosing languages, defining language varieties, and identifying relevant regions for each of those
* Identifying diverse text sources for each region and language variety


### Resources - onboarding - documentation

Entry document: [Dataset Org: Data Sourcing and Representativeness](https://docs.google.com/document/d/1BIIl-SObx6tR41MaEpUNkRAsGhH7CQqP_oHQrqYiH00/edit#heading=h.osyu638cv76c)


### Current members 

Karën Fort, Sam Bowman, Halil Akin, Caiming Xiong, Guillaume Klein, Samson Tan, Myle Ott, Philippe Muller, Ruiqi Zhong, Luke Zettlemoyer, Yacine Jernite, Wietse de Vries, Max Ryabinin, Antoine Neuraz , Tsvetomila Mihaylova, Hady Elsahar, Manan Dey, Shanya Sharma, Minh Quang Pham, Jin Koay, Ari Jankelowitz, Elizabeth Keleshian，Shiyue Zhang, Evan Dufraisse, Edoardo M. Ponti, Han Wang, Ona de Gibert Bonet, Zaid Alyafeai, Md Rabiul Awal, Kaustubh Dhole, Jonathan Chang, Maximin Coavoux, Adrian Popescu, Maraim Masoud, Ben Peters, Tasnim Mohiuddin, Rabin Banjade, Vinay Uday Prabhu, Aitor Soroa, Trishala Neeraj, Luca Soldaini, Rodrigo Wilkens, Canwen Xu, Sheng Shen, Michael McKenna, Rishi Bommasani, Patrick Drouin, Fredrik Olsson, Sadid A. Hasan, Francesco De Toni, Huu Nguyen, Laurent Besacier, Nicolas Hervé, Ludovic Tanguy, Benoît Sagot, Salomey Osei, Alham Fikri Aji, Filip Ginter, Sampo Pyysalo, Gérard Dupont, Aakanksha Naik, Olivier Nguyen, Trieu Le, Emily Reif, Tolga Bolukbasi


### Current chair(s)

Angie McMillan-Major, Pedro Ortiz Suárez, Zeerak Waseem


### Current status

Scoping out further collaborative tasks within the group.


# Data Tooling: from Data Sources to Training Dataset


### Scope

This working group will develop tools to gather text from the identified sources and process it to be both easy to use at training time and respectful of the data subjects’ rights. This includes tools for crawling, automatic PI detection and de-identification, documentation of web content, efficient web text formats that retain the website and page structure, tools for extracting text from audio or pdf files, as well as infrastructure for securely maintaining and dispensing the data for training.


### Resources - onboarding - documentation

Entry document: [BigScience Data Tooling Working Group](https://docs.google.com/document/d/1qur5PoDhj8_qIyngz5p4FGckAye_ym58Phoz5JqgNx8/edit?usp=sharing) (see also [Dataset Org: from Data Sources to Training Dataset](https://docs.google.com/document/d/1BIIl-SObx6tR41MaEpUNkRAsGhH7CQqP_oHQrqYiH00/edit#heading=h.113b8ppgbnyc))


### Current members

Benoit Dal Ferro, Xavier Tannier, Halil Akin, Pasquale Minervini, Antoine Simoulin, Shubham Agarwal, Yozh, Yacine Jernite, Max Ryabinin, Wietse de Vries, Hady Elsahar, Manan Dey, Shanya Sharma, Sampo Pyysalo, Veronika Laippala, Logesh Kumar Umapathi, Archiki Prasad, Elizabeth Keleshian, Shiyue Zhang, Fatma Tarlaci, Tal Perry, Ona de Gibert Bonet, Gunjan Chhablani, Madison May, Christophe Cerisara, Jonathan Chang, Arnaud Stiegler, Laurent Besacier, Nicolas Hervé, Tasnim Mohiuddin, Filip Ginter, Vinay Uday Prabhu, Trishala Neeraj, Matteo Manica, Tosin Adewumi , Rishi Bommasani, Fredrik Olsson, Sadid A. Hasan, Huu Nguyen, Gérard Dupont, Antoine Laurent, Salah Aït-Mokhtar, David I. Adelani, Dimitrios Christofidellis, Shamsuddeen Muhammad, Gabriel Ilharco, Alberto Bégué, Sebastian Nagel, Alessandro Suglia, Trieu Le, Emily Reif, Tolga Bolukbasi


### Current chair(s)

Colin Raffel, Albert Villanova, Sampo Pyysalo, Filip Ginter


### Current status

Scoping out further collaborative tasks within the group.



# Modeling approach


### Scope

The high level goal is to answer in natural language any prompted query expressed in natural language in a 0-shot manner:



* (a) Defining the prompted data creation and training procedure to make prompting less “accidental” than in GPT3
* (b) Looking at untapped sources of signal such as metadata and context and potential tools (such as retrieval) to include these signals
* (c) Adapting these in the context of multilinguality
* (d) Implementing and potentially small shared manual labor to create prompting instances
* (e) Coordinating with dataset and engineering working groups and training the beast
* (f) Coordinating with the evaluation working group to evaluate the trained model(s)


### Resources - onboarding - documentation

Folder on the google drive: [Modeling documents](https://drive.google.com/drive/folders/1FgoKJwVrwnTREYF2WFrwgNIdtQuk-_Cu?usp=sharing) and in particular the [Entry point document](https://docs.google.com/document/d/1RXGEzTvYQ4hk9FEw-GjtyaQyGU9fQRpGTWopA7nBxp0/edit?usp=sharing)


### Current members

Stephen Bach, M Saiful Bari, Stas Beckman, Iacer Calixto, Marine Carpuat, Joe Davison, Thibault Févry, Karën Fort, Jason Fries, Matthias Gallé, Claire Gardent, Braden Hancock, Yacine Jernite, Francois Lagunas, Veronika Laippala, Teven Le Scao, André Martins, Aurélie Névéol, Pierre-Yves Oudeyer, Matt Peters, Sampo Pyysalo, Colin Raffel, Nazneed Rajani, Verena Rieser, Sasha Rush, Victor Sanh, Timo Schick, Samson Tan, Eric Wallace, Thomas Wolf, Chen Xing, Caiming Xiong, Canwen Xu, Francois Yvon, Alexandre Allauzen, Yozh (jheuristic), Patrick Lewis, Peter Bloem, Josep Crego, Max Ryabinin Mohamed Ahmed, Manan Dey, Shanya Sharma, Iiro Rastas, Minh Quang Pham, Jean-Baptiste Cordonnier, Thijs Vogels, Ryan Teehan, Akash Mehra, Sandip Patil, Ruochen Zhang, Logesh Kumar Umapathi, Jonathan Berant, Xiang Zhou, Archiki Prasad, Fatma Tarlaci, Antoine Bosselut, Edoardo M. Ponti, Nicola De Cao, Han Wang, Pasquale Minervini, Marius Mosbach, Nils Reimers, Eliza Szczechla, Germán Kruszewski, Patrick Fernandes, Albert Webson, Arnaud Stiegler, Tian Yun, Leandro von Werra, Gunjan Chhablani, Madison May, Christophe Cerisara, Iz Beltagy, Md Rabiul Awal, Pedro Henrique Martins, Olivier Ferret, Sylvain Viguier,Amar Viswanathan, Chenglei Si, Mike Tian-Jian Jiang, Kamalkumar Rathinasamy, Kaustubh Dhole, Jonathan Chang, Mohit Bansal, Luou Wen, Nora Kassner, James Briggs, Roman Castagné, Diwakar Mahajan, Thomas Wang, Yujian Gan, Pawan Sasanka Ammanamanchi,  Jan-Christoph Kalo, Nicolas Chauville, Ben Peters, Abheesht Sharma, Tasnim Mohiuddin, Harshit Pandey, Urmish Thakker, Sushil Bharati, Rabin Banjade, Filip Ginter, Gorka Labaka, Elizabeth Keleshian, Siddharth Karamcheti, Vinay Uday Prabhu, Dimitra Gkatzia, Trishala Neeraj, Vishakha Sharma, Devamanyu Hazarika, Shubham Agarwal, Shannon Shen, Stella Biderman, Nickil Maveli, Sheng Shen, Jesse Dodge, Sadid A. Hasan, Ethan Perez, Stella Biderman, Taewoon Kim, Priyank Soni, Antoine Chaffin, Vikas Raunak, Zaid Alyafeai, Satviki Pathak, Debajyoti Datta, Zheng Xin Yong, Alessandro Suglia, Zhiqing Sun, Haryo Akbarianto Wibowo


### Current Area-chair(s)

Victor Sanh & Stephen Bach


### Current status

Initial experiments (small scale quantitative experiments to compare different options for injecting promoting behaviors) + kick started the sub working groups from the kickoff brainstorming


### Sub working groups

We organized the modeling approach working group into task forces (or sub working groups) around specific questions:

- [Modeling: Architecture and Scaling](#modeling-architecture-and-scaling) - Chairs: Julien Launay, Iz Beltagy
Scope: Comparing and deciding which Transformer architecture would be best. Axis of choices include encoder-decoder/decoder-only/prefix-LM, long range attentions, etc. We are also interested in estimating the best model, data and compute size configuration before scaling to a very large model so that we make the best use of the computational resources.

- [Modeling: Metadata](#modeling-metadata) - Chairs: Timo Schick, Nora Kassner
Scope: Metadata gives information about the situation in which a text was written and is a source of signal we want to squeeze out to condition text on available metadata as an additional source of context. 

- [Modeling: Multilinguality](#modeling-multilinguality) - Chairs: Vassilina Nikoulina, Hady Elsahar
Scope: We are interested in ensuring the model still has non-trivial few/0-shot abilities beyond English.

- [Modeling: Prompt engineering](#modeling-prompt-engineering)
Scope: Inputs alone often don’t contain enough information and providing additional context is required to faithfully react to the prompt without hallucinating or memorizing random things. We are interested in exploring whether a non-parametric component to the model would make sense.

- [Modeling: Retrieve](#modeling-retrieve) - Chair: Nils Reimers
Scope: Inputs alone often don’t contain enough information and providing additional context is required to faithfully react to the prompt without hallucinating or memorizing random things. We are interested in exploring whether a non-parametric component to the model would make sense.



# Modeling: Architecture and Scaling


### Scope

Comparing and deciding which Transformer architecture would be best. Axis of choices include encoder-decoder/decoder-only/prefix-LM, long range attentions, etc. Also, estimating the best model, data and compute size configuration before scaling to a very large model so that we make the best use of the computational resources.


### Resources - onboarding - documentation

Folder on the google drive: [Modeling documents](https://drive.google.com/drive/folders/1FgoKJwVrwnTREYF2WFrwgNIdtQuk-_Cu?usp=sharing)


### Current members

Thomas Wolf, Victor Sanh, Angela Fan, François Lagunas, Teven Le Scao, Sasha Rush, Yacine Jernite, Colin Raffel, Pasquale Minervini, Matthias Gallé, Francois Yvon, Gunjan Chhablani, M Saiful Bari, Timo Schick, André Martins, Suzana Ilic, Stephen Bach, Ryan Teehan, Arnaud Stiegler, Germán Kruszewski, Thomas Wang, Eliza Szczechla, Urmish Thakker, Sushil Bharati, Vinay Uday Prabhu, Vishakha Sharma, Nimshi Venkat Meripo, Ruochen Zhang, Shubham Agarwal, Shannon Shen, Nickil Maveli, Sheng Shen, Matthew Peters, Jesse Dodge, Stella Biderman, Jonathan Chang, Marius Mosbach, Jake Tae, Pawan Sasanka Ammanamanchi, Priyank Soni, Eric Wallace, Matt Peters, Jonathan Berant, Lewis Tunstall, Siddharth Karamcheti, Tasnim Mohiuddin, Trishala Neeraj, Ahmed Baruwa, Jason Phang, Gabriel Ilharco, Canwen Xu, Taewoon Kim, Srulik Ben David, Iacopo Poli, Alberto Bégué, Dimitri Lozeve, Alessandro Suglia, Zhiqing Sun, Sandip Patil


### Current chair(s)

Julien Launay, Iz Beltagy


### Current status

Merged Architecture Design and Scaling Laws into one group, Architecture and Scaling.



# Modeling: Metadata


### Scope

Metadata gives information about the situation in which a text was written and is a source of signal we want to squeeze out to condition text on available metadata as an additional source of context. 


### Resources - onboarding - documentation

Folder on the google drive: [Modeling documents](https://drive.google.com/drive/folders/1FgoKJwVrwnTREYF2WFrwgNIdtQuk-_Cu?usp=sharing)


### Current members

Thomas Wolf, Victor Sanh, Angela Fan, Teven Le Scao, Yacine Jernite, Colin Raffel, Patrick Lewis, Manan Dey, Matthias Gallé, M Saiful Bari, Timo Schick, Suzana Ilic, Stephen Bach, Eliza Szczechla, Kaustubh Dhole, Urmish Thakker, Vishakha Sharma, Shannon Shen, Gérard Dupont, Jonathan Chang, Marius Mosbach, Huu Nguyen, Taewoon Kim, Shanya Sharma, Alessandro Suglia


### Current chair(s)

Timo Schick, Nora Kassner


### Current status

Recently created



# Modeling: Multilinguality


### Scope

We are interested in ensuring the model still has non-trivial few/0-shot abilities beyond English.


### Resources - onboarding - documentation

Folder on the google drive: [Modeling documents](https://drive.google.com/drive/folders/1FgoKJwVrwnTREYF2WFrwgNIdtQuk-_Cu?usp=sharing)


### Current members

Thomas Wolf, Victor Sanh, Angela Fan, Teven Le Scao, Sasha Rush, Yacine Jernite, Colin Raffel, Patrick Lewis, Jonas Pfeiffer, Manan Dey, Matthias Gallé, M Saiful Bari, Nils Reimers, Suzana Ilic, Stephen Bach, Edoardo Ponti, Mohamed Ahmed, Archiki Prasad, Shanya Sharma, Eliza Szczechla, Patrick Fernandes, Tasnim Mohiuddin, Kaustubh Dhole, Urmish Thakker, David Stap, Vinay Uday Prabhu, Vishakha Sharma, Lintang Sutawika, Md Rabiul Awal, Sadid A. Hasan, Iacer Calixto, Ahmed Baruwa, Jonathan Chang, Samson Tan, Bjarke Felbo, Vikas Raunak, M Ali Jauhar, Zheng Xin Yong, Evangelia Gogoulou, Sandip Patil


### Current chair(s)

Vassilina Nikoulina, Hady Elsahar


### Current status

Recently created



# Modeling: Prompt engineering


### Scope

We are interested in the emergence of 0-shot prompting behaviors in very large language models and in making 0-shot prompting abilities more robust.


### Resources - onboarding - documentation

Folder on the google drive: [Modeling documents](https://drive.google.com/drive/folders/1FgoKJwVrwnTREYF2WFrwgNIdtQuk-_Cu?usp=sharing)


### Current members

Thomas Wolf, Victor Sanh, Angela Fan, François Lagunas, Teven Le Scao, Joe Davison, Sasha Rush, Yacine Jernite, Colin Raffel, Pasquale Minervini, Canwen Xu, Iz Beltagy, Manan Dey, Matthias Gallé, Claire Gardent, Pierre-Yves Oudeyer, Eric Wallace, Gunjan Chhablani, M Saiful Bari, Jonathan Berant, Y-Lan Boureau, Braden Hancock, Suzana Ilic, Stephen Bach, Jason Fries, Ruiqi Zhong, Mohamed Ahmed, Peter Bloem, Arnaud Stiegler, Marius Mosbach, Germán Kruszewski, Thomas Wang, Shanya Sharma, Eliza Szczechla, Madison May, Nicolas Chauville, Kaustubh Dhole, Urmish Thakker, Mike Tian-Jian Jiang, Dimitra Gkatzia, Tasnim Mohiuddin, Vishakha Sharma, Ruochen Zhang, Devamanyu Hazarika, Abheesht Sharma, Shannon Shen, Sheng Shen, Michael McKenna, Harshit Pandey, Ethan Perez, Jake Tae, Samira Shaikh, Taewoon Kim, Albert Webson, Priyank Soni, Satviki Pathak, Arun Raja, Debajyoti Datta, Trishala Neeraj, Vikas Raunak, Zheng Xin Yong, Patrick Lewis, Rachel Bawden, Andrea Santilli, Lintang Sutawika, Ryan Teehan, Matteo Manica, Animesh Prasad, Han Wang, Nihal Nayak, Zaid Alyafeai, Fatma Tarlaci, Michael McKenna, Srulik Ben David, Jacopo Staiano, Jonathan Chang, Zhiqing Sun, Kaustubh Dhole, Antoine Chaffin, Jos Rozen, Sandip Patil, Bec Johnson


### Current chair(s)

No chair yet


### Current status

Recently created



# Modeling: Retrieve


### Scope

Inputs alone often don’t contain enough information and providing additional context is required to faithfully react to the prompt without hallucinating or memorizing random things. We are interested in exploring whether a non-parametric component to the model would make sense.


### Resources - onboarding - documentation

Folder on the google drive: [Modeling documents](https://drive.google.com/drive/folders/1FgoKJwVrwnTREYF2WFrwgNIdtQuk-_Cu?usp=sharing)


### Current members

Thomas Wolf, Victor Sanh, Lysandre Debut, Angela Fan, Teven Le Scao, Sasha Rush, Yacine Jernite, Colin Raffel, Patrick Lewis, Matthias Gallé, Minh Quang Pham, M Saiful Bari, Timo Schick, Nils Reimers, Suzana Ilic, Stephen Bach, Nicola De Cao, Marius Mosbach, Thomas Wang, Eliza Szczechla, Madison May, Jan-Christoph Kalo, Urmish Thakker, Siddharth Karamcheti, Tasnim Mohiuddin, Vishakha Sharma, Ruochen Zhang, Devamanyu Hazarika, Nickil Maveli, Iacer Calixto, Nora Kassner, Jonathan Chang, Taewoon Kim, Vikas Raunak, Animesh Prasad, Dimitri Lozeve, Jakub Zavrel, Zhiqing Sun, Manan Dey, Sandip Patil


### Current chair(s)

Nils Reimers


### Current status

Recently created



# Tokenization


### Scope

Define and develop the tokenization used by the model:



* the tokenization algorithm itself
* the tokenization in the context of multilinguality
* implement it and coordinate with the dataset and modeling working groups to prepare the data for training


### Resources - onboarding - documentation

No ressource at the moment


### Current members

M Saiful Bari, Anthony Moi, Victor Sanh, Samson Tan, Francois Yvon, Wietse de Vries, Mohamed Ahmed, Wilson Lee, Sandip Patil, Rico Sennrich, Shiyue Zhang, Maxime De Bruyn, Vassilina NIkoulina, Zaid Alyafeai, Nick Doiron, Ben Peters, Chenglei Si, Mike Tian-Jian Jiang, Kamalkumar Rathinasamy, Kaustubh Dhole, Benoît Sagot, Roman Castagné, Thomas Wang, Uğur Ünal, Md Rabiul Awal, Tasnim Mohiuddin, Rachel Bawden, Elizabeth Keleshian, Manan Dey, Shannon Shen, Sadid A. Hasan, Arun Raja, Priyank Soni, Bjarke Felbo, Sabrina Mielke, Shamsuddeen Muhammad, Taewoon Kim, Zhiqing Sun, Elizabeth Salesky


### Current chair(s)

Benoît Sagot, Samson Tan


### Current status

Kicked off the discussion



# Evaluation


### Scope

This working group focuses on making precise the question: What makes a language model “good”? We aim to:

* Develop standardized measures for evaluating models both 1) relative to some extrinsic gold standard (e.g., human performance/theoretical bounds) and 2) relative to one another
* Design a diverse, multifaceted suite of evaluations that represents 1) the different ways in which people will use language models in practice and 2) the different scientific communities who are interested in the capabilities of language models


### Resources - onboarding - documentation

Our onboarding document is [here](https://docs.google.com/document/d/1emny_1yMaMk_ZPsfnRHQTQZrv_6ke6SmRoIUGIZaP6E/edit?usp=sharing).


### Current members

Laurent Besacier, Iacer Calixto, Marine Carpuat, Joe Davison, Karën Fort, Yacine Jernite, Teven Le Scao, Aurélie Névéol, Verena Rieser, Sasha Rush, Victor Sanh, Thomas Wolf, Francois Yvon, Benoît Crabbé, Pierre Colombo, Marie Candito, Yozh (jheuristic), Wietse de Vries, Maite Melero, Antoine Neuraz, Hady Elsahar, Vassilina Nikoulina, Manan Dey, Shanya Sharma, Philippe Muller, Wilson Lee, Ryan Teehan, Akash Mehra, Eric Wallace, Xiang Zhou, Saad Mahamood, Aline Villavicencio, Archiki Prasad, Jan-Christoph Kalo, Nora Kassner, Shiyue Zhang, Olga Majewska, Chrysoula (Chryssa) Zerva, Taisiya (Taya) Glushkova , Jos Rozen, Maraim Masoud, Yonatan Belinkov, Pierre-Yves Oudeyer, Marius Mosbach, Miruna Clinciu, Albert Webson, Tian Yun, Leandro von Werra, Salah Aït-Mokhtar, Gunjan Chhablani, Md Rabiul Awal, Olivier Ferret, Amar Viswanathan, Mike Tian-Jian Jiang, Kaustubh Dhole, Mohit Bansal, Abhinav Ramesh Kashyap, Caroline Brun, Luou Wen, Debajyoti Datta, Namrata Mukhija, Diwakar Mahajan, Samson Tan, Thomas Wang, Julien Tourille, Andrea Santilli, Nicolas Chauville, Pawan Sasanka Ammanamanchi, Abheesht Sharma, José Hernández-Orallo, Harshit Pandey, Urmish Thakker, Rabin Banjade, Rachel Bawden, Gorka Labaka, Dimitra Gkatzia, Elizabeth Keleshian, Trishala Neeraj, Ruochen Zhang, Alison Callahan, Shubham Agarwal, Jaap Jumelet, Arun Raja, Vered Shwartz, Nickil Maveli, Veronika Laippala, Sadid A. Hasan, Oskar van der Wal, Dan Garrette, Ethan Perez, Rodrigo Wilkens, Ahmed Baruwa, Satviki Pathak, Vikas Raunak, Vincent Claveau, Nafise Sadat Moosavi, Shamsuddeen muhammad, Giada Pistilli, Bec Johnson


### Current chair(s)

Aurélie Névéol, Dan Garrette, Ellie Pavlick, Marine Carpuat, Thomas Scialom, Sebastian Gehrmann, Verena Rieser


### Current status

Our subgroups have continued to refine their focus (see updates below). As a full group, we are working on populating a spreadsheet with an extensive (if not comprehensive) list of existing evaluation resources along with key metadata on the research questions and design decisions underlying each. The goal is to release the resulting spreadsheet to the community as a useful documentary resource, and then use it ourselves as the basis for our baseline evaluation suite. We welcome contributions from the community to the spreadsheet: the dataset tracker is here and the form for submitting new datasets is here.

Our goal is to filter this list down to a small, interpretable set of evaluations that will make up our baseline evaluation suite. We plan to finalize the spreadsheet in the coming week or two, and then spend several weeks finalizing a short list of evaluations. Our intent is for the short list to be “quality over quantity”--we want to include a smaller number of datasets such that changes in performance are easily interpretable, rather than a large number of possibly redundant or highly-correlated metrics of performance.  



# Evaluation: Extrinsic Evaluation


### Scope

Standardize a suite of application-oriented downstream tasks (e.g., Question Answering, Summarization, Machine Translation) on which to evaluate models


### Resources - onboarding - documentation

[Google drive sub-folder for evaluation](https://drive.google.com/drive/folders/1OXbex9ZlafQ5P2NNz2G2ioP4hDjmVFGp?usp=sharing)

[Main on-boarding document](https://docs.google.com/document/d/1emny_1yMaMk_ZPsfnRHQTQZrv_6ke6SmRoIUGIZaP6E/edit?usp=sharing).


### Current members

Shiyue Zhang (she/her), Pawan Sasanka Ammanamanchi (he), Salah Aït-Mokhtar, Julien Tourille, Luou Wen (any), Rachel Bawden, Joe Davison (he/him), Radu Florian, Thomas Scialom, Verena Rieser, Diwakar Mahajan, Sadid A. Hasan, Vered Shwartz, Rabin Banjade, Yacine Jernite, Iacer Calixto, Veronika Laippala, MaraimM, Md Rabiul Awal, Yonatan Belinkov, Samira Shaikh, Vikas Raunak, Vincent Claveau, M Saiful Bari, Miruna Clinciu, Nafise Sadat Moosavi, Ahmed Baruwa, Ksenia Shkaruta


### Current chair(s)

Thomas Scialom, Verena Rieser, Ehud Reiter


### Current status

Recently created


# Evaluation: Intrinsic Evaluation


### Scope

Standardize a suite of evaluations focused on interpretability of internal linguistic representations, including but not limited to linguistic knowledge (syntax, morphology, semantics), commonsense/world knowledge, and visualizations


### Resources - onboarding - documentation

[Google drive sub-folder for evaluation](https://drive.google.com/drive/folders/1OXbex9ZlafQ5P2NNz2G2ioP4hDjmVFGp?usp=sharing)

[Main on-boarding document](https://docs.google.com/document/d/1emny_1yMaMk_ZPsfnRHQTQZrv_6ke6SmRoIUGIZaP6E/edit?usp=sharing).


### Current members

Miruna-Adriana Clinciu, Amar Viswanathan, Reshinth, Nora Kassner (she/her), Inyoung, Gunjan Chhablani (he/him), Harshit Pandey (He/Him), Abheesht Sharma (he/him), Olga Majewska (she/her), Aline Villavicencio (she/her), Jan-Christoph Kalo (he/him), Shubham Agarwal, Jaap Jumelet (he/his), Eleni Metheniti (she/her), Saad Mahamood, Albert Webson, Sebastian Gehrmann, Rishi Bommasani, Sadid A. Hasan, Yanai Elazar, Samira Shaikh, Rodrigo Wilkens, Satviki Pathak, M Saiful Bari, Yonatan Belinkov, Gabriele Sarti, Ksenia Shkaruta


### Current chair(s)

Sebastian Gehrmann


### Current status

Recently created



# Evaluation: Few-Shot Generalization


### Scope

Standardize a set of tasks and procedures for evaluating models’ ability to generalize outside of the training domain/distribution


### Resources - onboarding - documentation

[Google drive sub-folder for evaluation](https://drive.google.com/drive/folders/1OXbex9ZlafQ5P2NNz2G2ioP4hDjmVFGp?usp=sharing)

[Main on-boarding document](https://docs.google.com/document/d/1emny_1yMaMk_ZPsfnRHQTQZrv_6ke6SmRoIUGIZaP6E/edit?usp=sharing).


### Current members

Arun Raja, Trishala Neeraj, Albert Webson (he/they), Md Rabiul Awal (he/him), Pierre Colombo, Urmish Thakker, Mike Tian-Jian Jiang (he/him), Abhinav  Ramesh kashyap, Xiang Zhou (he/him/his), Dimitra GKATZIA, Wilson Lee (he/him), Archiki Prasad (she/her), Andrea Santilli (he/him), Debajyoti Datta, Jose Hernandez-Orallo, Ryan Teehan (he/him), Jos Rozen (he-him), Namrata Mukhija (she/her), Tian Yun (He/Him), Ellie Pavlick, Ruochen Zhang (she/her), Sadid A. Hasan, Yanai Elazar, Jekaterina Novikova, Vincent Claveau, M Saiful Bari, Gonzalo Jaimovitch-López (He/Him,She/Her,They/Them), Aakanksha Naik, Taewoon Kim, Alessandro Suglia


### Current chair(s)

Ellie Pavlick


### Current status

We are working on populating the shared Evaluation WG spreadsheet with datasets that are aimed at evaluating few-shot learning and generalization. Our goal is to begin filtering these datasets to a short list in the following week. We expect that some work will be required to adapt datasets to a few-shot setting (e.g., combining a Wikipedia training set with a biomedical domain test set to test few-shot domain transfer). 



# Evaluation: Bias, Fairness, and Social Impact


### Scope

Standardize a set of tasks and procedures for evaluating models’ biases and risks, with focus on the impact model will have on people if deployed in real-world scenarios.


### Resources - onboarding - documentation

[Google drive sub-folder for evaluation](https://drive.google.com/drive/folders/1OXbex9ZlafQ5P2NNz2G2ioP4hDjmVFGp?usp=sharing)

[Main on-boarding document](https://docs.google.com/document/d/1emny_1yMaMk_ZPsfnRHQTQZrv_6ke6SmRoIUGIZaP6E/edit?usp=sharing).


### Current members

Ioana Baldini, Hady Elsahar (he/him), Rabin Banjade, Verena Rieser (she/her), Samson Tan (he/him) , Brun Caroline, Aurelie Neveol, Diwakar Mahajan, Rishi Bommasani, Oskar van der Wal, Deepa Muralidhar, Maxime Amblard, Jake Tae (he/him), Vincent Claveau, M Saiful Bari, M Ali Jauhar, Marie Candito, Miles Brundage, Debajyoti Datta, Maraim Masoud, Xudong Shen, Miruna Clinciu, Giada Pistilli, Bec Johnson


### Current chair(s)

Aurelie Neveol


### Current status

Recently created



# Evaluation: Multilinguality


### Scope

Interface with all other subgroups to ensure all proposed evaluations cover a sufficient range of languages and language families, and potentially design other evaluations specific to multilinguality


### Resources - onboarding - documentation

[Google drive sub-folder for evaluation](https://drive.google.com/drive/folders/1OXbex9ZlafQ5P2NNz2G2ioP4hDjmVFGp?usp=sharing)

[Main on-boarding document](https://docs.google.com/document/d/1emny_1yMaMk_ZPsfnRHQTQZrv_6ke6SmRoIUGIZaP6E/edit?usp=sharing)


### Current members

Maraim Masoud, Laurent Besacier, Yacine Jernite, Shanya (She/Her), Wietse de Vries (he/him/his), Diwakar mahajan(he/him), Manan Dey (He/Him), Marine Carpuat, Iacer Calixto, Fatma Tarlaci, Lintang Sutawika (He/Him), Evi Gogoulou (she/her), Aline Villavicencio, David I. Adelani, M Saiful Bari, Rachel Bawden, Samson Tan, Md Rabiul Awal, Vassilina Nikoulina, Rabin Banjade, M Ali Jauhar, Ahmed Baruwa, Rui Zhang


### Current chair(s)

Marine Carpuat, Dan Garrette


### Current status

Recently created


# Interpretability and interaction/visualization


### Scope

Developing tools and interactive methods horizontally to the other working groups to:



* help debugging model (see https://exbert.net )
* help identifying bias and mitigate for it
* create interactive prototypes for human-AI generation to test model under human constraints
* encourage to train models with more interpretable latents
* more…


### Resources - onboarding - documentation

Not ressource at the moment


### Current members

Hendrik Strobelt, Terrell Ibanez, Pierre Colombo, Mohamed Ahmed, Ryan Teehan, Ioana Baldini, Yonatan Belinkov, Miruna Clinciu, Eliza Szczechla, Patrick Fernandes, Zaid Alyafeai, Gunjan Chhablani, Mohit Bansal, Debajyoti Datta, Sebastian Gehrmann, Diwakar Mahajan, Luca Moschella, Andrea Santilli, Uğur Ünal, Abheesht Sharma, Urmish Thakker, Sushil Bharati, Trishala Neeraj, Jaap Jumelet, Shannon Shen, Nickil Maveli, Michael McKenna, Matteo Manica, Sara Meftah, Sadid A. Hasan, Taewoon Kim, Satviki Pathak, James Wexler, Rishi Bommasani, Nora Kassner, Manan Dey, Germán Kruszewski, Gabriele Sarti, Vinay Prabhu, Maraim Masoud, Emily Reif, Luciana Benotti, Tolga Bolukbasi, Max Huang


### Current chair(s)

Hendrik Strobelt, Ryan Teehan


### Current status

Kicked off the discussion



## Engineering/scaling


### Scope

A working group focusing on the technical challenges of training at scale on several hundred GPUs and how to make the best use of the (large) compute budget we have.

Note that participating in this working group does not imply that you will have direct access to the supercomputer since there are additional (quite strong) national restrictions on the access to this machine (see some details in the [section on access to compute here](https://docs.google.com/document/u/1/d/1O0Ts3uyRiB6huFmJaUjHDK_S2-e5uWdgj0Esa5Jf2_o/edit)). It does mean however that you will participate in the discussion on these aspects.


### Resources - onboarding - documentation


### Current members

Sean Narenthiran, Stas Bekman, Thomas Wolf, Teven Le Scao, Morgan Funtowicz, Yozh (justheuristic), Max Ryabinin, Jean-Baptiste Cordonnier, Thijs Vogels, Akash Mehra, Antoine Bosselut, Samyam Rajbhandari, Gérard Dupont, Minjia Zhang, guillaume Alleon, Christophe Cerisara, James Briggs, Uğur Ünal, Harshit Pandey, Urmish Thakker, Sushil Bharati, Myriam Peyrounette, Hatim Bourfoune, Hadrien de Dompsure, Kamel Guerda, Siddharth Karamcheti, Laurel Orr, Espoir Murhabazi, Thomas Wang, Luca Moschella, Francois Courteille, Kari Briski, Meriem Bendris, Mohammad Shoeybi, Bryan Catanzaro, Jared Casper, Joey Conway, Sylvain Jeaugey, Camille Parisel, Deepak Narayanan,Bertrand Cabot, Rémi Lacroix, Sampo Pyysalo, Pierre-François Lavallée, Jeff Rasley, Olatunji Ruwase, Pawan Sasanka Ammanamanchi, Vikas Raunak, M Ali Jauhar, Arun Raja, Alberto Bégué, Dimitri Lozeve, Michael Z Wang, Zenodia Charpy, Shaden Smith


### Current chair(s)

Yozh (jheuristic), Max Ryabinin


### Current status



# Collaborations with education and research communities


### Scope

Around the workshop there are many actors with which we could do actions or events for collaborating or raising awareness.

Examples:

* Collaborating with ELLIS for student workshop
* Finding possibilities for early students (masters/licences) to be either involved in some part of the project or work on related projects (e.g. Hackathon)

Also it seems important to make sure we don’t do some unreflected choices which can impact wide access to the workshop for the international community (typical example: selecting a location with VISA restrictions for an in-person event) (could be separated Working Groups).


### Resources - onboarding - documentation


### Current members

Thomas Wolf, Dieuwke Hupkes, Yozh (jheuristic), Omar Sanseviero, Peter Bloem, Manan Dey, Nora Kassner, Andrea Santilli, Maraim Masoud, David Stap, Madhulika Srikumar, Maxime Amblard, Salomey Osei, Ksenia Shkaruta, Yonatan Belinkov


### Current chair(s)

Dieuwke Hupkes, Yozh (jheuristic), François Yvon


### Current status



# Carbon footprint


### Scope

A Working Group interested in evaluating the carbon footprint of the collaborative tasks (model training, inference, evaluation, dataset creation, sharing) and proposing ways to reduce this footprint.

We will be working on this from two angles:

1. We will develop a plugin for transformers to automatically collect data about the energy consumption and carbon emission.
2. We will work together with modeling WG to provide high-quality compressed models (distillation, quantization, pruning etc.) thus can reduce the carbon footprint for downstream practitioners. 


### Resources - onboarding - documentation


### Current members

Thomas Wolf, Anne-Laure Ligozat, Vassilina Nikoulina, Ari Jankelowitz, Elizabeth Keleshian, Han Wang, Sylvain Viguier, Julien Launay, Uğur Ünal, Urmish Thakker, Vishakha Sharma, Benoît Sagot, Michael McKenna, Sheng Shen, Sasha Luccioni, Jesse Dodge, Jake Tae, Anthony Hevia, Wangchunshu Zhou, Manan Dey, Xabier Soto


### Current chair(s)

Anne-Laure Ligozat, Canwen Xu, Sasha Luccioni


### Current status



# [Meta-Group] Social Impact Across Groups


### Scope

While each of the working groups is responsible for considering the prospective social impacts and for researching the relevant social context for its decisions, these aspects of the various tasks cannot be considered in isolation from each other. The purpose of this working group will be to collaborate with each of the others to share skills and knowledge, propose general guidelines, identify common threads and relevant differences across their respective societal questions, and aggregate findings in the context of the overall effort.

This group is intended mostly as a **meta-group** where questions can be raised and discussed.


### Resources - onboarding - documentation


### Current members

Yacine Jernite, Thomas Wolf, Samson Tan, Omar Sanseviero, Peter Bloem, Karen Fort, Aurélie Névéol, Pierre-Yves Oudeyer, Christophe Cerisara, Benoît Sagot, Madhulika Srikumar, Sheng Shen, Rishi Bommasani, Aviv Ovadya, Huu Nguyen, Sasha Luccioni, Meheresh Masanpally, Shanya Sharma, Zeerak Waseem, Taewoon Kim, Pedro Ortiz Suárez, Debajyoti Datta, Maraim Masoud, Xudong Shen


### Current chair(s)

Karen Fort, Michael McKenna


### Current status



# Sharing and accessibility of model and dataset


### Scope

Prepare tools and strategies to make the model easy to use and accessible to the community. 


### Resources - onboarding - documentation


### Current members

Thomas Wolf, Alexandre Allauzen, Benoit Crabbé, Rajaram Sivaramakrishnan, Reshinth Adithyan, Benoît Sagot, Vishakha Sharma, Canwen Xu, Max Huang, Maxime Amblard, Shannon Shen, M Ali Jauhar, Miles Brundage


### Current chair(s)

Thomas Wolf - Happy to welcome co-chairs :)


### Current status


# Challenges in the biomedical domain


### Scope

This transversal WG will focus on questions specifically related to the biomedical domain. It would include (non exhaustive list): data sourcing, modeling, evaluation, interpretability, data privacy,...

 Ideally, it would include people from other WGs.


### Resources - onboarding - documentation


### Current members

Antoine Neuraz, Thomas Wolf, Aurélie Névéol, Vassilina Nikoulina, Salah Aït-Mokhtar, Jason Fries, Olivier Ferret, Diwakar Mahajan, Sushil Bharati, Laurel Orr, Byung-Hak Kim, Vishakha Sharma, Manan Dey, Alison Callahan, Debajyoti Datta, Maya Varma, Michael McKenna, Sadid A. Hasan, Iacer Calixto, Maxime Amblard, Vincent Claveau, Andrey Kormilitzin, Matteo Manica, Aakanksha Naik, Xabier Soto, Dimitri Lozeve


### Current chair(s)

Antoine Neuraz, Jason Fries, Byung-Hak Kim


