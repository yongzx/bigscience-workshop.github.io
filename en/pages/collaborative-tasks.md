# Collaborative tasks

Note: The workshop involves a set of **collaborative tasks** conducted along the year and aimed at creating, sharing and evaluating a large multilingual dataset and a large language model as tools for research. The collaborative tasks are quite large since they involve several millions GPU hours on a supercomputer.

The goal of the collaborative tasks is in particular to collaboratively create and share several **artifacts** as tools for the research community:



*   A **Multilingual Dataset** for Research (possibly full-open-access, possibly behind an authentication access portal to follow GdPR and data privacy legislations => to be defined by the organization committee in charge of this artifact)
*   A **large Language Model** for Research (possibly full-open-access, possibly behind a researcher’s authentication access portal like the dataset => to be defined by the organization committee in charge of this artifact)
*   **Software tools** created to complete the shared tasks, e.g. dataset filtering, model off-loading, etc (under very permissive licence, e.g. Apache2 => to be by the organization committee in charge of this artifact)
*   Extensive **documentation** of the evaluation results, protocols, approach, datasets, and tools developed in the course of the project for future reconduction



## Workshop organization


### Scope

This working group is in charge with generally defining how the collaboration could be structured (as a workshop) and organizing the live events and activities not directly related to the collaborative tasks during the one year duration of the workshop as well as communication tools (newsletters, forum, etc).


### Resources - onboarding - documentation

Folder on the google drive: [Organization](https://drive.google.com/drive/folders/1DkTnYMhha3H8NrAFQkoq-MvZUc5SPHcJ?usp=sharing)

This folder includes past newsletters summarizing the evolution of the project as well as general organizational documents and documents related to the live events and other activities not directly related to the collaborative tasks.


### Current members:

Matthias Gallé, Angela Fan, Y-Lan Boureau, Hendrik Strobelt, Ellie Pavlick, Verena Rieser, Thomas Wolf, Victor Sanh, Yacine Jernite, Suzana Ilic, Sebastian Gehrmann


### Current chair(s)

Angela Fan and Matthias Gallé


### Current status

Currently planning the tools (website + forum), organizing the first kick-off live event, discussing the general workshop setup, inviting members to the workshop, discussing with (public and private) compute providers


## Dataset creation


### Scope

The Dataset Creation effort is concerned with the creation of a large multilingual dataset. It is further split into 3 distinct working groups:



1. [Data Governance and Archival Strategies](#heading=h.fl61nnxqupav)
2. [Data Sourcing and Representativeness](#heading=h.c1khgych4q5f)
3. [Data Tooling: from Data Sources to Training Dataset](#heading=h.dve77z191wyy)


### Resources - onboarding - documentation



*   Folder on the google drive: [Dataset documents](https://drive.google.com/drive/folders/1tpXx_vP_m6pfbTEKJ5MCQ-N3Sid4fHjL?usp=sharing)
*   Entry document: [BigScience Data Section](https://docs.google.com/document/d/1BIIl-SObx6tR41MaEpUNkRAsGhH7CQqP_oHQrqYiH00/edit?usp=sharing)


### Current chair(s)

Yacine Jernite


## Data Governance and Archival Strategies


### Scope

This working group is tasked with exploring questions about how data is gathered and managed, choosing the right metadata and indexing and documentation structure, and developing protocols to ensure that data is used while respecting the rights and for the benefit of the data subjects.



1. Defining a management and ownership structure for the dataset
2. Scoping out legal concerns and societal impact of data choices
3. Providing recommendations for how the above should affect the indexing, metadata, sourcing, and data maintenance infrastructure


### Resources - onboarding - documentation

Entry document: [Dataset Org: Data Governance and Archival Strategies](https://docs.google.com/document/d/1BIIl-SObx6tR41MaEpUNkRAsGhH7CQqP_oHQrqYiH00/edit#heading=h.phj215kefz6k)


### Current members

M Saiful Bari, Guillaume Klein, Samson Tan, Jordi Armengol-Estapé, Yacine Jernite


### Current chair(s)

(Yacine Jernite)


### Current status

Scoping out further collaborative tasks within the group.


## Data Sourcing and Representativeness


### Scope

This working group is responsible for helping define language choices and local and global representativeness criteria, analysing the diversity of existing text sources for each region in terms of social contexts represented, and finding diverse sources of text to meet these criteria, including both online and offline text in all available media.



1. Defining frameworks for analysing representativeness and diversity across regions
2. Exploring different modes of data collection from web crawling to participatory methods and collaboration with existing data organizations
3. Choosing languages, defining language varieties, and identifying relevant regions for each of those
4. Identifying diverse text sources for each region and language variety


### Resources - onboarding - documentation

Entry document: [Dataset Org: Data Sourcing and Representativeness](https://docs.google.com/document/d/1BIIl-SObx6tR41MaEpUNkRAsGhH7CQqP_oHQrqYiH00/edit#heading=h.osyu638cv76c)


### Current members

Sam Bowman, Halil Akin, Caiming Xiong, Guillaume Klein, Samson Tan, Myle Ott, Philippe Muller, Ruiqi Zhong, M Saiful Bari, Luke Zettlemoyer, Yacine Jernite


### Current chair(s)

(Yacine Jernite)


### Current status

Scoping out further collaborative tasks within the group.


## Data Tooling: from Data Sources to Training Dataset


### Scope

This working group will develop tools to gather text from the identified sources and process it to be both easy to use at training time and respectful of the data subjects’ rights. This includes tools for crawling, automatic PI detection and de-identification, documentation of web content, efficient web text formats that retain the website and page structure, tools for extracting text from audio or pdf files, as well as infrastructure for securely maintaining and dispensing the data for training.


### Resources - onboarding - documentation

Entry document: [Dataset Org: from Data Sources to Training Dataset](https://docs.google.com/document/d/1BIIl-SObx6tR41MaEpUNkRAsGhH7CQqP_oHQrqYiH00/edit#heading=h.113b8ppgbnyc)


### Current members

Benoit Dal Ferro, Xavier Tannier, Halil Akin, Julien Launay, Pasquale Minervini, Antoine Simoulin, Shubham Agarwal, M Saiful Bari, Yozh, Yacine Jernite


### Current chair(s)

(Yacine Jernite)


### Current status

Scoping out further collaborative tasks within the group.


## Modeling approach


### Scope

The high level goal is to answer in natural language any prompted query expressed in natural language in a 0-shot manner:



*   (a) Defining the prompted data creation and training procedure to make prompting less “accidental” than in GPT3
*   (b) Looking at untapped sources of signal such as metadata and context and potential tools (such as retrieval) to include these signals
*   (c) Adapting these in the context of multilinguality
*   (d) Implementing and potentially small shared manual labor to create prompting instances
*   (e) Coordinating with dataset and engineering working groups and training the beast
*   (f) Coordinating with the evaluation working group to evaluate the trained model(s)


### Resources - onboarding - documentation

Folder on the google drive: [Modeling documents](https://drive.google.com/drive/folders/1FgoKJwVrwnTREYF2WFrwgNIdtQuk-_Cu?usp=sharing)


### Current members

Stephen Bach, M Saiful Bari, Laurent Besacier, Stas Beckman, Iacer Calixto, Marine Carpuat, Joe Davison, Thibault Févry, Karën Fort, Jason Fries, Matthias Gallé, Claire Gardent, Braden Hancock, Yacine Jernite, Francois Lagunas, Veronika Laippala, Teven Le Scao, André Martins, Aurélie Névéol, Pierre-Yves Oudeyer, Matthew Petters, Sampo Pyysalo, Colin Raffel, Nazneed Rajani, Verena Rieser, Sasha Rush, Victor Sanh, Timo Schick, Samson Tan, Eric Wallace, Thomas Wolf, Chen Xing, Caiming Xiong, Canwen Xu, Francois Yvon


### Current chair(s)

Victor Sanh


### Current status

Implementing and running 1st small scale quantitative experiments to compare different options for injecting promoting behaviors


## Tokenization


### Scope

Define and develop the tokenization used by the model:



1. the tokenization algorithm itself
2. the tokenization in the context of multilinguality
3. implement it and coordinate with the dataset and modeling working groups to prepare the data for training


### Resources - onboarding - documentation

Not ressource at the moment


### Current members

M Saiful Bari, Anthony Moi, Victor Sanh, Samson Tan, Francois Yvon


### Current chair(s)

Benoît Sagot, Djamé Seddah


### Current status

Kicked off the discussion  - need to find a chair


## Evaluation


### Scope

Developing the evaluation protocols and tools:



1. intrinsic performance measures such as perplexity across languages
2. extrinsic task-based measures (0/few shot prompting scenarios on downstream tasks, fine-tuning, etc.)
3. impact measures from the perspective of fairness, toxicity, safety, inclusion, etc. 
4. human/cognitive measures (e.g. psycholinguistic tasks)
5. extending these evaluations beyond English
6. implement these (or integrate with existing resources) and coordinate with the modeling working group to evaluate the model


### Resources - onboarding - documentation

Not ressource at the moment


### Current members

Laurent Besacier, Iacer Calixto, Marine Carpuat, Joe Davison, Karën Fort, Sebastian Gehrmann, Yacine Jernite, Teven Le Scao, Aurélie Névéol, Ellie Pavlick, Verena Rieser, Sasha Rush, Victor Sanh, Thomas Wolf, Francois Yvon


### Current chair(s)

No chair/co-chairs at the moment


### Current status

Kicked off the discussion. Relying on EleutherAI’s harness for the first small scale experiments  - need to find a chair - probably split the Working Group in several


## Visualization and Interaction


### Scope

Developing tools and interactive methods horizontally to the other working groups to:



1. help debugging model (see https://exbert.net )
2. help identifying bias and mitigate for it
3. create interactive prototypes for human-AI generation to test model under human constraints
4. encourage to train models with more interpretable latents
5. more…


### Resources - onboarding - documentation

Not ressource at the moment


### Current members

Sebastian Gehrmann, Hendrik Strobelt


### Current chair(s)

Hendrik Strobelt


### Current status

Kicked off the discussion


## Proposal for New Working Groups

Here you can propose new Working Groups. Feel free to propose yourself as a Chair or just propose a Working Groups idea. You can feel a-minima the “Scope”.


## Engineering/scaling


### Scope

A working group focusing on the technical challenges of training at scale on several hundred GPUs and how to make the best use of the (large) compute budget we have.

Note that participating to this working group does not imply that you will have direct access to the supercomputer since there are additional (quite strong) national restrictions on the access to this machine (see some details in the [section on access to compute here](https://docs.google.com/document/u/1/d/1O0Ts3uyRiB6huFmJaUjHDK_S2-e5uWdgj0Esa5Jf2_o/edit)). It does mean however that you will participate in the discussion on these aspects.


### Resources - onboarding - documentation


### Current members

Sean Narenthiran, Stas Bekman, Thomas Wolf, Teven Le Scao, Morgan Funtowicz


### Current chair(s)


### Current status


## Inclusion and research community collaborations


### Scope

Around the workshop there are many actors with which we could do actions or events for collaborating or raising awareness.

Examples:



*   Collaborating with ELLIS for student workshop
*   Finding possibilities for early students (masters/licences) to be either involved in some part of the project or work on related projects (e.g. Hackathon)

Also it seems important to make sure we don’t do some unreflected choices which can impact wide access to the workshop for the international community (typical example: selecting a location with VISA restrictions for an in-person event) (could be separated Working Groups).


### Resources - onboarding - documentation


### Current members

Thomas Wolf (currently opening the idea, happy to welcome other interested members :)


### Current chair(s)


### Current status


## Carbon footprint


### Scope

A Working Group interested in evaluating the carbon footprint of the collaborative tasks (model training, inference, evaluation, dataset creation, sharing) and proposing ways to reduce this footprint.


### Resources - onboarding - documentation


### Current members

Thomas Wolf (currently opening the idea, happy to welcome other interested members :)


### Current chair(s)


### Current status


## Social Impact Across Groups


### Scope

While each of the working groups is responsible for considering the prospective social impacts and for researching the relevant social context for its decisions, these aspects of the various tasks cannot be considered in isolation from each other. The purpose of this working group will be to collaborate with each of the others to share skills and knowledge, propose general guidelines, identify common threads and relevant differences across their respective societal questions, and aggregate findings in the context of the overall effort.


### Resources - onboarding - documentation


### Current members

Yacine Jernite (proposal, this working group is looking for organizers)


### Current chair(s)


### Current status

