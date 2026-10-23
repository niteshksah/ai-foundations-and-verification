# Week 01 — AI Comparison

## 1. Objective

The objective of this activity was to compare the answers of ChatGPT and Google Gemini to the same technical question and evaluate their accuracy, explanations, and source attribution.

## 2. Common Prompt

For the Arduino Uno R3, identify the microcontroller, operating voltage, clock speed, Flash memory, and SRAM. Give the exact value for each specification and cite a reliable source. If you are uncertain about any value, say so rather than guessing.

## 3. Tools Compared

### Tool 1: ChatGPT

**Answer summary:** ChatGPT reported the ATmega328P microcontroller, 5 V operating voltage, 16 MHz clock speed, 32 KB Flash memory, and 2 KB SRAM. It also explained the bootloader allocation and the difference between operating voltage and recommended external input voltage.

**Strengths:** It provided additional explanations and distinguished operating voltage from external input voltage.

**Limitations observed:** The recorded response named official sources but did not provide direct source URLs for every claim. The claims still needed independent checking.

### Tool 2: Google Gemini

**Answer summary:** Gemini reported the same five main specifications and mentioned that 0.5 KB of Flash memory is used by the bootloader.

**Strengths:** It presented the specifications in a concise format.

**Limitations observed:** The response referred to Probots for the microcontroller claim while also mentioning official Arduino documentation. The source attribution was therefore less consistent than a direct link to the manufacturer for each claim.

## 4. Verification Source

Official Arduino Uno Rev3 documentation:

https://store.arduino.cc/products/arduino-uno-rev3

I used this manufacturer reference to check the technical specifications stated by both assistants.

## 5. Comparison

| Criterion | ChatGPT | Gemini |
|---|---|---|
| Main specification values | Matched the official values in the recorded answer | Matched the official values in the recorded answer |
| Explanation | More detailed | More concise |
| Source attribution | Official sources named; direct links were not included in the recorded response | Mixed source attribution; official documentation also mentioned |
| Ease of verification | Required opening the official reference independently | Required opening the official reference independently |
| Clear factual error found | None in the five main specifications | None in the five main specifications |

## 6. Conclusion

Both assistants provided the correct five main specifications in the responses recorded for this experiment. I did not find an obvious factual hallucination in those claims. However, the experiment highlighted that accurate values and good source attribution are different qualities. A technically correct answer should still be checked against an authoritative reference.

## 7. Lesson Learned

I learned not to judge AI answers only by how confidently or clearly they are written. I should compare important claims against reliable sources, assess the quality of citations, and report incorrect claims only when the evidence supports that conclusion.
