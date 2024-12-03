---
layout: post
title: Scalable Collaboration of Multiple AI Agents in Workspaces
categories: blog
permalink: blog/slack-agents
---

Ever wondered how to make AI agents actually useful in your daily work? While there's been lots of buzz around AI automation, most solutions still struggle with a fundamental problem: they don't fit naturally into how we actually work. That's where SlackAgents comes in.

<figure>
  <img class="single" src="/images/blog/slackagents.png" alt="SlackAgents.">
  <figcaption>A glimpse into how SlackAgents works</figcaption>
</figure>

We present **SlackAgents**, a *multi-agent* library for scalable management and collaboration of AI agents on Slack. As an agentic layer developed upon the Slack platform, the framework offers instant AI integration into organizational workflows, enabling continuous improvement through daily use. It also leverages Slack’s extensive features to enable AI-powered automation of real daily tasks. Furthermore, **SlackAgents** facilitates scalable collaboration, allowing for effective communication and task orchestration. Our solution bridges existing gaps in AI agent management, offering a robust platform for developing, deploying and managing AI agents for workplace environments.

## What Makes SlackAgents Different?

Here is a comparison of features supported by SlackAgents library vs existing libraries in terms of  **Multiple Agents**: multi-agent orchestration; **Workspace Automation**: native Slack workspace feature support and automation; **Scalable Collaboration**: support for vast number of agents for collaborative task solving; **Admin Management**: interfaces for human supervisors to monitor and intervene; **Market Distribution**: instant deployment and distribution to workspaces via the Slack Marketplace.

| Library | Multiple Agents | Workspace Automation | Scalable Collaboration | Admin Management | Market Distribution |
|---------|----------------|---------------------|---------------------|-----------------|-------------------|
| LangChain | ❌ | ❌ | ❌ | ✅ | ❌ |
| LlamaIndex | ❌ | ❌ | ❌ | ✅ | ❌ |
| AutoGen | ✅ | ❌ | ❌ | ✅ | ❌ |
| CrewAI | ✅ | ❌ | ❌ | ✅ | ❌ |
| CAMEL | ✅ | ✅ | ✅ | ❌ | ❌ |
| OpenAI Swarm | ✅ | ❌ | ❌ | ❌ | ❌ |
| SlackAgents | ✅ | ✅ | ✅ | ✅ | ✅ |

Our solution is a multi-agent library as an **agentic layer** leveraging the Slack infrastructure, the most widely used messaging and collaboration platform for corporate workspaces. The marriage of multi-agent framework with Slack can immediately bring the following benefits: 

- **Scalable Collaboration**: multi-agent communication and task orchestration are handled by various types of conversation sessions across threads and channels of the Slack messaging system. 
- **Slack-Powered Automation**: interfaces AI agents to various Slack features and visual components, such as [canvas](https://slack.com/features/canvas), [bookmarks](https://slack.com/help/articles/205239997-Pin-messages-and-bookmark-links), [workflows](https://slack.com/features/workflow-automation), [notifications](https://slack.com/help/articles/201355156-Configure-your-Slack-notifications), etc., incentivizing developers to build AI agents that can control Slack for automating real daily work and tasks;
- **Workspace Integration**: enables developers to use every AI agent in the existing workflows, ensuring immediate deployment and continuous improvement through daily interactions. The agent can be easily distributed to the public and other Slack workspaces;
<!--more-->

<div style="position: relative; padding-bottom: 38.48631239935588%; height: 0;"><iframe src="https://www.loom.com/embed/21f5c21bc22b47eb940221871959e7cd?sid=22ab7b92-bf03-41fd-92e3-e7994851b5cd" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>

## Framework Architecture

**SlackAgents** has two core agent types: 

- **Assistant Agent**: AI agent that can use various tools (custom functions, public APIs, external libraries, code interpreters) in multi-turn conversation. 
- **Workflow Agent**: AI agent with complex multi-stage workflows and manages state and transitions towards sequential goals in multi-turn conversation. 

<figure>
  <img class="single" src="/images/blog/code_interpreter.png" alt="Code Interpreter Assistant Agent." style="width:75%;">
  <figcaption>Code Interpreter Assistant Agent.</figcaption>
</figure>
Each AI agent, whether an Assistant or Workflow type, operates as a standalone Slack App. To facilitate both user-agent interactions and inter-agent communication, each agent is equipped with specific message listeners, and conversation tools for requesting and providing assistance to one another. This enables multiple agents to collaborate in Slack threads across channels.

### Multi-agent Collaboration

The core of the multi-agent collaboration in **SlackAgents** is for the current agent to *(1) produce* a message that contains a request for assistance with @ mention of the chosen agents or human from a pre-defined colleague list, *(2) send* the message to the colleague(s) in a dedicated session, and *(3) listen* for colleagues' responses in the session. Compared with the **handoff** strategy in **OpenAI swarm**, which hands off all messages to another agent by swapping system prompt and tools, our collaboration strategy is decentralized, asynchronous, and scalable by leveraging Slack-specific functionalities, and importantly, same as how human workers collaborate in Slack channels by looping in colleagues for help in threads.

<figure>
  <img class="single" src="/images/blog/protocol.png" alt="Multi-agent collaboration protocol.">
  <figcaption>Multi-agent collaboration protocol.</figcaption>
</figure>

### User Interface

#### Command Line Interface (CLI)

The SlackAgents Command-Line Interface (CLI) provides a comprehensive set of commands for managing AI agents within Slack workspaces. This specification details the command structure, available operations, and implementation guidelines.

<figure>
  <img class="single" src="/images/blog/cli.png" alt="SlackAgents CLI.">
  <figcaption>SlackAgents CLI.</figcaption>
</figure>

#### AI Management Dashboard

The admin dashboard serves as a central hub for managing AI agents, tools, and workflows. It provides real-time visibility into agent performance, task execution, and system status. Key features include user management, tool configuration, and detailed analytics on agent interactions. Admins can monitor agent activity, adjust tool settings, and troubleshoot issues directly from the dashboard. 

<figure>
  <img class="single" src="/images/blog/dashboard.png" alt="SlackAgents Dashboard.">
  <figcaption>SlackAgents Dashboard.</figcaption>
</figure>

#### Github Repository

The Github repository is the central hub for the development of **SlackAgents**. It contains the source code for the **SlackAgents** library, as well as the documentation and examples.

<figure>
  <img class="single" src="/images/blog/slackagents_repo.png" alt="SlackAgents Github Repository.">
  <figcaption>SlackAgents Github Repository.</figcaption>
</figure>
