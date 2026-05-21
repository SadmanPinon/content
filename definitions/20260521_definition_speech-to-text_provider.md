---
title: 'Speech-to-Text Provider'
description: 'A service adapter that converts audio input into text through a speech recognition API or model.'
date: 2026-05-21
author: 'SadmanPinon'
---

# Speech-to-Text Provider

## Definition

A speech-to-text provider is a service, model, or API adapter that receives audio
input and returns a transcript. In an application, the provider usually hides
provider-specific authentication, request fields, file upload rules, response
formats, and error handling behind one common interface.

## Context and Usage

Developer tools often support more than one speech-to-text provider so teams can
choose based on language coverage, cost, latency, compliance, and output format.
For example, a transcription CLI might expose `--api openai`, `--api groq`, or
`--api sarvam`, while each provider implementation handles its own API key,
endpoint, model name, and transcript parsing.
