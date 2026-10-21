---
title: "Anthropic AI rediscovers the forgotten origin of the ECDSA curves used in cryptography"
video_id: enZi-oL_LBI
date: 2026-10-21
url: https://www.youtube.com/watch?v=enZi-oL_LBI
channel: Dr. Samuel Allen Alexander
tags:
  - ai-tools
  - ai-strategy
  - industry-news
transcript: ../transcripts/2026-10-21-anthropic-ai-rediscovers-the-forgotten-origin-of-the-ecdsa-c.md
relevant: true
knowledge: true
highlight: true
---

# Anthropic AI rediscovers the forgotten origin of the ECDSA curves used in cryptography

## Executive Summary

Anthropic's Claude AI has solved a long-standing cryptographic mystery by reverse-engineering the origins of the NIST ECDSA curve seeds, revealing they were generated using a weak pseudo-random number generator (lrand48) seeded with Unix timestamps from 1997-1998, rather than any deliberate backdoor selection. This discovery significantly increases trust in the security of these widely used cryptographic curves, although some base points and one binary curve seed remain unexplained. The finding demonstrates the power of AI in mathematical discovery and cryptographic forensics.

## Key Points

- Anthropic's Claude AI reverse-engineered the NIST ECDSA curve seeds, discovering they were generated using the lrand48 pseudo-random number generator seeded with Unix timestamps from 1997-1998, not a hash of a humorous phrase as previously rumored. [00:05:36](https://www.youtube.com/watch?v=enZi-oL_LBI&t=336)
- The discovery significantly reduces the likelihood of deliberate backdoors in the curves, as the timestamps are clustered within a year, limiting the search space for any malicious selection. [00:07:03](https://www.youtube.com/watch?v=enZi-oL_LBI&t=423)
- Claude also identified the origins of some base points, using a different random number generator (Liarjen Lenstra's long integer arithmetic package), but the base points for P224, P256, P384, and P521 remain unexplained, leaving some open questions. [00:16:14](https://www.youtube.com/watch?v=enZi-oL_LBI&t=974)
