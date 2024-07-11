---
title: "Watch out for confirmation bias"
categories:
  - In-context learning
tags:
  - Chatbots
author: David Mimno
---

This afternoon I was at a presentation by the Cornell Digital Humanities Summer Fellows. Afterwards, I was talking analysis of poetic forms, and pulled out my laptop to try something out.

There are good reasons to think that this task would be extremely difficult. Language models are amazing in many ways, but two things that they struggle with are *counting* and *meta-knowledge about words*. They see many words in sequence, but internally they represent them as whole words or sub words that have been mapped to integers. They never *hear* language, so concepts like rhyme, syllables, or starting letters are so difficult even though to us they seem natural. 

So I wanted to ask the newest most powerful model about a line of poetry that it has never seen. Since I happened to have my foot on a chair, I came up with this not-quite grammatical example. I passed it to [Claude](https://claude.ai).

> What is the poetic meter of the following line? 
> the chair on which I set my foot upon

The response was surprisingly good! It correctly identifies this as iambic pentameter, marks the stress pattern with CAPS, provides a scansion, and defines some key terms.

> To analyze the poetic meter of this line, let's break it down into syllables and stress patterns:
> 
> the CHAIR on WHICH I SET my FOOT u-PON
> 
> This line has 10 syllables with alternating unstressed and stressed syllables. The pattern is:
> 
> unstressed - stressed - unstressed - stressed - unstressed - stressed - unstressed - stressed - unstressed - stressed
> 
> This metrical pattern is known as iambic pentameter. Here's why:
> 
> 1. Iambic: An iamb is a metrical foot consisting of an unstressed syllable followed by a stressed syllable.
> 2. Pentameter: There are five ("penta") iambs in the line.
> 
> Iambic pentameter is one of the most common metrical patterns in English poetry, often used in sonnets, blank verse, and other poetic forms.
> 
> Would you like me to explain any aspect of this analysis further?

But although we should be rightly impressed when a model does something amazing, we also need to push it to the point where it breaks. Back at my office, which is currently next to a construction site, I then tried a line with four anapests, a much less common meter. Claude still guesses iambic pentameter! The capitalization for stressed syllables is correct, but the scansion is the same as the previous example, and the syllable count is off by two.

> Certainly, let's analyze this new line:
> 
> the con-STRUC-tion of BUILD-ings is WASHED by the RAIN
> 
> Breaking it down, we have:
> 
> unstressed - stressed - unstressed - stressed - unstressed - stressed - unstressed - stressed - unstressed - stressed
> 
> This line has 10 syllables with a clear alternating pattern of unstressed and stressed syllables. This metrical pattern is known as iambic pentameter. Here's why:
> 
> 1. Iambic: Each foot is an iamb (unstressed syllable followed by a stressed syllable).
> 2. Pentameter: There are five ("penta") iambs in the line.
> 
> The line consists of five iambs:
> 1. the con-
> 2. STRUC-tion
> 3. of BUILD-
> 4. ings is
> 5. WASHED by
> 6. the RAIN
> 
> This is a perfect example of iambic pentameter, one of the most common and influential meters in English poetry. It's often used in sonnets, blank verse, and many other poetic forms.

