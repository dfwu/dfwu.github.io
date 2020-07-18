---
author: dfwu
comments: true
date: 2020-02-08 23:11:24+00:00
layout: post
link: https://dfwu.wordpress.com/2020/02/08/orthography/
slug: orthography
title: The point of a written language is not to record speech
wordpress_id: 157
categories:
- Orthography
- Prosody
---

What’s the point of written language (aka orthography)? Assuming it is a human invention, why was it created? A simple assumption is that it records spoken language, so that information can be transmitted in more permanent and replicable ways. A reader who sees the written text can reconstruct the speech in the physical absence of the speaker. This makes sense conceptually because we know that in a spoken language, information is generally transmitted through speech. Then any written form that captures the uttered sounds in speech can transmit the information. This idea also has its empirical support: all written languages in the world postdate their spoken counterparts, and are “glottographic” - they all record uttered sounds with symbols.





In this post I argue based on case studies of the English and Chinese writing systems that this idea is in fact wrong. <!-- more -->Both writing systems leave out critical aspects of speech (I call this _“under-documentation” of speech_, where some meaningful differences in speech are lost in writing), while at the same time over-specifying other aspects of speech (_“over-documentation” of speech_, where the same sound may correspond to different symbols). I have a speculation (based on a small number of observations) as to which aspects of speech tend to be under-documented, and which aspects tend to be over-documented. Sentence-level sound information (e.g. intonation and pitch) tends to be under-documented, whereas word-level sound information tends to be over-documented. Furthermore, I argue that over-documentation is a result of an important property of orthography: it should avoid ambiguities in the mapping between form and meaning. 





First, I will talk about how English orthography (or any existing writing system that I know of) under-documents certain sentence-level information. Before doing so, here’s what I mean by “sentence-level” and “word-level”. They are the two levels on which humans convey information through uttered sounds: (sentence-level) prosody, and (word-level) phonology. On the word level, different words are pronounced differently, e.g. _apple_ sounds different from _dog_. In addition, given an identical string of words, prosody (intonation, prominence, and breaks) plays an important role in distinguishing their meanings. Consider (1):





(1) The Vikings won over their enemies.





This sentence can mean two things: “The Vikings defeated their enemies” or “The Vikings persuaded their enemies.” Prosody is the only factor that distinguishes them: there is a greater break between _over_ and _their _in the former meaning than in the latter, and _over_ is more prominent in the former meaning than in the latter. Clearly English orthography does not transcribe prosody, hence creating ambiguity with texts like (1). 





While sentence-level features such as prosody are under-documented, word-level features are often over-documented. In many writing systems, words with identical pronunciation but different meanings (homophones) may have different spellings, such as _there_ and _their_ in English.1 





If the sole purpose of orthography is to record uttered sounds, then orthography should not bother to distinguish words with identical sounds because they are not distinguished in speech anyway. But this move makes sense if orthography is designed to avoid ambiguities, to ensure that a reader is not confused when reading a string of words. While ambiguities may arise in speech due to accidental homophony, they are avoided in writing whenever possible.2





When homophony arises, the obvious solution is to create different spellings for the homophones, as we saw in English. However, spoken English has a relatively small number of homophones. What happens in a language with a large number of homophones? Designing the orthography for such a language will be a complex problem, as there are opposing factors to consider. On the one hand, orthography should avoid ambiguities, such that homophones should appear differently in writing. But since there are so many homophones, this will generate a large number of symbols to distinguish them, making them difficult to learn and memorize. Therefore, an efficient writing system should avoid ambiguities, while keeping its symbols easy to learn. 





Mandarin Chinese is an ideal case of study due to its large number of homophones. Chinese orthography (Simplified Chinese and Traditional Chinese) may appear to be unnecessarily complicated at first glance, but once we view it as a balancing act of opposing factors, it actually makes a lot of sense. 





Let’s begin by examining Simplified Chinese. Just like all the writing systems in the world, it encodes the segmental properties of a word - a word’s composition of consonant and vowels. For example, the sound _ma_ is a combination of the consonant m and the vowel a. The smallest unit of Chinese orthography is a character, which often consists of at least two parts (aka radicals), one of which encodes the segmental property. Take 妈 (mā) ‘mother’ as an example. It has two radicals, one on the left 女 and one on the right 马. The radical on the right 马 (mǎ) is identical to 妈 (mā) in its consonant-and-vowel combination, so this radical encodes the segmental properties of 妈 (mā). Let’s call 马 the _segmental radical_ of 妈.





To appreciate the existing Chinese orthography, let’s try designing an alternative system. Imagine we are commissioned by a skeptic of the current writing system to design an alternative. Where do we start? It makes sense for orthography to encode the segmental properties, so suppose we have decided that for the character for ‘mother’, we should at least have the radical 马. What other features should the character include? 





An obvious answer is the tone. Like segments, tone is a “lexical” property - it helps the listener determine which lexical item / word the speaker is using. The same combination of consonants and vowels can have different meanings depending on which tone it carries (_ma_ means ‘mother’ with one tone, and ‘hemp’ with another tone). Therefore, just having the segments _ma_ does not tell us exactly which word it is. There are 5 tones in total, so encoding the tones is easy. We just need to add a symbol that can make a 5-way distinction (e.g. with numeral “radicals”: 马1, 马2, 马3, 马4, 马5). 





If the sole function of orthography is to record speech, we should be done now — each character does encode the lexical, phonological property of a word, including information about its segments and tone. But as we just saw with English, orthography should avoid ambiguities created by homophony. 





Mandarin Chinese has a large number of homophones, even when taking tone into account. The segmental and tonal combination mǎ, for example, is ambiguous between 马 ‘horse’, 码 ‘code’, 蚂 ‘ant’, 玛 ‘agate’, and so on. Just knowing the phonological properties of the word is not enough.3 





To disambiguate all these meanings, let’s use the simple, dummy “radical”, numeral again. But instead of assigning numbers to tones, let’s assign numbers to the different meanings that the segments _ma _can have, say 马1 is ‘mother’, 马2 is ‘hemp’, 马3 is ‘horse’, 马4 is ‘code’, 马5 is ‘ant’, and so on. Then for a different segmental combination such as _ba _(whose segmental radical is 巴), we use the numeral radical again, so that 巴1 is ‘father’, 巴2 is ‘take’, 巴3 is ‘palladium’, and so on. We repeat this numeral assignment process for every possible segmental combination in Chinese (_pa_, _na_…).





This alternative system is clearly cumbersome and difficult to learn. Learners of this system would have to memorize exactly which number corresponds to which meaning. It does not help that the number–meaning combination is completely arbitrary. For example, there is no clear relation between the number one and ‘mother’, or between number two and ‘hemp’. Furthermore, the memorized knowledge of number–meaning combinations for _ma_ does not transfer to _ba_. After memorizing the combinations for _ma_, the learner has to start over, and memorize the combinations for _ba_ again. 





To facilitate learning, rather than arbitrary numeral radicals, we can assign slightly more meaningful radicals to meanings. To ‘mother’, we can assign a radical that reminds the learner that the word has to do with motherhood, but not hemp, horse, code, or any other confusable meaning corresponding to _ma_. 





This system is actually very similar to the existing one. In the existing system, 妈 ‘mother’ has a radical on the left side 女 in addition to the segmental radical on the right 马. This left-side radical has nothing to do with the phonological property of ‘mother’, but vaguely suggests its meaning. 女 means female, which distinguishes 妈 ‘mother’ from all the other meanings with the same segments _ma_ because 妈 ‘mother’ is the only one that is related to femaleness. Let’s call this left-side radical of 妈 its _meaning radical_. It is essentially an advanced version of the dummy numeral radical I proposed. It is a mnemonic that helps the learner memorize the semi-arbitrary grapheme-to-meaning assignments.





Having a meaning radical also allows the learner to transfer knowledge from one segmental combination to another. For example, meaning radicals assigned to _ma_ can be reused for _ba_, so that a learner does not have to start over again. The meaning radical 口 (suggesting the character is related to mouths) can be combined with the segmental radical for _ma_, generating 吗, a sentence-final particle (it is vaguely related to mouths due to its discourse/speech-related function). It can also be combined with the segmental radical for _ba_, generating 吧, another sentence-final particle. Every character has a segmental radical, and most of them also have a meaning radical.4, 5 There are over 200 radicals in total.





This raises a further question: we know the existing system is pretty good for its ability to disambiguate homophones while being relatively easy to learn, but exactly how good is it? How efficient is it at assigning meaning radicals to different meanings? Given a segmental radical, a maximally efficient system should make all the necessary meaning distinctions (such that there is no ambiguity), while keeping the total number of meaning radicals as low as possible. In other words, it should have the lowest number of redundant radicals possible.





A good designer of Chinese orthography should achieve this goal by first examining all the meanings that share the same segment (e.g. for _ma_, it is ‘mother’, ‘hemp’, ‘horse’, ‘code’, ant’, ‘agate’, etc.). Then they should create the meaning radicals, so that every meaning has a distinct meaning radical (for _ma_, we should create a meaning radical for ‘mother’, a meaning radical for ‘hemp’, a meaning radical for ‘horse’, and so on). Then in order to minimize the redundancy of these meaning radicals, the designer should make sure that the meaning radicals they created for _ma_ can be maximally reusable for the meaning space of the other segments, e.g. _ba_. [Jon Gauthier](http://www.foldl.me/) and I are currently working to find the most efficient allocation of meaning radicals given the segments, and compare this allocation system with the existing Chinese system.





So far, we have taken the segmental radical as a given, and asked how to manage the inventory of meaning radicals most efficiently. If we can alter the structure of the segmental radical, the writing system will be improved significantly. Suppose that instead of the segmental radical, we use a “phonological” radical, which encodes _both_ the segmental properties and the tone. For example, we can borrow the five diacritics from the Romanization system _pinyin_, so that the phonological radicals for mā, má, mǎ, mà, and ma are 马̄ , 马,́ 马̆ , 马̀, and 马 respectively. Then we can significantly reduce the number of meaning radicals needed because the confusable meanings given the segments _and_ the tone (e.g. mā) are way fewer than the confusable meanings given just the segments (i.e., where the tone is not specified, e.g. ma). This system requires a combination of segmental radicals like 马, the five tonal diacritics, plus a small number of meaning radicals. The radical required by this system are far fewer than what’s required by the existing system, which demands a combination of segmental radicals plus a large number of meaning radicals. 





Therefore, the existing Chinese orthography provides a pretty good solution, but there is certainly space for improvement. If we believe that languages evolve over time to become more efficient (a common assumption in the study of language evolution), does this assumption apply to writing systems, too? If so, why doesn’t Chinese orthography follow obvious ways to improve itself, e.g. by adopting the system I just outlined? Chinese orthography has changed a lot over its history, and did these changes occur as an effort to improve? A speculation is that some changes are more costly to adopt than others. It may be cheaper to add or delete some meaning radicals under the existing framework, than to change the framework itself (e.g. replace all segmental radicals with phonological radicals). I leave this question of cost-sensitive, incremental evolution for another post.





I’ve argued in this post that written language doesn’t likely serve the function of recording speech, as it both over-documents and under-documents important features of spoken language. I suggested instead that the function of written language might be to clearly map to word meanings, and drew on evidence from Mandarin Chinese to show that distinguishing lexical meanings already plays a role in the structure of a writing system. It is not clear that written Chinese distinguishes lexical meanings efficiently or perfectly. In future posts, I will further explore alternative writing systems based on the Mandarin example to ask how efficient this system is.





[1]: Interestingly, while English over-documents certain aspects of word-level phonology (by spelling out homophones differently), it under-documents other aspects of word-level phonology, specifically lexical stress. English stress is a lexical property, as the same combination of consonants and vowels can mean different things depending on the location of stress, e.g. the nominal use of _record_ vs. the verbal use of _record_. Clearly English writing does not specify stress placement, hence creating ambiguity with the written word _record_.





[2]: This does not always seem true, as homographs are often tolerated. These are written forms that correspond to different meanings, e.g. _lead_ in English (ambiguous between the act of directing and a metal). Unlike in writing, the different meanings of _lead_ are actually distinguished by sounds ([li:d] vs. [lɛd]), so _lead_ is a case where phonology is better at disambiguation than orthography. There are also cases where homophones are not distinguished in writing, e.g. _light_, _bank_, and _ball_, where orthography does just as poorly as phonology at disambiguation. I speculate that while the goal of orthography should be to clearly map forms to meanings, occasional failures are tolerated, especially when the meanings are different enough, and the context can usually help distinguish them. They also suggest that orthography is not perfect, a point I will briefly discuss at the end of the post. This is again why Mandarin Chinese may be a more instructive case of study: it has far more homophones than English, and presents a more challenging problem to distinguish homophones in writing. 





[3]: One might hope that the context in which the character is used can help distinguish these homophones, but context is not always helpful. One example where contexts don’t help to disambiguate meanings is names. Chinese human names are typically two to four syllables long. Organizational names are more varied in length, but in general short as well. Each syllable has its own meaning that is represented by a character, and contributes to the meaning of the name as a whole. The contexts in which names are mentioned often do not help to distinguish exactly the meaning of each syllable. However, names are probably the first thing someone learns to write when they learn writing. 





[4]: There are two types of characters in Chinese orthography. The first consists of radicals that compose with each other in the way I outlined, such that one radical encodes segmental information, and the other encodes meaning. The second type is a pictograph that does not consist of radicals which compose in the way I outlined. For example, 耳 (ĕr) ‘ear’ is derived from the image of an ear. An interesting example of the second type is 取 (qŭ) ‘take’, which can apparently be analyzed as consisting of two radicals, 耳 (ĕr) ‘ear’ on the left and 又 (yòu) ‘right hand’ on the right. They don’t compose in the way I outlined. Instead, together they make the image of a hand grabbing an ear, which alludes to the custom of taking the ears of dead enemy soldiers. I do not consider characters like 取 decomposable into a meaning radical and a segmental radical. For the purpose of this post, I take characters like 取 to consist of just one radical, a segmental radical. This is because 取 can combine with a meaning radical like 女 ‘female’ to generate 娶 (qŭ) ‘to marry’. 





[5]: The actual picture is more complicated than what I presented here. A segmental combination may be represented by different segmental radicals. For example, 马 and 麻 are both segmental radicals for _ma_. They may combine with the same meaning radical 口, generating different characters: 吗 and 嘛. Because both characters are sentence-final particles, and indicate the discourse property of the sentence, they share the meaning radical 口, which suggests the character has to do with mouth. Here what serves to disambiguate the two characters is in fact not the meaning radical, but the segmental radical.
