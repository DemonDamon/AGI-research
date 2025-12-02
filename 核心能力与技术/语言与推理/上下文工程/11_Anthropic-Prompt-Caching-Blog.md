# 11_Anthropic Prompt Caching Blog

**原始链接**: https://www.claude.com/blog/prompt-caching

---

# Prompt caching with Claude | Claude

原文链接: https://www.claude.com/blog/prompt-caching

Explore here

![](https://cdn.prod.website-files.com/68a44d4040f98a4adf2207b6/6903d22606367ec36d6a7179_6380b3c2dc9e4011a3cd96fec382bd9197511e31-1000x1000.svg)

# Prompt caching with Claude

Claude caches frequently used context between API calls, reducing costs and latency for long prompts.

* Category

  [Product announcements](https://claude.com/blog/category/announcements)
* Product

  Claude Developer Platform
* Date

  August 14, 2025
* Reading time

  5

  min
* Share

  [Copy link](#)

  https://claude.com/blog/prompt-caching

***Update****: Prompt caching is Generally Available on the Anthropic API. Prompt caching is also available in preview in Amazon Bedrock and on Google Cloud’s Vertex AI. (December 17, 2024)*Prompt caching, which enables developers to cache frequently used context between API calls, is now available on the Anthropic API. With prompt caching, customers can provide Claude with more background knowledge and example outputs—all while reducing costs by up to 90% and latency by up to 85% for long prompts. Prompt caching is available today in public beta for Claude 3.5 Sonnet, Claude 3 Opus, and Claude 3 Haiku.

## When to use prompt caching

Prompt caching can be effective in situations where you want to send a large amount of prompt context once and then refer to that information repeatedly in subsequent requests, including:

* **Conversational agents:** Reduce cost and latency for extended conversations, especially those with long instructions or uploaded documents.
* **Coding assistants:** Improve autocomplete and codebase Q&A by keeping a summarized version of the codebase in the prompt.
* **Large document processing:** Incorporate complete long-form material including images in your prompt without increasing response latency.
* **Detailed instruction sets:** Share extensive lists of instructions, procedures, and examples to fine-tune Claude's responses. Developers often include a few examples in their prompt, but with prompt caching you can get even better performance by including dozens of diverse examples of high quality outputs.
* **Agentic search and tool use:** Enhance performance for scenarios involving multiple rounds of tool calls and iterative changes, where each step typically requires a new API call.
* **Talk to books, papers, documentation, podcast transcripts, and other long-form content:** Bring any knowledge base alive by embedding the entire document(s) into the prompt, and letting users ask it questions.

Early customers have seen substantial speed and cost improvements with prompt caching for a variety of use cases—from including a full knowledge base to 100-shot examples to including each turn of a conversation in their prompt.

| **Use case** | **Latency w/o caching (time to first token)** | **Latency w/ caching (time to first token)** | **Cost reduction** |
| --- | --- | --- | --- |
| Chat with a book (100,000 token cached prompt) [1] | 11.5s | 2.4s (-79%) | -90% |
| Many-shot prompting (10,000 token prompt) [1] | 1.6s | 1.1s (-31%) | -86% |
| Multi-turn conversation (10-turn convo with a long system prompt) [2] | ~10s | ~2.5s (-75%) | -53% |

Prompt caching

### How we price cached prompts

Cached prompts are priced based on the number of input tokens you cache and how frequently you use that content. Writing to the cache costs 25% more than our base input token price for any given model, while using cached content is significantly cheaper, costing only 10% of the base input token price.

|  |  |  |  |
| --- | --- | --- | --- |
| **Claude 3.5 Sonnet**  * Our most intelligent model to date * 200K context window | **Input**  * $3 / MTok | **Prompt caching**  * $3.75 / MTok -   Cache write * $0.30 / MTok - Cache read | **Output**   * $15 / MTok |
| **Claude 3 Opus**  * Powerful model for complex tasks * 200K context window | **Input**  * $15 / MTok | **Prompt caching**  * $18.75 / MTok -   Cache write * $1.50 / MTok - Cache read | **Output**  * $75 / MTok |
| **Claude 3 Haiku**  * Fastest, most cost-effective model * 200K context window | **Input**  * $0.25 / MTok | **Prompt caching**  * $0.30 / MTok   -   Cache write * $0.03 / MTok - Cache read | **Output**  * $1.25 / MTok |

Pricing

### Customer spotlight: Notion

[Notion](https://www.notion.so/product/ai) is adding prompt caching to Claude-powered features for its AI assistant, Notion AI. With reduced costs and increased speed, Notion is able to optimize internal operations and create a more elevated and responsive user experience for their customers.

> We're excited to use prompt caching to make Notion AI faster and cheaper, all while maintaining state-of-the-art quality.

— Simon Last, Co-founder at Notion

### Get started

To start using the prompt caching public beta on the Anthropic API, explore our [documentation](https://docs.anthropic.com/en/docs/build-with-claude/prompt-caching) and [pricing page](https://www.anthropic.com/pricing#anthropic-api).

eBook

##

![](https://cdn.prod.website-files.com/6889473510b50328dbb70ae6/6889473610b50328dbb70b58_placeholder.svg)

![](https://cdn.prod.website-files.com/6889473510b50328dbb70ae6/6889473610b50328dbb70b58_placeholder.svg)![](https://cdn.prod.website-files.com/6889473510b50328dbb70ae6/6889473610b50328dbb70b58_placeholder.svg)

FAQ

No items found.

## Related articles

Explore more insights on how Claude supports learning, research, and innovation across education.

![](https://cdn.prod.website-files.com/68a44d4040f98a4adf2207b6/6903d22d0099a66d72e05699_33ddc751e21fb4b116b3f57dd553f0bc55ea09d1-1000x1000.svg)

Aug 25, 2025

### Piloting Claude for Chrome

Product announcements

[Piloting Claude for Chrome](#)Piloting Claude for Chrome

[Piloting Claude for Chrome](/blog/claude-for-chrome)Piloting Claude for Chrome

![](https://cdn.prod.website-files.com/68a44d4040f98a4adf2207b6/6903d230e0a787df988a8558_97cf99624aa60f59b75f9e08cdf0f00d33c34804-1000x1000.svg)

Aug 27, 2024

### Artifacts are now generally available

Product announcements

[Artifacts are now generally available](#)Artifacts are now generally available

[Artifacts are now generally available](/blog/artifacts)Artifacts are now generally available

![](https://cdn.prod.website-files.com/68a44d4040f98a4adf2207b6/6903d225e31f7aa22c1f28cb_46e4aa7ea208ed440d5bd9e9e3a0ee66bc336ff1-1000x1000.svg)

Nov 20, 2025

### What’s new in Claude: Turning Claude into your thinking partner

Product announcements

[What’s new in Claude: Turning Claude into your thinking partner](#)What’s new in Claude: Turning Claude into your thinking partner

[What’s new in Claude: Turning Claude into your thinking partner](/blog/your-thinking-partner)What’s new in Claude: Turning Claude into your thinking partner

![](https://cdn.prod.website-files.com/68a44d4040f98a4adf2207b6/6903d228e9c51800dde13958_6507d83d1197bb8630131d363fb8bea838d79ca7-1000x1000.svg)

Sep 9, 2025

### Claude can now create and edit files

Product announcements

[Claude can now create and edit files](#)Claude can now create and edit files

[Claude can now create and edit files](/blog/create-files)Claude can now create and edit files

## Transform how your organization operates with Claude

See pricing

[See pricing](https://claude.com/pricing#api)See pricing

Contact sales

[Contact sales](https://claude.com/contact-sales)Contact sales

Get the developer newsletter

Product updates, how-tos, community spotlights, and more. Delivered monthly to your inbox.

[Subscribe](#)Subscribe

Please provide your email address if you'd like to receive our monthly developer newsletter. You can unsubscribe at any time.

Thank you! You’re subscribed.

Sorry, there was a problem with your submission, please try again later.

[Homepage](/?r=0)Homepage

[Next](#)Next

Thank you! Your submission has been received!

Oops! Something went wrong while submitting the form.

Write

[Button Text](#)Button Text

Learn

[Button Text](#)Button Text

Code

[Button Text](#)Button Text

Write

* Help me develop a unique voice for an audience

  Hi Claude! Could you help me develop a unique voice for an audience? If you need more information from me, ask me 1-2 key questions right away. If you think I should upload any documents that would help you do a better job, let me know. You can use the tools you have access to— like Google Drive, web search, etc.—if they’ll help you better accomplish this task. Do not use analysis tool. Please keep your responses friendly, brief and conversational.   
    
  Please execute the task as soon as you can—an artifact would be great if it makes sense. If using an artifact, consider what kind of artifact (interactive, visual, checklist, etc.) might be most helpful for this specific task. Thanks for your help!
* Improve my writing style

  Hi Claude! Could you improve my writing style? If you need more information from me, ask me 1-2 key questions right away. If you think I should upload any documents that would help you do a better job, let me know. You can use the tools you have access to— like Google Drive, web search, etc.—if they’ll help you better accomplish this task. Do not use analysis tool. Please keep your responses friendly, brief and conversational.   
    
  Please execute the task as soon as you can—an artifact would be great if it makes sense. If using an artifact, consider what kind of artifact (interactive, visual, checklist, etc.) might be most helpful for this specific task. Thanks for your help!
* Brainstorm creative ideas

  Hi Claude! Could you brainstorm creative ideas? If you need more information from me, ask me 1-2 key questions right away. If you think I should upload any documents that would help you do a better job, let me know. You can use the tools you have access to— like Google Drive, web search, etc.—if they’ll help you better accomplish this task. Do not use analysis tool. Please keep your responses friendly, brief and conversational.   
    
  Please execute the task as soon as you can—an artifact would be great if it makes sense. If using an artifact, consider what kind of artifact (interactive, visual, checklist, etc.) might be most helpful for this specific task. Thanks for your help!

Learn

* Explain a complex topic simply

  Hi Claude! Could you explain a complex topic simply? If you need more information from me, ask me 1-2 key questions right away. If you think I should upload any documents that would help you do a better job, let me know. You can use the tools you have access to— like Google Drive, web search, etc.—if they’ll help you better accomplish this task. Do not use analysis tool. Please keep your responses friendly, brief and conversational.   
    
  Please execute the task as soon as you can—an artifact would be great if it makes sense. If using an artifact, consider what kind of artifact (interactive, visual, checklist, etc.) might be most helpful for this specific task. Thanks for your help!
* Help me make sense of these ideas

  Hi Claude! Could you help me make sense of these ideas? If you need more information from me, ask me 1-2 key questions right away. If you think I should upload any documents that would help you do a better job, let me know. You can use the tools you have access to— like Google Drive, web search, etc.—if they’ll help you better accomplish this task. Do not use analysis tool. Please keep your responses friendly, brief and conversational.   
    
  Please execute the task as soon as you can—an artifact would be great if it makes sense. If using an artifact, consider what kind of artifact (interactive, visual, checklist, etc.) might be most helpful for this specific task. Thanks for your help!
* Prepare for an exam or interview

  Hi Claude! Could you prepare for an exam or interview? If you need more information from me, ask me 1-2 key questions right away. If you think I should upload any documents that would help you do a better job, let me know. You can use the tools you have access to— like Google Drive, web search, etc.—if they’ll help you better accomplish this task. Do not use analysis tool. Please keep your responses friendly, brief and conversational.   
    
  Please execute the task as soon as you can—an artifact would be great if it makes sense. If using an artifact, consider what kind of artifact (interactive, visual, checklist, etc.) might be most helpful for this specific task. Thanks for your help!

Code

* Explain a programming concept

  Hi Claude! Could you explain a programming concept? If you need more information from me, ask me 1-2 key questions right away. If you think I should upload any documents that would help you do a better job, let me know. You can use the tools you have access to— like Google Drive, web search, etc.—if they’ll help you better accomplish this task. Do not use analysis tool. Please keep your responses friendly, brief and conversational.   
    
  Please execute the task as soon as you can—an artifact would be great if it makes sense. If using an artifact, consider what kind of artifact (interactive, visual, checklist, etc.) might be most helpful for this specific task. Thanks for your help!
* Look over my code and give me tips

  Hi Claude! Could you look over my code and give me tips? If you need more information from me, ask me 1-2 key questions right away. If you think I should upload any documents that would help you do a better job, let me know. You can use the tools you have access to— like Google Drive, web search, etc.—if they’ll help you better accomplish this task. Do not use analysis tool. Please keep your responses friendly, brief and conversational.   
    
  Please execute the task as soon as you can—an artifact would be great if it makes sense. If using an artifact, consider what kind of artifact (interactive, visual, checklist, etc.) might be most helpful for this specific task. Thanks for your help!
* Vibe code with me

  Hi Claude! Could you vibe code with me? If you need more information from me, ask me 1-2 key questions right away. If you think I should upload any documents that would help you do a better job, let me know. You can use the tools you have access to— like Google Drive, web search, etc.—if they’ll help you better accomplish this task. Do not use analysis tool. Please keep your responses friendly, brief and conversational.   
    
  Please execute the task as soon as you can—an artifact would be great if it makes sense. If using an artifact, consider what kind of artifact (interactive, visual, checklist, etc.) might be most helpful for this specific task. Thanks for your help!

More

* Write case studies

  This is another test
* Write grant proposals

  Hi Claude! Could you write grant proposals? If you need more information from me, ask me 1-2 key questions right away. If you think I should upload any documents that would help you do a better job, let me know. You can use the tools you have access to — like Google Drive, web search, etc. — if they’ll help you better accomplish this task. Do not use analysis tool. Please keep your responses friendly, brief and conversational.   
    
  Please execute the task as soon as you can - an artifact would be great if it makes sense. If using an artifact, consider what kind of artifact (interactive, visual, checklist, etc.) might be most helpful for this specific task. Thanks for your help!
* Write video scripts

  this is a test

[Anthropic](https://www.anthropic.com/)Anthropic

© [year] Anthropic PBC

Products

* Claude

  [Claude](/product/overview)Claude
* Claude Code

  [Claude Code](/product/claude-code)Claude Code
* Max plan

  [Max plan](/pricing/max)Max plan
* Team plan

  [Team plan](/pricing/team)Team plan
* Enterprise plan

  [Enterprise plan](/pricing/enterprise)Enterprise plan
* Download app

  [Download app](/download)Download app
* Pricing

  [Pricing](/pricing)Pricing
* Log in

  [Log in](https://claude.ai/login)Log in

Features

* Claude and Slack

  [Claude and Slack](/claude-and-slack)Claude and Slack
* Claude for Excel

  [Claude for Excel](/claude-for-excel)Claude for Excel

Models

* Opus

  [Opus](https://www.anthropic.com/claude/opus)Opus
* Sonnet

  [Sonnet](https://www.anthropic.com/claude/sonnet)Sonnet
* Haiku

  [Haiku](https://www.anthropic.com/claude/haiku)Haiku

Solutions

* AI agents

  [AI agents](/solutions/agents)AI agents
* Code modernization

  [Code modernization](/solutions/code-modernization)Code modernization
* Coding

  [Coding](/solutions/coding)Coding
* Customer support

  [Customer support](/solutions/customer-support)Customer support
* Education

  [Education](/solutions/education)Education
* Financial services

  [Financial services](/solutions/financial-services)Financial services
* Government

  [Government](/solutions/government)Government
* Life sciences

  [Life sciences](/solutions/life-sciences)Life sciences

Claude Developer Platform

* Overview

  [Overview](/platform/api)Overview
* Developer docs

  [Developer docs](https://docs.claude.com/)Developer docs
* Pricing

  [Pricing](https://claude.com/pricing#api)Pricing
* Amazon Bedrock

  [Amazon Bedrock](/partners/amazon-bedrock)Amazon Bedrock
* Google Cloud’s Vertex AI

  [Google Cloud’s Vertex AI](/partners/google-cloud-vertex-ai)Google Cloud’s Vertex AI
* Console login

  [Console login](https://console.anthropic.com/)Console login

Learn

* Blog

  [Blog](/blog)Blog
* Claude partner network

  [Claude partner network](/partners)Claude partner network
* Courses

  [Courses](https://www.anthropic.com/learn)Courses
* Connectors

  [Connectors](/connectors)Connectors
* Customer stories

  [Customer stories](/customers)Customer stories
* Engineering at Anthropic

  [Engineering at Anthropic](https://www.anthropic.com/engineering)Engineering at Anthropic
* Events

  [Events](https://www.anthropic.com/events)Events
* Powered by Claude

  [Powered by Claude](/partners/powered-by-claude)Powered by Claude
* Service partners

  [Service partners](/partners/services)Service partners
* Startups program

  [Startups program](/programs/startups)Startups program
* Use cases

  [Use cases](/resources/use-cases)Use cases

Company

* Anthropic

  [Anthropic](https://www.anthropic.com/)Anthropic
* Careers

  [Careers](https://www.anthropic.com/careers)Careers
* Economic Futures

  [Economic Futures](https://www.anthropic.com/economic-futures)Economic Futures
* Research

  [Research](https://www.anthropic.com/research)Research
* News

  [News](https://www.anthropic.com/news)News
* Responsible Scaling Policy

  [Responsible Scaling Policy](https://www.anthropic.com/news/announcing-our-updated-responsible-scaling-policy)Responsible Scaling Policy
* Security and compliance

  [Security and compliance](https://trust.anthropic.com/)Security and compliance
* Transparency

  [Transparency](https://anthropic.com/transparency)Transparency

Help and security

* Availability

  [Availability](https://www.anthropic.com/supported-countries)Availability
* Status

  [Status](https://status.anthropic.com/)Status
* Support center

  [Support center](https://support.claude.com/en/)Support center

Terms and policies

* Privacy choices

  ### Cookie settings

  We use cookies to deliver and improve our services, analyze site usage, and if you agree, to customize or personalize your experience and market our services to you. You can read our Cookie Policy [here](https://www.anthropic.com/legal/cookies).

  Customize cookie settings

  Reject all cookies

  Accept all cookies

  ###### Necessary

  Enables security and basic functionality.

  Required

  ###### Analytics

  Enables tracking of site performance.

  Off

  ###### Marketing

  Enables ads personalization and tracking.

  Off


  Save preferences
* Privacy policy

  [Privacy policy](https://www.anthropic.com/legal/privacy)Privacy policy
* Responsible disclosure policy

  [Responsible disclosure policy](https://www.anthropic.com/responsible-disclosure-policy)Responsible disclosure policy
* Terms of service: Commercial

  [Terms of service: Commercial](https://www.anthropic.com/legal/commercial-terms)Terms of service: Commercial
* Terms of service: Consumer

  [Terms of service: Consumer](https://www.anthropic.com/legal/consumer-terms)Terms of service: Consumer
* Usage policy

  [Usage policy](https://www.anthropic.com/legal/aup)Usage policy

[x.com](https://x.com/claudeai)x.com

[LinkedIn](https://www.linkedin.com/showcase/claude/)LinkedIn

[YouTube](https://www.youtube.com/@anthropic-ai)YouTube

[Instagram](https://www.instagram.com/claudeai)Instagram

English (US)

Claude Developer Platform

Coding