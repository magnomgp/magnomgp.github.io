---
layout: post
title: Accelerating global roll-outs with a strategic core model approach
categories: [Strategize, Lifecycle Services, Data Management]
---
Achieving a successful global ERP roll-out hinges on meticulous coordination among teams, processes, and plans. By optimizing processes and developing a comprehensive toolkit, we can expedite the deployment of new regions or business units. This strategic approach is the cornerstone of attaining success and capitalizing on the advantages of economies of scale.

## Core Model
Developing a core model strategy involves pinpointing a specific region or legal entity that can serve as a model for upcoming regions or business unit rollouts. This initial instance, often referred to as the pilot, will encompass a set of business processes and configurations that will be deemed as the benchmark for subsequent implementations.

The chosen legal entity for reference should originate from a region with minimal customizations and specific legal demands, maximizing its core attributes. By establishing this pilot, we not only define a precise implementation script but also simplify estimating rollout schedules. Moreover, this practice streamlines subsequent implementations, as the core model toolkit will readily apply pre-existing processes and configurations, akin to a standard copy-and-paste approach.

## Toolkit
With Dynamics 365 Finance and SCM, we can use their built-in tools to create a toolkit for the core model deployment. First up, we employ the Business Process Modeler (BPM), which I discussed in my recent post "[The Power of Leveraging a Quality BPM Library](https://magnomgp.github.io/the-power-of-leveraging-a-quality-BPM-library/)" – check it out for more details. In a nutshell, we document all the standard core processes in BPM, including task records for user training and test case generation.

When the next rollout comes around, we just circle back to this core model library. We connect it to the specific implementation and legal entity. It's like hitting the streamline button – from business processes to whipping up training materials and running the necessary tests.

After that, we can turn to data management to put together data packages containing the core model's configuration data. This also involves crafting templates for migrating both master and transactional data. To keep things organized, it's important to set up a data entities management matrix. This matrix helps us track and plan the application of the data packages.

Another approach to gather the configuration involves setting up a designated DAT legal entity. This entity serves as a storage hub for configuration data. We can then make use of the "Copy into legal entity" feature within Data Management. This lets us efficiently transfer the required settings.

By utilizing this streamlined rollout toolkit, we not only save time but also ensure that the rollouts adhere to global directives. At this stage, the benefits of economies of scale begin to manifest themselves.

## Local requirements
Certain regions might necessitate unique legal configurations that need to be addressed individually during each rollout. This could involve customizations too, if necessary. At this time, seeking assistance from local experts becomes crucial. It's vital to ensure that during the testing phase, these new local requirements are thoroughly tested alongside the core model processes. This helps determine whether the core model's configuration could be affected by these changes.