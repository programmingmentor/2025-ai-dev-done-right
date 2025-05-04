---
# You can also start simply with 'default'
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /dou-first-slide-bg.png
# some information about your slides (markdown enabled)
title: Cursor, Windsurf, Copilot, Cline — best practices for development with AI
info: |
  ## Presentation for DOU

# apply unocss classes to the current slide
# class: text-center  <-- Removing default text-center for more control
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# take snapshot for each slide in the overview
overviewSnapshots: true

# Configure fonts (https://sli.dev/custom/config-fonts.html)
fonts:
  sans: "IBM Plex Sans"
  # Optional: specify weights and italic if needed
  # weights: '400,500,700'
  # italic: false
---

<!-- DOU Logo Top Right -->
<div class="absolute top-4 right-5 z-10">
  <img src="/dou-day-logo-bw.png" alt="DOU Logo BW" style="height: 60px;" />
</div>

<div class="absolute top-1/3 left-[20%] text-white text-lg z-10" style="margin-top: -40px; background-color: black; padding: 10px;">
  Kyiv, 2025
</div>

<!-- Wrapper Div for Both Blocks -->
<div class="absolute top-1/3 left-[20%] w-3/5 z-10">
  <!-- Black Title Div -->
  <div class="p-6" style="background-color: black;">
    <h1 class="text-white font-black uppercase tracking-wide leading-none" style="font-size: 30px; line-height: 1;">
      Cursor, Windsurf, Copilot, Cline — best practices for development with AI
    </h1>
  </div>
  <!-- Pink Subtitle Div (moved back inside, width adjusted) -->
  <div class="p-4 w-2/3 ml-1/2" style="background-color: rgb(255, 22, 177);"> <!-- Adjusted width to w-2/3 -->
    <p class="text-white text-sm">
      Viacheslav Koldovskyy, SoftServe
    </p>
  </div>
</div>

---
layout: image-left
image: /prince-of-persia.webp
---

<div class="h-full flex items-center">
  <h1>Do you remember the moment when you wanted to become a developer?</h1>
</div>

---
layout: image-left-bg-color
image: /troll-face.png
bgColor: white
backgroundSize: contain
---

<div class="h-full flex items-center">
  <h1>And when you started writing code, do you remember your first impressions?</h1>
</div>

---

<div class="w-full h-full flex justify-center items-center">
  <img src="/meme-error-line-42.jpg" class="h-3/4 object-contain" />
</div>

---
layout: image
image: /meme-dot1-dot2.png
backgroundSize: 40%
---

---

<div class="w-full h-full flex justify-center items-center">
  <img src="/meme-different-error.jpg" class="h-3/4 object-contain" />
</div>

---

# Vibe Coding

<div class="w-full flex justify-center">
  <img src="/vibe-coding-tweet.png" class="w-1/2"/>
</div>

---

# Pieter Levels

<div class="w-full flex justify-center">
  <img src="/levelsio.png" class="w-1/2"/>
</div>

---

<div class="w-full flex justify-center">
  <div class="ml-20"> 
    <Tweet scale="0.65" id="1901660771505021314" class="w-100"/>
  </div>
</div>

---

<div class="w-full flex justify-center">
  <img src="/personal-motivation-calendar.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://personalmotivationcalendar.com/">https://personalmotivationcalendar.com/</a>
</div>

---

# Fails - SaaS

<div class="w-full flex justify-center">
  <img src="/fail-saas.png" class="w-1/3"/>
</div>

---

# Fails - Fetch

<div class="w-full flex justify-center">
  <img src="/fail-fetch.png" class="w-1/3"/>
</div>

---

# Fails - rm -rf

<div class="w-full flex justify-center">
  <img src="/fail-clean-directory.png" class="w-4/5"/>
</div>

---

# Are there any tasks for which code generation with AI already works today?

- MVP
- Hobby projects
- "One-time" tasks
- Experiments and prototypes
- ...

---

<div class="w-full flex justify-center">
  <div class="ml-16"> 
    <Tweet scale="0.75" id="1739052802314539371" class="w-100"/>
  </div>
</div>

---
layout: image-left
image: /vibe-coding-tools.jpg
---

# Tools

- Cursor
- Windsurf
- Cline
- Github Copilot
- v0.dev
- bolt.new
- repl.it agent
- lovable
- ChatGPT
- Grok
- ...

---

# How it works: everything is controlled by LLM

<div class="w-full flex justify-center">
  <img src="/how-works-prompt-llm-code.png" class="w-4/5"/>
</div>

---

# LLM

<div class="w-full flex justify-center">
  <img src="/chatbot-arena-language.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://lmarena.ai/">https://lmarena.ai/</a>
</div>

---

# WebDev Arena

<div class="w-full flex justify-center">
  <img src="/web-dev-arena.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://web.lmarena.ai/">https://web.lmarena.ai/</a>
</div>

---

# SWE Bench Verified

<div class="w-full flex justify-center">
  <img src="/swe-bench.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://www.swebench.com/#verified">https://www.swebench.com/#verified</a>
</div>

---

# What does a prompt consist of?

<div class="w-full flex justify-center mt-20">
  <img src="/how-works-prompt-expanded-llm-code.png" class="w-4/5"/>
</div>

---

# Simple agent

<div class="w-full flex justify-center">
  <img src="/how-works-simple-agent.png" class="w-4/5"/>
</div>

---

# Agent with tools

<div class="w-full flex justify-center">
  <img src="/how-works-modern-agent.png" class="w-4/5"/>
</div>

---

# Main problems

- Non-deterministic LLM: butterfly effect
- Context window limitations
- Hallucinations
- Security and legal issues
- Current knowledge
- ...

---
layout: image-left
image: /butterfly-effect.png
---

# Non-deterministic LLM - butterfly effect

Using LLM for a classical engineer is like fighting chaos

- **Repeatability not guaranteed**
- **Unstable dependencies**
- **Scattered edits across the project**
- **Mass rewriting of existing code**
- **Divergence (drift) of agents in multi-step chains**

---

# Context window limitations

<div class="w-full flex justify-center">
  <img src="/context-window.png" class="w-4/5"/>
</div>

---

# LOC in LLM tokens

## React:

- **React jsx (100 lines):** 700 tokens
- **React jsx (200 lines):** 1,500 tokens

## SQL:

- **SQL script (100 lines):** 1,150 tokens
- **SQL script (200 lines):** 2,500 tokens

## Python:

- **Python source code file (100 lines):** 1,000 tokens
- **Python source code file (200 lines):** 1,700 tokens

Source: https://prompt.16x.engineer/blog/chatgpt-context-window-token-limit

---

# Price

<div class="w-full flex justify-center">
  <img src="/openai-pricing.png" class="w-120"/>
</div>

<div class="w-full flex justify-center mt-5">
  <a href="https://openai.com/api/pricing/">https://openai.com/api/pricing/</a>
</div>

---

# Security and legal issues with AI code generation

- Generation of unsafe (vulnerable) code
- Execution of arbitrary commands in the system
- Use of integrations with external services without proper control
- Installation of unwanted dependencies (attack vector)
- Leakage of confidential information and intellectual property
- Generation of code that violates intellectual property rights

---

# Tools: general purpose

- ChatGPT
- Gemini (gemini.google, aistudio.google.com)
- Grok
- Claude
- DeepSeek
- ...

---

# ChatGPT

<div class="w-full flex justify-center">
  <img src="/chatgpt-canvas.png" class="w-4/5"/>
</div>

---

# Grok

<div class="w-full flex justify-center">
  <img src="/grok.png" class="w-140"/>
</div>

---

# Gemini

<div class="w-full flex justify-center">
  <img src="/gemini.png" class="w-4/5"/>
</div>

---

# Gemini AI Studio

<div class="w-full flex justify-center">
  <img src="/gemini-ai-studio.png" class="w-4/5"/>
</div>

---

# Two Steps Back Pattern

<div class="w-full flex justify-center">
  <img src="/two-steps-back.png" class="w-4/5"/>
</div>

---

# Repository Prompt Tools - Repomix

<div class="w-full flex justify-center">
  <img src="/repomix.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://repomix.com/">https://repomix.com/</a>
</div>

---

# 16x Prompt

<div class="w-full flex justify-center">
  <img src="/16x-prompt.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://prompt.16x.engineer/">https://prompt.16x.engineer/</a>
</div>

---

# bolt.new

<div class="w-full flex justify-center">
  <img src="/bolt-new.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://bolt.new/">https://bolt.new/</a>
</div>

---

# v0.dev

<div class="w-full flex justify-center">
  <img src="/v0-dev.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://v0.dev/">https://v0.dev/</a>
</div>

---

# repl.it agent

<div class="w-full flex justify-center">
  <img src="/replit.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://repl.it/">https://repl.it/</a>
</div>

---

# Github Copilot

<div class="w-full flex justify-center">
  <img src="/github-copilot.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://copilot.github.com/">https://copilot.github.com/</a>
</div>

---

# Cursor

<div class="w-full flex justify-center">
  <img src="/cursor.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://www.cursor.com/">https://www.cursor.com/</a>
</div>

---

# Windsurf

<div class="w-full flex justify-center">
  <img src="/windsurf.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://codeium.com/windsurf">https://codeium.com/windsurf</a>
</div>

---

# Cline

<div class="w-full flex justify-center">
  <img src="/cline.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://cline.bot/">https://cline.bot/</a>
</div>

---

# MCP - Model Context Protocol

<div class="w-full flex justify-center">
  <img src="/mcp.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://modelcontextprotocol.io/">https://modelcontextprotocol.io/</a>
</div>

---

# Memory bank

---

# MCP.so

<div class="w-full flex justify-center">
  <img src="/mcp-list.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://mcp.so/">https://mcp.so/</a>
</div>

---

<div class="w-full h-full flex justify-center items-center">
  <h1 class="text-center">Tips, Tricks and Resources</h1>
</div>

---

# Cursor Rules

<div class="w-full flex justify-center">
  <img src="/cursor-rules.png" class="w-2/3"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://docs.cursor.com/context/rules-for-ai">https://docs.cursor.com/context/rules-for-ai</a>
</div>

---

# Cursor.directory

<div class="w-full flex justify-center">
  <img src="/cursor-directory.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://cursor.directory/">https://cursor.directory/</a>
</div>

---

# llms.txt

<div class="w-full flex justify-center">
  <img src="/llms-txt.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://llmstxt.org/">https://llmstxt.org/</a>
</div>

---

# Drizzle ORM llms.txt

<Tweet scale="0.65" id="1896981123559002158" class="w-3/4"/>

https://orm.drizzle.team/llms.txt

---

# Plan Mode

<div class="w-full flex justify-center">
  <img src="/cursor-plan-mode.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://forum.cursor.com/t/plan-vs-act-mode-xml-prompt/50996">https://forum.cursor.com/t/plan-vs-act-mode-xml-prompt/50996</a>
</div>

---

# Docs

<div class="w-full flex justify-center">
  <img src="/cursor-docs.png" class="w-3/4"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://docs.cursor.com/context/@-symbols/@-docs">https://docs.cursor.com/context/@-symbols/@-docs</a>
</div>

---

# TDD

# Prompt:

## create ...

## write tests first, then the code, then update code until tests pass

---

# Local History Plugin

<div class="w-full flex justify-center">
  <img src="/local-history.png" class="w-1/2"/>
</div>

---

# Issues

- Breaking code changes
- Hallucinations and incorrect solutions
- Deadlocks
- Limited knowledge of new libraries/frameworks
- Issues with large codebases
- Issues with security
- Speed of development
- Cost of usage
- ...

---
layout: image-left
image: /vyacheslav-koldovskyy.png
---

# Viacheslav Koldovskyy

- Ph.D, Associate Professor
- 20+ years in IT
- SoftServe Academy Competence Manager
- Certified Google Cloud Professional Architect
- Practical AI Enthusiast
- YouTuber: [youtube.com/@programmingmentorua](https://www.youtube.com/@programmingmentorua)
- Blogger: [t.me/programmingmentor](https://t.me/programmingmentor)
- LinkedIn: [koldovsky](https://www.linkedin.com/in/koldovsky/)

---
## layout: end
---

# Thank you!

<div class="flex justify-center w-full h-30 items-center">
  <img src="/slides-qr.png" class="w-25 h-25"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://programmingmentor.github.io/slidev-vibe-coding/">https://programmingmentor.github.io/slidev-vibe-coding/</a>
</div>
