# NAIRR AI - Workshop notes

_04/02/25_
## Introductory Remarks (8:45am-9:15am)

First workshop for the program. The organizers expected around 100 applicants for support, and got 768. Selectees where evaluated and chosen depending on their.
NAIRR is a pilot program that started its inception during Trump 1, then came to life during Biden and it's been acknowledged by Trump 2.

> The people in this room are the future of AI in this country. - Marin Stanek, UC Boulder CIO

Party crashers aren't welcome! Folks here who didn't register will be escorted out.

## Intermediate Track

__Getting Access to NAIRR Pilot Resources (9:15am-10:00am)__ 

- We will cover proposal preparation, submission, matching resources and follow up support.
- The program is still a pilot, but the horizon for a long term funded project looks great.
- Check the website for the rapdly changing resources available
- The available resources are enumerated in the `Available Resources` (Nvidia DGX Rack)
- Important to request an allocation in the units specific to the desired resource
- Classroom educator resources available for __US based educators and researchers__ for __US based students__. They have to be physically in the US, but not necessarily US citizens.
- Proposals accepted any time. Review happens right away, awards notified within 3 months, but that amount of time is decreasing.
- PIs are required to demonstrate progress frequently
- Research products are expected to be publicly available as open source software
- Not required to have existing funding, but existing funding will help because it demonstrates that the work has already been peer reviewed.
- Projects have to be completed within 12 months. For larger scoped prohects, just propose the compute part and make it fit within that time frame.
- Existing allocations are shown in the website, so that we can learn from them.
- Proposal is for a hardware allocation, not as a scientific project.
- Proposals that aren't accompanied by funding will have more scrutinity on the scientific merit
- It is imporant that the project is ready to be run in an allocation, including data and code
- Compare different performance on different GPUs in the proposal
- Office hours available to clarify the available resources
- Smaller allocations availabel for testing
- Number 1 pitfall is not providing enough detail about the requested allocation resources. Show your work! Number 2: demonstrate that the team is ready to be using the resources.

__Computational resources for AI (10:00am-10:30am)__

This session was a brief description of all the resources for research and education through NAIRR

- All resources in NAIRR have no cost for you
- Available to people affiliated with 2 an 4 years institutions
- Important to disclouse if research are backed by a funding grant
- Resources available from NSF ACCESS
- Anything within the Amazon, Google and Azure cloud catalgos is available through NAIRR
- Nvidia DGX is no longer available 😭
- There are other alternative options to request resources. See the slides to find them

__Machine Learning vs Deep Learning (10:45am-12:15pm)__

This is a hands on session about running models on some of the super computing clusters. It started with an introductory definition of Machine Learning, then we spinned up a jupyter lab instance in one HPC to run a notebook.

__AWS Tools Showcase (1:00pm-2:45pm)__

We got a description of AWS' array of services. Then we did a hands on demo of sage maker
Bedrock seems to be the one better suited to scale infrastructure.
- Bedrock supports RAG workflows implicitly based on knowledge bases created by the users (Relevant to AI Verde)
- Bedrock supports running agents on the server side.
- AWS has a free jupyter lab environment called studiolab. https://studiolab.sagemaker.aws/

Sagemaker Studio has a nicely integrated JupyterLab that is intertwined with their own suite of services, such as S3, SageMaker, etc. This allows for integrated submission of jobs and data and configuration of endpoints right on the spot.

__AI Using Large Language Models (LLMs) (3:00pm-4:30pm)__
We started with a technical explanation of the transformer architecture, used as a building block in LLMs.
Followed by a list of use cases where LLM shines. Such as document summarization, sentiment analysis, machine translation, etc.
Then, a very detailed description on how to run an LLM yourself, how to accomodate an LLM using quantization, how to find the appropriate model, etc.

Jetstream 2 offers two llms: Llama 3.3 70B and Deepseek R1 671B through OpenWebUI. Anyone with an ACCESS CI account can access it, as well as the OpenAI API access. In the near future, access might be restricted to people who have a JS2 allocation.

I must say that DeepSeek R1 ran really fast during the demo.

__Lightning talks (4:30pm-5:30pm)__

Industry partners explain their offerings for 6 min each.

#### Cerebras System
- Available through three distinct NAIRR offerings
- Hardware company that manufactures their own accelerators
- Scalable architecture
- Supports standard tooling, i.e. PyTorch. Their compiler handles the kernels internally

#### CloudBank.org

They manage the access to commercial clouds on behalf of NSF and the NAIRR Pilot.

#### Google

Pitch about how they offer their cloud resources for free through NAIRR.

#### SambaNova Cloud

Another provider of AI accelerators. They specialize on inference and provide their hardware through a cloud offering through NAIRR. Could be good to shift inference to a dedicated provider and use HPC and other cloud services for training.

---
_04/03/25_

__Introduction to PyTorch (9:15am-10:45am)__
PyTorch provides two main components:
1. Tensor library that supports GPU acceleration
2. Neural network support through auto-grad

Brief tour over the properties of PyTorch tensors: data type, device, tensor arithmetic, broadcasting rules.
Brief tour over the neural network utilities and autograd functionality.

There was a hands on session running a jupyter notebook on the Expanse HPC cloud from SDSC.
