---

layout: col-sidebar
title: OWASP Dragon-GPT
tags: dragon-gpt
level: 2
type: tool
pitch: An automatic OpenAI-powered threat modeling analysis based on OWASP Threat Dragon diagram
---

<img src="assets/images/icon.png" width="20%" height="20%" alt="Dragon-GPT Icon" align="left" hspace="15" vspace="45" style="margin-bottom: 30px; position: relative">

[![](https://img.shields.io/badge/owasp-incubator-blue)](https://owasp.org/other_projects/)
[![GitHub contributors](https://img.shields.io/github/contributors/LuizBoina/dragon-gpt)](https://github.com/LuizBoina/dragon-gpt/graphs/contributors)
[![GitHub Pulse](https://img.shields.io/github/commit-activity/m/LuizBoina/dragon-gpt)](https://github.com/badges/shields/pulse)
[![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/LuizBoina/dragon-gpt/.github%2Fworkflows%2Fdjango-test.yml)](https://github.com/LuizBoina/dragon-gpt/actions)

## Description

Dragon-GPT is an AI-powered tool that automatically performs the threat modeling analysis on the diagram made using the OWASP Threat Dragon modeling software. It uses the OpenAI API, so you need to have a valid account for their tokens to use on each program call, and the JSON file generated when you save/export an OWASP Threat Dragon project (generally saved in td.vue folder).

The program itself is pretty simple, it extracts every relevant information on the JSON file, like the diagram model and components used on the modeling, and transforms it into a human-readable sentence. After that, the sentence is send via OpenAI API, and the result of the analysis is printed. By default, it uses chatgpt-3.5-turbo but you can change that via parameter to another model like the chatgpt-4.

## Changelog

 - [Update on 27/10/23] Add Support to Local LLM, the Llama 2, so you don't need an OpenAI account. The results using Llama may be inferior and slower than ChatGPT but at least it's free.