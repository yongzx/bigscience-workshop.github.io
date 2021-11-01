# Big Science 🌸 Data Governance

## 🐠 Overview

The [Hugging Face](https://huggingface.co/) "[Big Science](pages/index.md)"
project is a year-long workshop that brings together nearly 600 researchers from
50 countries to work together on better understanding Large Language Models (
LLMs)
-- a family of deep learning systems that are trained on considerable amounts of
data to learn statistical properties of language. LLMS have been increasingly
adopted in contemporary language technologies, from Internet search to automatic
translation.

Our goal is to improve the scientific understanding of the capabilities and
limitations of large-scale neural network models in NLP. In doing so, we seek to
create both a multilingual language corpus and an open-source large language
model, open to the scientific community. The
May [MIT Tech Review article by Karen Hao](https://www.technologyreview.com/2021/05/20/1025135/ai-large-language-models-bigscience-project/)
provides an excellent overview of the project in its broader context, and
further details can be found in our recent article in
VentureBeat: [NLP needs to be open. 500+ researchers are trying to make it happen](https://venturebeat.com/2021/07/14/nlp-needs-to-be-open-500-researchers-are-trying-to-make-it-happen/)
.

A core part of this project focuses on creating ethical protocols for Data
Governance, including the collection and management of a training dataset. There
are a wealth of language data sources to draw from to meet the growing needs of
these technologies, but bringing those together to train large models while
giving due consideration to ethical concerns such as **anonymization** (no PII)
, **consent** (if the dataset does include PII), and **contestation** (
individuals can request their information be removed from the dataset), remains
an open problem.

To this end, we are exploring the feasibility of working with a small network of
organizations who are themselves interested in working on aspects of ethical
data governance and can help develop tools and protocols for data collection,
hosting, and management. Together, these organizations serve as “Data
Custodians” for the Big Science project.

### Data Custodians: Overview

We are starting to implement a global collaborative data governance
structure ([as described in this poster](https://drive.google.com/file/d/10pgOzQllHe-EXe5G6t-0pKlkaGJdZSqC/view))
, where “Data Custodians” help to collect and serve the data. Data Custodians
can be further broken down into Data Providers -- institutions collecting and
providing the data -- and Data Hosts -- institutions serving the data. Data
Providers and Data Hosts may be one and the same entity, or may collaborate
together, for example, on data curation

#### Data Providers

Data Providers will work with Data Hosts and other members of Big Science,
including pro-bono legal scholars, on the data collection process. A Data
Provider’s main role is to provide access to data they own or have access to.
This data may come in the form of e.g. web content, digitized books or
scientific articles, audio files such as radio shows or podcasts that can be
transcribed, images of text to be OCR’ed, or any other media containing language
data.

Collaborations between Data Providers and the rest of the Big Science project
will focus on mechanisms for extracting specific kinds of data at a large scale,
and brainstorming on how to share the processed data beyond the Big Science
language model training run. The collaboration is also intended to catalyze the
sharing of all of the processing tools, which may also be useful for Data
Providers’ indexing (e.g., new audio transcripts), or training models of their
own.

We are also working on a long form paper on approaches to data governance in the
context of the emergence of data-driven technology, and are hoping to focus on
Data Providers’ existing models of global data governance.

#### Data Hosts

In collaboration with Big Science Workshop participants, the role of Data Hosts
is to serve their data for at least 1 year. Each data host will serve their
different data, which together will form the input training data for a large
language model. Data Hosts are selected to help serve a diversity of languages.

Additionally, Data Hosts are welcome to work with us on refining the data
governance structure, including:

1. Collecting, obtaining, and/or curating appropriate language data from a
   variety of sources and providers
2. Developing tools to manage, index, and visualize these data sources
3. Developing protocols to make the data available to users and other host
   organizations subject to the rights and requirements of the data creators,
   subjects, and providers

---

In addition to being part of a new approach to handling data in Machine 
Learning, a key benefit of participation is access to the shared 
infrastructure for data
governance.

The questions we still need to iron out are:

4. How can we manage access to the input datasets to most efficiently achieve
   the above goals?
5. How might contestation protocols work, for asking that one’s data be removed?


For more information, please email: meg@huggingface.co, yacine@huggingface.co

