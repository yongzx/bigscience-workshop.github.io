# Frequently Asked Questions (FAQ)

This page gathers the most frequently asked questions about the “BigScience” project and tries to answer them.
This page is still a work in progress (and probably will continue to be as every FAQ).
Note: some of these questions are expected to be explored and further answered in the workshop itself. 

## Why not forming a Consortium?

While the option of creating a consortium should definitely be considered in the future for similar large scale projects, this road was not taken for the present collaboration for a few reasons:

*   Organizing a binding contractual/legal relationship between the +90 entities behind the +200 researchers interested in the project is a daunting task that is currently left for future work ;)
*   Consortium are difficult to be made inclusive and are difficult to keep open over a long time which is a major goal of the present project (being able to welcome new participant along the one year of the project)
*   A workshop is one of the most inclusive collaborations of researchers (and general public) that exists today
*   Consortium make it more difficult to accommodate an open and flexible participation from the public and community which is also a goal of the present projet

Not doing a consortium has some drawbacks though, namely:


*   Contributors are more free to decide the amount of time they dedicate to the project
*   A workshop will have greater ratio of followers versus doers than a consortium
*   Not having a legal entity with a bank account behind the collaboration means it’s not possible to collectively apply for monetary grants


## How will the model and weights be released?

The exact licence and release process for the model, dataset and tools is still to be discussed in the relevant working group. The general goal is to make all the artifacts fully and freely available to the research community.

This means different things for each artifact:

**Model checkpoints (size/license):**

The model and checkpoint and in particular the largest checkpoints should be fully accessible to researchers. Given its anticipated large size, a plan is to develop tools to help make it work on smaller workstations, targeting a single GPU workstation. These (newly developed) tools would typically use CPU offloading, possibly combined with memory-mapping. Currently a 11B parameter model like T5 can already fit and run on a single GPU, thus seems quite possible to have a roughly one order of magnitude larger model run on a single GPU with specially developed tools. The model will likely be slow to run at inference but the underlying assumption of a research model is that researchers have less latency constraints than practitioners and can wait a few tens seconds for a generation.

In addition, a research API giving full access to the model could be designed for researchers without access to even a single GPU but this will involve finding a grant or hosting solution to provide for the GPU or TPU backing such free access for the community.

**Dataset access:**

Like for the model, access to the dataset is

Depending on the conclusion of the working group on dataset, access to the dataset 


## Why a model and dataset for research? Can I use it in production?

This particular research workshop is directed by research community and the research questions surrounding the creation and usage of large language models in practice (zero-shot behavior, evaluation, strength and limitations, bias concerns, memorization versus generalization, out-of-domain behavior) are of paramount importance. 

While these models may have application and some companies are already offering commercial offers based on them, the founding idea of this project is that: used without careful analysis and understanding --- of the data, the model, and the predictions of such models --- can easily perpetuate harms. These harms are not yet fully understood, particularly as new applications of large language models could be discovered in the near future. Our goal is to enable the research community to participate in the creation and analysis of these models, to allow for stronger understanding and the development of safer technology. For now, we do not recommend the usage of these models in production without first understanding the societal effects they could have.  


## Will several models and/or dataset be created - will there be distilled or smaller versions of the model?

All these question are currently discussed and not answered. Though given the size targeted for the model it is already pretty clear that only on single main large model will be trained. Distilling or sharing smaller version of the model could be investigated, keeping in mind that the general research goal of the workshop/project. 

## How is this energy efficient? Why not smaller models?


## What would happen if some participants don’t finish the task they promised to do?


## How is the access to the compute facilities/providers handled?


## How is the decision making process handled?


## Which languages will be in the dataset?


## Who is behind this initiative?


## Could the model, whose creation is proposed during the shared task, be a multimodal model?


## How can I help, what can I do?

