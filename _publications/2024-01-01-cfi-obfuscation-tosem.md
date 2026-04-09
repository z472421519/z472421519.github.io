---
title: "Posing New Challenges to Function Entry Identification Through Fine-Grained CFI Obfuscation"
collection: publications
category: manuscripts
permalink: /publication/2025-cfi-obfuscation-tosem
date: 2025-01-01
venue: 'ACM Transactions on Software Engineering and Methodology (TOSEM)'
excerpt: 'We propose fine-grained CFI obfuscation techniques that systematically challenge existing function entry identification methods in binary analysis tools.'
citation: '<b>Tiantai Zhang</b>*, Chengbin Pang*, Fei Peng, Linzhang Wang, Bing Mao. &quot;Posing New Challenges to Function Entry Identification Through Fine-Grained CFI Obfuscation.&quot; <i>ACM Transactions on Software Engineering and Methodology</i>, ACM, 2025. (* equal contribution)'
---

Function entry identification is a crucial yet challenging task for binary disassemblers. Recent research shows that call frame information (CFI) provides accurate and almost complete function entries, giving disassemblers significant improvements in function entry detection. CFI is specifically designed for efficient stack unwinding, and every function has corresponding CFI in x64 and aarch64 architectures.

We propose a prototype of OCFI to obfuscate CFI based on the observation that not every function and instruction unwinds the stack at runtime. The goal is to obstruct function detection of popular disassemblers that use CFI as a way to detect function entries.

**Authors:** **Tiantai Zhang**\*, Chengbin Pang\*, Fei Peng, Linzhang Wang, Bing Mao (* equal contribution)

**Publisher:** ACM
