ESA's European Space Operations Centre initiated a project to outline a clear direction for data strategy and AI implementation in mission operations. This initiative led to the creation of the DataX [1] strategy, developed to improve the scalability of advanced analytics applications, including AI systems and to increase the value of data within the organization. One of the key elements of developing an AI system is the security of AI applications addressed within the Assurance for Space Domain AI Applications project and its Catalogue of Security Risks for AI Applications in Space. This competition is based on two real-life AI security threats identified within the project - data poisoning and overreliance for text data [2,3,4].

Story
A company uses LLM(s) to perform operations on its official document (e.g., summarization). Different models are used for this purpose and the history of which model with which setting performed which operation on which document is not strictly tracked.

In the meantime, it was found that sometimes the models malfunction and may provide harmful output (hallucination, hidden triggers changing the facts in the documents). The reason for this behaviour has yet to be discovered, but for now, there is a more critical task - detection, which text is correct (real) and which was changed (fake).

Fortunately, a few days ago, one of your colleagues found out that there is a small set of texts for which there are both real and fake texts available, and for some of them, someone managed to detect which one is real and which is fake. Unfortunately, there is no way to continue the task since the person has gone missing and no code was found.

You are the company's data scientist, who was asked to continue this job and create the algorithm to distinguish between real and fake documents.

Task description
You are provided with a collection of documents. Some of them are real (optimal for the recipient, as close as possible to the hidden original text), and some of them are fake (more or much more distant from the hidden original text). The documents are divided into pairs, one of which is always real and one fake, but there is no specific order in which one is which in a given pair. They were sorted randomly.

The main topic of the documents is research and organization in space-related projects. They may contain information about scientific devices, research outcomes, space-related workshops or interesting people in engineering, science, or even astronauts. The documents are public, but it is not necessary to have online access to complete tasks. Each of the documents has been significantly modified using LLMs. The language of all original documents is English.

Summarizations were made using a standard prompt that is not provided but is not necessary to complete tasks. Note that even for decent models, the summarization may not be satisfying in each case. Tasks are created to distinguish between mostly always good outputs and corrupted outputs, so this should not be an issue.

The texts have been modified in several different ways. Be aware that not all modifications may be provided in public test sets. Therefore, manual solutions or rule-based solutions might not be the best idea.

Data
More details regarding the data are provided in the Data tab.

Code
The competition offers a notebook to reproduce the results of baseline algorithms directly at Kaggle and show sample solution format.
