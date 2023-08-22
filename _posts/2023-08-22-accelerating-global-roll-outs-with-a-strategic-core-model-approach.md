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
Using Dynamics 365 Finance and SCM, we can tap into their standard features to create a toolkit for deploying the core model. To kick things off, we employ the Business Process Modeler (BPM), which I discussed in my recent post "The Power of Leveraging a Quality BPM Library" – check it out for more details. In a nutshell, we document all the standard core processes in BPM, including task records for user training and test case generation.

When it's time for the next implementation, we just refer back to this core model BPM library. We link it to the specific implementation and legal entity. This makes everything streamlined – from business processes to training materials creation and necessary testing.