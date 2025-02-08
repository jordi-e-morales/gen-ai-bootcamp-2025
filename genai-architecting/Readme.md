# Architecting AI

## Architectural & Design Considerations

### Requirements

#### Business Requirements

An enhancement of the existing Lang Portal is required to provide lang students with resources such as study activities that  aid tutors to complement classes, and allows them to review the student progress through these activities. This would increase students engagement, learning experience and gamification of learning. 

Due to the recent developments of NLP and particularly Generative AI, the hypothesis is that the business requirement can integrate AI-powered systems that provides the capabilities to easily integrate into the system.

#### Functional Requirements

The system must be capable of:
- Enable students with AI-powered activities
- A database of core words that enables the initial language mastery.
- Access to Teachers to review students scores

##### Assumptions

A phased deployment is assumed, starting with an exploratory phase of open-weight, open-source, or subscription-based (paid) models from cloud providers, and further potential development based on locally owned infrastructure due to data governance.

##### Risks

- The lack of knowledge of closed models about their training data could potentially represent a risk on accuracy or bias of generated content. A curation / validation process by a human expert (e.g. native speaker) could provide mitigation of this risk.
- Despite huge development of LLMs, they are propense to Hallucinations. Hence, a proper strategy for prompt engineering should be considered to allow for context management and mitigation of Large Language Model Halucinations.
- LLM parameters can potentially trim or divert the output. Limits to address these risks should be considered, such as context windows, tokens limitations, api calls limitations (e.g. in paid models), etc.
- Unexpected surge of costs due to lack of knowledge of users, generating high input/output tokens and impacting the business model. Limitations to user queries must be considered to mitigate this issue.
