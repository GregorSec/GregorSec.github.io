---
title: Captured Signal
description: Official Writeup for Misc/Crypto Captured Signal
author: gregorsec
date: 2025-10-22 18:11:00 +0800
categories: [Writeups, Authored]
tags: [Misc,Crypto,CTF Challenge]
pin: true
math: true
mermaid: true
---

## Challenge Description

> One of our satellites intercept a signal coming from Kepler-22b, it could be nothing but we want you to verify that it is nothing.
> 
> 48 74 80 55 57 48 74 71 49 56 43 62 71 84 42 48 74 71 49 56 48 72 96 41 40 48 74 71 52 56 48 74 70 86 40 48 74 80 58 57 48 101 107 67 42 48 101 107 67 58 48 74 71 49 56 43 62 71 81 40 48 101 98 58 57 48 72 96 41 40 48 101 107 64 58 48 101 106 101 42 48 101 107 64 57 48 74 80 55 40 48 101 98 58 56 48 101 98 61 57 43 62 71 81 41 48 74 71 49 56 48 100 38 50 42 48 101 107 64 57 48 74 70 86 40 48 74 71 52 57 48 101 98 61 41 48 101 98 58 57 48 101 98 58 57 43 62 71 81 41 48 101 107 64 57 48 100 38 50 42 48 101 98 58 56 48 101 97 95 41 48 74 71 49 56 48 74 71 49 39 48 101 98 61 58 48 74 80 58 58 43 62 62 78 40 48 74 71 49 56 48 100 38 50 42 48 101 98 58 56 48 74 79 92 41 48 74 71 52 56 48 74 80 55 40 48 101 98 61 58 48 74 80 58 58 43 62 71 84 42 48 74 71 49 55 48 100 38 50 41 48 74 80 55 56 48 101 106 101 42 48 74 80 58 57 48 101 98 61 41 48 74 80 58 58 48 101 98 61 58 43 62 71 84 42 48 74 71 49 56 48 72 96 41 40 48 74 71 49 56 48 74 70 86 40 48 74 80 58 58 48 74 71 49 39 48 74 71 52 56 48 74 71 49 55 43 62 71 84 41 48 74 80 58 57 48 72 96 41 40 48 101 98 58 56 48 101 106 101 41 48 74 80 55 56 48 74 71 49 39 48 101 107 67 59 48 74 71 49 55 43 62 71 81 40 48 101 107 67 58 48 100 38 50 41 48 74 80 58 57 48 74 79 92 41 48 74 80 58 58 48 74 71 52 40 48 74 71 52 57 48 74 71 49 55 43 62 62 78 40 48 101 107 67 59 48 100 38 50 42 48 101 98 58 56 48 101 97 95 41 48 74 71 52 56 48 101 98 61 41 48 101 98 58 56 48 101 107 67 58 43 62 71 84 42 48 74 71 49 56 48 100 38 50 41 48 74 71 49 55 48 101 106 101 42 48 74 80 55 57 48 74 80 55 40 48 101 107 67 58 48 74 71 52 56 43 62 71 81 40 48 74 80 58 58 48 72 96 41 40 48 74 80 55 56 48 101 106 101 41 48 74 80 58 57 48 74 71 52 40 48 101 107 67 58 48 74 71 52 57 43 62 71 81 40 48 74 71 49 56 48 100 38 50 41 48 101 98 61 57 48 101 97 95 41 48 101 107 64 57 48 74 80 55 40 48 101 98 58 57 48 74 80 55 57 43 62 71 81 40 48 74 80 58 58 48 72 96 41 41 48 101 98 58 56 48 101 97 95 41 48 74 71 49 55 48 101 98 58 40 48 101 98 61 58 48 101 98 58 56 43 62 62 75 40 48 74 71 49 55 48 72 96 41 41 48 74 71 52 57 48 74 70 86 40 48 74 80 55 56 48 74 80 58 41 48 74 71 52 56 48 74 71 49 55 43 62 62 78 41 48 101 107 67 58 48 72 96 38 40 48 101 107 67 59 48 74 70 86 39 48 101 98 61 58 48 101 107 67 42 48 74 71 52 57 48 74 80 55 56 43 62 71 84 42 48 74 71 49 56 48 100 38 50 41 48 74 71 49 55 48 101 106 101 42 48 74 80 55 57 48 74 80 55 40 48 101 107 67 58 48 74 71 52 56 43 62 71 81 40 48 74 71 52 57 48 72 96 41 40 48 101 107 67 58 48 74 70 86 39 48 101 98 61 58 48 101 107 67 42 48 101 107 64 57 48 101 98 61 57 43 62 71 81 40 48 101 98 61 58 48 72 96 38 39 48 101 107 64 57 48 101 106 101 41 48 101 107 67 59 48 101 98 58 40 48 74 80 58 58 48 101 107 64 57 43 62 62 75 40 48 101 98 58 56 48 72 96 41 41 48 101 98 58 56 48 101 106 101 42 48 74 71 49 55 48 74 80 58 41 48 101 98 61 57 48 101 98 61 57 43 62 71 84 42 48 74 71 49 56 48 72 96 41 40 48 74 71 49 56 48 101 97 95 41 48 74 80 58 58 48 74 71 49 39 48 74 80 58 58 48 101 107 64 58

> Flag: GregorSec{}
{: .prompt-note }

### Steps to Decoding

For this challenge we take the “captured” signal and put it into [Cyberchef](https://cyberchef.org/). Doing this actually will solve the first two steps automatically, and will also give you a glimpse into the final ciphertext.

#### Step 1

We decode the captured signal from decimal. This will give us the following ciphertext:

> 0JP790JG18+>GT\*0JG180H\`)(0JG480JFV(0JP:90ekC\*0ekC:0JG18+>GQ(0eb:90H\`)(0ek@:0eje\*0ek@90JP7(0eb:80eb=9+>GQ)0JG180d&2\*0ek@90JFV(0JG490eb=)0eb:90eb:9+>GQ)0ek@90d&2\*0eb:80ea\_)0JG180JG1'0eb=:0JP::+>>N(0JG180d&2\*0eb:80JO\\)0JG480JP7(0eb=:0JP::+>GT\*0JG170d&2)0JP780eje\*0JP:90eb=)0JP::0eb=:+>GT\*0JG180H\`)(0JG180JFV(0JP::0JG1'0JG480JG17+>GT)0JP:90H\`)(0eb:80eje)0JP780JG1'0ekC;0JG17+>GQ(0ekC:0d&2)0JP:90JO\\)0JP::0JG4(0JG490JG17+>>N(0ekC;0d&2\*0eb:80ea\_)0JG480eb=)0eb:80ekC:+>GT\*0JG180d&2)0JG170eje\*0JP790JP7(0ekC:0JG48+>GQ(0JP::0H\`)(0JP780eje)0JP:90JG4(0ekC:0JG49+>GQ(0JG180d&2)0eb=90ea\_)0ek@90JP7(0eb:90JP79+>GQ(0JP::0H\`))0eb:80ea\_)0JG170eb:(0eb=:0eb:8+>>K(0JG170H\`))0JG490JFV(0JP780JP:)0JG480JG17+>>N)0ekC:0H\`&(0ekC;0JFV'0eb=:0ekC\*0JG490JP78+>GT\*0JG180d&2)0JG170eje\*0JP790JP7(0ekC:0JG48+>GQ(0JG490H\`)(0ekC:0JFV'0eb=:0ekC\*0ek@90eb=9+>GQ(0eb=:0H\`&'0ek@90eje)0ekC;0eb:(0JP::0ek@9+>>K(0eb:80H\`))0eb:80eje\*0JG170JP:)0eb=90eb=9+>GT\*0JG180H\`)(0JG180ea\_)0JP::0JG1'0JP::0ek@:
{: .prompt-note }

#### Step 2

From here we can see the message is Base85 encoded. When we decode the Base85, we get the following ciphertext:

> 01010001 11100010 10001000 10110111 11100001 10010010 10110111 11100010 10001010 10100011 11110000 10011101 10011001 10111001 11100010 10001000 10110111 01000011 11100001 10010010 10110111 11100001 10010011 10110101 01111011 11100010 10000100 10111000 00100000 11001100 10100011 00100000 11110000 10011101 10011001 10111001 00110000 01011111 11100010 10010101 10001110 11100011 10000011 10101010 11100010 10001110 10010011 00110001 11100011 10000011 10101010 11100010 10010101 10001110 11100010 10000100 10111000 00100000 11001100 10100011 00100000 01111100 01111100 01011111 00110100 11100011 10000011 10101010 11100010 10000110 10111000 01011111 11001010 10010110 00110011 01111100 01111100 00110000 11100011 10000011 10101010 11100010 10000110 10111000 01111101
{: .prompt-note }

#### Step 3

Clearly we can determine this to be binary. When we decode this we get:

> Q∷ᒷ⊣𝙹∷cᒷᓵ{ℸ ̣ 𝙹0\_╎リ⎓1リ╎ℸ ̣ ||\_4リ↸\_ʖ3||0リ↸}
{: .prompt-note }

> Please Note: if the message looks messed up or like this: Gâ·á·â£ð¹â·sá·áµ{â¸ Ì£ ð¹0\_âãªâ1ãªââ¸ Ì£ ||\_4ãªâ¸\_Ê3||0ãªâ¸}  
>   
> You need to change the output character encoding in Cyberchef from Raw Bytes to UTF-8 as seen below
{: .prompt-tip }
---
image:
  path: MiscCrypto Challenge Captured Signal/5_MiscCrypto Challenge Captu.png
  alt: Raw Bytes Output
---
---
image:
  path: MiscCrypto Challenge Captured Signal/7_MiscCrypto Challenge Captu.png
  alt: UTF-8 Output
---

#### Step 4

We can now determine that we have a Standard Galactic Alphabet translated message. From here we can take 2 different approaches to getting the flag. The intended approach is to realize the message begins with Q instead of G and perform a ROT16 cipher. Doing so you will receive the following message:

> G∷ᒷ⊣𝙹∷sᒷᓵ{ℸ ̣ 𝙹0\_╎リ⎓1リ╎ℸ ̣ ||\_4リ↸\_ʖ3||0リ↸}
{: .prompt-note }

Or you can take the unintended path which is to translate the message now, using a website such as [dcode's Standard Galactic Alphabet page](https://www.dcode.fr/standard-galactic-alphabet) or [texttoolz's Standard Galactic Alphabet Translator](https://texttoolz.com/tools/standard-galactic-alphabet-Translator). Doing this you will get something along the lines of the following:

> Qregorcec{t o0\_inf1nit y\_4nd\_b3y0nd} ← texttoolz's translation
> 
> QREGORcEC{TO0\_INF1NITY\_4ND\_B3Y0ND} ← Dcode's translation
{: .prompt-tip }

#### Step 5

Finally for the final step, dependent on the approach you took you will either translate it from SGA using any SGA Translator or you simply correct the flag prefix by swapping the Q and C for a G and S.

#### Flagging

And here you have the final flag:

> Flag: GregorSec{to0\_inf1nity\_4nd\_b3y0nd}
{: .prompt-note }

> Using the texttoolz's translator is the most successful way of getting the flag. There was an issue with the copying of the translated message into other online tools for translation and encoding/decoding that was not caught until after the event completed. This issue end up changing the message from:  
>   
> G∷ᒷ⊣𝙹∷Sᒷᓵ{ℸ ̣𝙹0\_╎リ⎓1リ╎ℸ ̣||\_4リ↸\_ʖ3||0リ↸}   
>   
> to this:  
>   
> G∷ᒷ⊣𝙹∷sᒷᓵ{ℸ ̣ 𝙹0\_╎リ⎓1リ╎ℸ ̣ ||\_4リ↸\_ʖ3||0リ↸}  
>   
> This would cause a few issues such as S in GregorSec to be lowercase and spaces to appear within the translated flag.
{: .prompt-warning }

### Images Showing the Solution
---
image:
  path: MiscCrypto Challenge Captured Signal/MiscCrypto Challenge Captu.JPG
  alt: Full Cyberchief portion
---
---
image:
  path: MiscCrypto Challenge Captured Signal/1_MiscCrypto Challenge Captu.JPG
  alt: Texttoolz SGA to English Translation
---






