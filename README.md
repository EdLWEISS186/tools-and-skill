# Hermes Tools, Skills & Integration Catalog

![Catalog](https://img.shields.io/badge/catalog-66%20entries-5E6F58) ![Categories](https://img.shields.io/badge/categories-14-5E6F58) ![Platform](https://img.shields.io/badge/platform-Hermes%20Agent-1B1A17) ![License](https://img.shields.io/badge/license-MIT-8A857C)

A curated catalog of **66 tools, skills, and integrations** for the [Hermes Agent](https://github.com/NousResearch/hermes-agent) — evaluated across 14 categories with a classification system and an integration-feasibility assessment for each entry.

> **Repository note:** This catalog originated from a personal evaluation of tools and skills for agent-based workflows. Each entry records its source repository, category, type, and whether it can be integrated into Hermes directly, through an intermediary (API/CLI/MCP/adapter), or only as a reference.

---

## Table of Contents

* Overview
* Classification Guide
* Agent Skills & Workflow
* AI Agent Platform
* AI Image Generation
* Browser & Desktop Automation
* Communication & Customer Support
* Context, Memory & Token Optimization
* Database & Backend Infrastructure
* Developer Tools & Engineering
* Document & Presentation
* Productivity & Project Management
* Research & Intelligence
* UI/UX & Visual Design
* Video, Audio & Voice
* Writing & Content Creation
* Combination Guide
* Avoid Matrix
* Credits & Support

## Overview

The agent ecosystem is large, and not every tool or skill fits every runtime. This repository answers a single question for each entry: **can it be integrated into Hermes Agent, and how much work does that integration require?**

Entries are grouped into 14 categories — from agent workflow systems and browser automation to memory optimization, UI/UX design, and content creation. Integration status is expressed in three grades:

| Status | Meaning |
| ------ | ------- |
| **Yes** | Relatively ready to install or adapt as a Hermes skill/plugin. |
| **Conditional** | Requires an intermediary — an API, CLI, MCP server, or adapter. |
| **Not directly** | Reference or catalog material only; not a ready-to-use integration. |

A machine-readable version of the full catalog is available at [`data/catalog.csv`](data/catalog.csv).

## Classification Guide

| Type | Meaning |
| ---- | ------- |
| **Plugins** | Agent skills, MCP servers, and extensions. |
| **App** | Standalone applications. |
| **Code** | Libraries, frameworks, and CLIs. |

## Agent Skills & Workflow

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **bmad-method** | [bmad-code-org/BMAD-METHOD](https://github.com/bmad-code-org/BMAD-METHOD) | Plugins | Yes — workflows and agent personas can be adapted; verify command compatibility with Hermes. | An AI-assisted software development methodology with clearly defined stages and roles, covering requirements analysis, planning, design, implementation, and testing. It provides a structured approach to managing the software development lifecycle. |
| **gsd** | [open-gsd/gsd-pi](https://github.com/open-gsd/gsd-pi) | Plugins | Yes — provided as agent workflows and instructions; the format and commands must be adapted for Hermes. | A workflow system that enables coding agents to handle large projects in structured stages. It helps organize specifications, plans, context, and implementation phases so the agent can maintain direction throughout the project. |
| **gstack** | [garrytan/gstack](https://github.com/garrytan/gstack) | Plugins | Yes — based on agent skills and commands; installation must be adapted for Hermes. | A set of commands and workflows that divides coding-agent responsibilities across roles such as product planning, design, engineering, code review, quality assurance, and release management. |
| **karpathy-guidelines** | [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) | Plugins | Yes — provided as instructions and skills that can be adapted for Hermes. | Behavioral guidelines for AI coding agents, based on Andrej Karpathy's observations of common mistakes made when using LLMs for coding. They encourage agents to work carefully, avoid rushing, and understand the context before modifying code. |
| **prompt-master** | [nidhinjs/prompt-master](https://github.com/nidhinjs/prompt-master) | Plugins | Yes — the skill and prompts can be adapted for Hermes. | A skill that helps create prompts tailored to the AI tool being used. It guides agents in maintaining context and producing more specific instructions. |
| **replica** | [Jakeschincariol/replica-skill](https://github.com/Jakeschincariol/replica-skill) | Plugins | Yes — the skills can be adapted for Hermes; review the dependencies and instructions for each skill. | A collection of skills for examining how an application works, recreating a similar version, testing the result, and addressing identified shortcomings. |
| **superpowers** | [obra/superpowers](https://github.com/obra/superpowers) | Plugins | Yes — the skills can be installed as agent capabilities; verify the Hermes installation format. | A collection of software development skills and workflows for AI coding agents. It helps agents understand requirements, create plans, write tests first, fix bugs, conduct reviews, and complete tasks through a structured process. |

## AI Agent Platform

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **multica-ai** | [multica-ai/multica](https://github.com/multica-ai/multica) | App | Conditional — an API connection or another integration mechanism with Hermes is required. | A platform for collaboration between people and AI agents within a shared workflow. It is designed to enable tasks to be assigned, completed, and monitored by both people and agents. |
| **open-hands** | [OpenHands/OpenHands](https://github.com/OpenHands/OpenHands) | App | Conditional — this is a standalone agent platform; integration with Hermes requires an API or adapter. | A software development agent platform that can assist with coding tasks, use the terminal, modify files, and interact with development environments. |
| **paperclip** | [paperclipai/paperclip](https://github.com/paperclipai/paperclip) | App | Conditional — this is a standalone application; an API or MCP connection is required for Hermes to control it. | An application for coordinating multiple AI agents within a virtual organization or team. It helps manage agent tasks, objectives, costs, and activities. |

## AI Image Generation

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **comfy-ui** | [Comfy-Org/ComfyUI](https://github.com/Comfy-Org/ComfyUI) | App | Conditional — it can be controlled through its API or workflows; a connection to Hermes is required. | A node-based visual application for building generative AI workflows, primarily for image generation and processing. Users can connect models and processing steps without creating the entire pipeline from scratch. |

## Browser & Desktop Automation

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **agent-browser** | [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) | Code | Conditional — it can be invoked through the Hermes terminal or tools after installation. | A browser automation CLI for AI agents. It enables agents to open pages, navigate websites, interact with page elements, and retrieve information from the browser. |
| **agent-desktop** | [vercel-labs/agent-desktop](https://github.com/vercel-labs/agent-desktop) | Code | Conditional — this CLI tool must be installed and configured as a Hermes tool. | A CLI that enables AI agents to control a computer through its desktop interface, including viewing the screen, clicking, typing, and interacting with UI elements. |
| **playwright-mcp** | [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) | Plugins | Yes — it can be connected as an MCP server if Hermes has MCP support enabled. | An MCP server that enables AI agents to control a browser using Playwright. It supports tasks such as opening pages, clicking elements, filling out forms, and testing web applications. |

## Communication & Customer Support

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **chatwoot** | [chatwoot/chatwoot](https://github.com/chatwoot/chatwoot) | App | Conditional — it can be connected through an API, webhook, or MCP. | A customer service platform for managing live chat, email, and conversations from multiple channels in a unified inbox. It can be self-hosted as an alternative to commercial customer support services. |
| **i-have-adhd** | [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) | Plugins | Yes — provided as instructions and a skill that can be adapted for Hermes. | A skill that configures agents to deliver responses that are concise, well-structured, and easy to scan. It prioritizes important information so that key points are not buried in lengthy text. |

## Context, Memory & Token Optimization

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **caveman** | [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) | Plugins | Conditional — the skill can be adapted; using the proxy requires additional configuration. | A skill and proxy that condense agent communication into highly concise language to reduce token consumption. Its primary objective is to conserve context while retaining essential information. |
| **claude-mem** | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | Plugins | Yes — the README mentions Hermes support; follow the official integration and configuration instructions. | A cross-session memory system that records agent activity, summarizes it, and restores relevant context when a subsequent session begins. |
| **codegraph** | [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) | Plugins | Yes — the repository states that it supports Hermes Agent; follow the official installation instructions. | Creates a map of relationships between components in a codebase, helping AI agents understand project structure, identify file dependencies, and navigate code with better context. |
| **ecc** | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Plugins | Yes — skills and prompts can be adapted; integrations with specialized features must be evaluated. | An optimization package for coding agents that includes skills, working guidelines, memory, security, research, and verification mechanisms. Its purpose is to make coding-agent workflows more consistent and controlled. |
| **graphify** | [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) | Plugins | Yes — available as a skill for several coding agents; adapt the installation process for Hermes. | Transforms source code, documentation, database schemas, configuration files, and documents into a knowledge graph. Agents can explore relationships between components to better understand a project. |
| **headroom** | [headroomlabs-ai/headroom](https://github.com/headroomlabs-ai/headroom) | Code | Conditional — available as a library, proxy, or MCP; connect it according to the Hermes operating mode. | A tool that reduces the size of tool outputs, logs, files, and JSON data before they are sent to an AI model. It aims to lower token usage and costs while preserving most of the information required. |
| **rtk** | [rtk-ai/rtk](https://github.com/rtk-ai/rtk) | Code | Conditional — it can be used as a CLI by Hermes after installation and configuration. | A CLI proxy that summarizes developer command outputs, such as Git results, test reports, and logs, making them more concise for AI agents. It helps reduce token consumption when agents work in the terminal. |
| **understand-anything** | [Egonex-AI/Understand-Anything](https://github.com/Egonex-AI/Understand-Anything) | Plugins | Yes — the repository provides integrations for several coding agents; verify Hermes support or use the CLI or skill. | Analyzes a codebase and generates an explorable, searchable, and queryable visual map and knowledge graph. It helps users understand project structure and relationships between files. |

## Database & Backend Infrastructure

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **coolify** | [coollabsio/coolify](https://github.com/coollabsio/coolify) | App | Conditional — API or CLI access, or an MCP connection, is required; it is not a skill that can be installed directly. | A self-hosted platform for deploying and managing applications, websites, databases, and other services on your own server. It serves as an alternative to cloud-based deployment services. |
| **noco-db** | [nocodb/nocodb](https://github.com/nocodb/nocodb) | App | Conditional — integration is available through an API, MCP, or connector; it is not injected as a skill. | A no-code database application that converts databases into spreadsheet-like interfaces. It allows users to manage tables, relationships, forms, and data views with minimal coding. |
| **supabase** | [supabase/supabase](https://github.com/supabase/supabase) | App | Conditional — it can be accessed through an API, CLI, or MCP; connection configuration is required. | A PostgreSQL-based backend platform that provides databases, authentication, file storage, realtime capabilities, and other backend features for web and mobile applications. |

## Developer Tools & Engineering

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **agent-skills** | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | Plugins | Yes — the skills can be installed or adapted for Hermes. | A collection of engineering skills for AI coding agents, covering practices such as test-driven development, API design, code review, debugging, security, and frontend development. |
| **awesome-mcp-servers** | [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) | Plugins | Not directly — this is a reference catalog rather than a standalone plugin; select a compatible server and connect it separately. | A curated directory of MCP servers that connect AI agents to services, applications, databases, developer tools, and data sources. |
| **bruno** | [usebruno/bruno](https://github.com/usebruno/bruno) | App | Conditional — it is not a Hermes plugin; it can be connected through a CLI, API, or custom MCP integration. | A desktop application for creating, managing, and executing API requests. It is suitable for testing HTTP endpoints without relying on cloud-based services. |
| **github-mcp** | [github/github-mcp-server](https://github.com/github/github-mcp-server) | Plugins | Yes — it can be connected to Hermes as an MCP server. | GitHub's official MCP server, which provides AI agents with structured access to repositories, issues, pull requests, commits, and other GitHub features, subject to token permissions. |
| **ponytail** | [DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail) | Plugins | Conditional — the skill can be adapted; the proxy requires a separate technical integration. | A skill and proxy designed to simplify coding-agent workflows by prioritizing the smallest viable solution, avoiding unnecessary abstractions, and preventing premature code additions. |
| **skills** | [mattpocock/skills](https://github.com/mattpocock/skills) | Plugins | Yes — provided the skills follow a format supported by Hermes. | A collection of practical skills for engineering tasks, including feature development, debugging, testing, and coding practices. The content consists of guidance that AI coding agents can read and follow. |

## Document & Presentation

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **archify** | [tt-a1i/archify](https://github.com/tt-a1i/archify) | Plugins | Yes — available as an agent skill; adapt its installation method for Hermes. | A skill for converting ideas, plans, or codebases into interactive diagrams. It is useful for visually explaining system architecture and process flows. |
| **markitdown** | [microsoft/markitdown](https://github.com/microsoft/markitdown) | Code | Conditional — Hermes can invoke it as a CLI or Python tool after installation. | A Python tool from Microsoft that converts various file formats, including Office documents and PDFs, into Markdown for easier reading and processing by AI systems. |
| **pdf-me** | [pdfme/pdfme](https://github.com/pdfme/pdfme) | Code | Conditional — the library must be accessed through code or a tool developed for Hermes. | A library for generating PDFs from templates. It provides a visual template editor and data-population features for producing PDF documents through web applications or Node.js. |
| **ppt-master** | [hugohe3/ppt-master](https://github.com/hugohe3/ppt-master) | App | Conditional — it must be run as a tool or API; it is not a ready-to-install Hermes skill. | An AI-powered tool for generating PowerPoint presentations from documents or topics. Its output consists of editable PowerPoint elements, including shapes, charts, tables, transitions, and animations. |
| **presenton** | [presenton/presenton](https://github.com/presenton/presenton) | App | Conditional — it can be connected through an API; it is not a direct plugin. | An AI-powered presentation creation application that generates slides from topics or source materials and provides an API as well as self-hosting options. |
| **unstract** | [Zipstack/unstract](https://github.com/Zipstack/unstract) | App | Conditional — integration is available through an API; it is not a skill that can be installed directly. | A platform for extracting information from unstructured documents, such as PDFs and scanned files, and converting it into data that can be used in APIs or ETL pipelines. |

## Productivity & Project Management

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **appflowy** | [AppFlowy-IO/AppFlowy](https://github.com/AppFlowy-IO/AppFlowy) | App | Conditional — an API, MCP, or connector is required; it is not a skill that can be installed directly. | A collaborative workspace application for managing documents, wikis, projects, and team tasks. It is an open-source alternative to Notion that offers users greater control over their data. |
| **cal-com-cal-diy** | [calcom/cal.diy](https://github.com/calcom/cal.diy) | App | Conditional — integration is available through an API or MCP; access configuration is required. | A self-hostable meeting-scheduling application. Users can configure availability, event types, and booking pages so that others can select a suitable time. |
| **career-ops** | [career-ops-hq/career-ops](https://github.com/career-ops-hq/career-ops) | Plugins | Yes — available as a plugin or skill for certain agents; its format must be adapted for Hermes. | An AI-powered job search assistant. It helps find job openings, match roles to a CV, tailor resumes and cover letters, prepare for interviews, and track applications. |
| **open-project** | [opf/openproject](https://github.com/opf/openproject) | App | Conditional — it can be connected through an API; it is not a ready-to-install Hermes plugin. | A project management application for organizing team work, tasks, schedules, roadmaps, Gantt charts, time tracking, and collaboration. |

## Research & Intelligence

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **Agent-reach** | [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) | Plugins | Conditional — Hermes can invoke the CLI or skill after the required dependencies and source access have been configured. | An internet research tool for AI agents that searches and collects information from platforms such as X, Reddit, YouTube, GitHub, and other web sources through a unified interface. |
| **last30days** | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | Plugins | Yes — the skill can be adapted; connectors and data sources must be configured. | A research skill that finds recent discussions on a topic across Reddit, X, YouTube, Hacker News, the web, and other sources, then summarizes the findings with time-based context. |
| **open-notebook** | [lfnovo/open-notebook](https://github.com/lfnovo/open-notebook) | App | Conditional — integration is possible through an available or custom-built API or MCP connection. | An open-source application for organizing research materials and generating summaries or document-based conversations, similar to NotebookLM. It can be self-hosted and supports multiple models. |
| **rea** | [morluto/rea](https://github.com/morluto/rea) | Code | Conditional — it is provided as a toolkit and CLI; it must be installed as a tool and connected to Hermes. | A toolkit for investigating how applications work with the assistance of agents, from observing application behavior to examining the underlying components and binaries. |
| **Scrapling** | [D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling) | Code | Conditional — it is available as a library or CLI; Hermes can use it through Python or terminal tools. | A Python framework for web scraping, ranging from extracting individual pages to crawling large numbers of pages. It is designed to handle websites with dynamic structures and challenging data extraction requirements. |
| **syetem-prompt-n-tools-models** | [x1xhlol/system-prompts-and-models-of-ai-tools](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools) | Code | Not directly — this is a reference repository, not a ready-to-use integration or plugin. | An archive of system prompts, examples of internal tools, and model information from various AI products. It is useful for studying instruction patterns and the capabilities of different AI tools. |
| **vane** | [ItzCrazyKns/Vane](https://github.com/ItzCrazyKns/Vane) | App | Conditional — this is an application or service; an API or MCP connection is required for Hermes to use it. | An AI-powered search and question-answering engine. It combines web search with answer summaries to provide users with responses supported by sources. |

## UI/UX & Visual Design

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **diagram-design** | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | Plugins | Yes — the skill can be adapted for Hermes. | A skill for creating diagrams with a polished editorial visual style. It provides various diagram types and generates HTML/SVG-based visuals to explain ideas or systems. |
| **hallmark** | [Nutlope/hallmark](https://github.com/Nutlope/hallmark) | Plugins | Yes — the skill can be adapted for Hermes. | A UI design skill that helps AI produce more intentional product interfaces and avoid generic, template-like AI-generated designs. It can be used when designing or improving user interfaces. |
| **impeccable** | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | Plugins | Yes — the skill can be adapted for Hermes; verify support for its commands and hooks. | A collection of design commands for critiquing, auditing, refining, and improving user interfaces. It helps identify UI patterns that appear generic or poorly executed. |
| **taste** | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | Plugins | Yes — the skill can be adapted for Hermes; browser-based checks require a browser tool. | A collection of skills that helps coding agents produce more distinctive frontend designs. It guides agents in using visual references, establishing a design direction, and reviewing results in a browser. |
| **ui-ux-pro-max** | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | Plugins | Yes — the skill can be installed or adapted for Hermes. | A UI/UX design skill that provides recommendations on visual styles, colors, typography, components, and user experience practices. It helps agents build more consistent interfaces. |

## Video, Audio & Voice

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **auto-clip** | [zhouxiaoka/autoclip](https://github.com/zhouxiaoka/autoclip) | App | Conditional — this is a standalone application; CLI/API access or desktop automation is required. | An AI-powered desktop application that converts long-form videos, such as podcasts, interviews, and classes, into multiple short clips. It can also help generate subtitles, cover images, and publication copy. |
| **hyperframes** | [heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) | Code | Conditional — this framework and CLI can be used by Hermes through coding and terminal tools. | A framework for creating videos using HTML, CSS, and JavaScript. Agents can build web-based scenes and animations, then render them as video files. |
| **open-montage** | [OpenMontageInc/OpenMontage](https://github.com/OpenMontageInc/OpenMontage) | Plugins | Yes — many skills can be adapted; specific pipelines and tools may require additional dependencies. | An agent-assisted video production system that provides pipelines, tools, and a collection of skills to support the video production process from initial work through final output. |
| **openwhispr** | [OpenWhispr/openwhispr](https://github.com/OpenWhispr/openwhispr) | App | Conditional — this is a desktop application; integration requires an API, CLI, or desktop automation. | A voice dictation application that converts speech into text, with options for local or cloud-based processing. It emphasizes privacy and supports multiple platforms. |
| **remotion** | [remotion-dev/remotion](https://github.com/remotion-dev/remotion) | Code | Conditional — Hermes can use this library or framework through a coding project and terminal tools. | A React framework for programmatically creating videos. Video scenes are built using components and code, then rendered into video files. |
| **voicestudio** | [debpalash/VoiceStudio](https://github.com/debpalash/VoiceStudio) | App | Conditional — this is a standalone application; an API, CLI, or custom integration is required. | A locally deployable audio-processing application. It supports audio generation and design, voice cloning, transcription, dictation, video dubbing, and audiobook creation. |

## Writing & Content Creation

| Name | Repository | Type | Integration | About |
| ---- | ---------- | ---- | ----------- | ----- |
| **humanizer** | [blader/humanizer](https://github.com/blader/humanizer) | Plugins | Yes — the skill can be adapted for Hermes. | A skill for editing written content so that it does not sound like generic AI-generated text. It recommends changes to rigid language patterns while preserving the original meaning. |
| **marketing-skills** | [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | Plugins | Yes — the skill can be adapted for Hermes. | A collection of marketing skills for AI agents, covering copywriting, SEO, conversion optimization, analytics, growth strategy, and marketing research. |
| **no-ai-slop** | [petergyang/no-ai-slop](https://github.com/petergyang/no-ai-slop) | Plugins | Yes — the skill can be adapted for Hermes. | An editing skill that detects and reduces more than 20 language patterns commonly associated with AI-generated writing, without changing the core message. |
| **postiz** | [gitroomhq/postiz-app](https://github.com/gitroomhq/postiz-app) | App | Conditional — integration can be developed through an API; it is not a ready-to-install Hermes plugin. | An application for planning, creating, scheduling, and publishing content across multiple social media platforms from a single location. It supports AI-assisted content management workflows. |
| **stop-slop** | [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop) | Plugins | Yes — it consists of instructions and a skill that Hermes can use. | A guide and skill for removing clichéd, excessive, or unnatural characteristics of AI-generated writing, making the text more direct and readable. |

## Combination Guide

Recommended pairings — tools whose functions complement each other rather than overlap.

| Combination | Rationale |
| ----------- | --------- |
| **superpowers + agent-skills** | A structured workflow combined with a collection of engineering practices; select the relevant skills for each stage. |
| **github-mcp + superpowers** | Repository, issue, and pull request access combined with structured engineering and review workflows. |
| **gstack + ui-ux-pro-max** | gstack manages workflow and role assignments, while UI-UX Pro Max provides design guidance during the UI stage. |
| **playwright-mcp + ui-ux-pro-max** | Design guidance can be validated through browser interactions and visual checks. |
| **graphify + claude-mem** | A knowledge graph for codebase relationships combined with session memory for agent work context. |
| **gsd + claude-mem** | GSD divides projects into stages, while Claude-mem carries relevant context across sessions. |
| **last30days + open-notebook** | Recent research findings can be collected and developed into research notes or documents. |
| **markitdown + open-notebook** | Converting documents to Markdown makes it easier to add source materials to the research workspace. |
| **remotion + open-montage** | Remotion supports code-based video production, while Open Montage provides agent-assisted production pipelines. |
| **agent-browser + Scrapling** | Use the browser for website interactions and Scrapling for data extraction or crawling when needed. |

## Avoid Matrix

Pairings to avoid — overlapping functionality that produces duplicated effort or conflicts.

| Avoid combining | Reason |
| --------------- | ------ |
| **humanizer + stop-slop** | Their writing-style editing functions overlap substantially; use one as the primary editor. |
| **humanizer + no-ai-slop** | Both reduce AI-like writing patterns; running them sequentially may result in repetitive edits. |
| **stop-slop + no-ai-slop** | All three tools serve nearly identical purposes; select one to avoid excessive revisions. |
| **gstack + bmad-method** | Both provide role-based and staged workflows; do not enable both full orchestration systems simultaneously. |
| **gsd + bmad-method** | Both organize projects into stages; select one as the primary planning framework. |
| **superpowers + gsd** | Both can orchestrate agent workflows; use one as the primary workflow. |
| **agent-browser + playwright-mcp** | Both control the browser; choose one control mechanism to prevent session/profile conflicts. |
| **ppt-master + presenton** | Both create presentations; choose one based on the required output rather than using both for the same deck. |

## Credits & Support

Made by **JERUZZALEM** — [github.com/EdLWEISS186](https://github.com/EdLWEISS186)

If this catalog is useful, a coffee is appreciated:

`0x870ad63acc507cdfd878F170606d19ae78988AFE`

## License

[MIT](LICENSE)

