---
author: dfwu
comments: true
date: 2019-09-15 02:10:13+00:00
layout: post
link: https://dfwu.wordpress.com/2019/09/14/why-not-linear/
slug: why-not-linear
title: Why we can never be sure that a human or a neural network has a grammar that
  uses hierarchical structure
wordpress_id: 69
categories:
- CogSci
- Syntax
tags:
- cognitive science
- computer science
- hierarchical structure
- linear order
- neural networks
---

MIT Linguistics is offering a new course this semester called "Linguistics for Researchers in Computer Science, Cognitive Science, and Related Fields". As the TA, I gave an opening speech at the beginning of the first class. Here is my speech
<!-- more -->

, and I added at the end additional thoughts that weren't put into the speech:





Hi everyone! Welcome to the class. Whether your research is in Natural Language Processing, cognitive science or any other language-related topic, you may find some of these topics interesting: what do speakers know about their native language? Can we find a general theory to characterize this linguistic knowledge? How is this knowledge learned? For cognitive scientists who study language, these are the topics of primary interest. For NLPers who want to find an efficient algorithm for processing human languages, knowing about the linguistic features of human languages would be helpful, too. These are precisely the topics of this class, so you are in the right place.





In addition to gaining linguistic knowledge, I hope this class achieves a more ambitious goal: hopefully it helps us become better researchers. 





Here is what I think makes a great researcher, and why I think this course will help us in that direction. Great researchers are broad: they read broadly, think broadly and have a broad knowledge. They may work on an apparently narrow topic, but they always bear in mind the bigger questions behind it, and situate their research in a grand picture. Great research requires breadth. In science, as we try to discover the order behind a phenomenon, a deep answer to a question often relates a broad range of phenomena.





But it’s very expensive to be broad: you may want to attend a talk in another department or read a paper in another field, but they are often too specialized and too dense to understand. That is why I co-organize [CompLang](https://complang.mit.edu/), a discussion group that engages members of CSAIL, BCS and linguistics. CompLang bridges between these fields. Instead of assuming a lot of prior knowledge from the audience, presenters are required to make their talk accessible to people who have very little background in the topic, bearing in mind the diversity of the audience. CompLang is in some sense a predecessor to this course. It is through organizing CompLang that I realized how important these inter-disciplinary discussions are to all of us.





From my experience, these discussions allow participants to take a step back and reflect on their own research approaches. I will show you what I mean by sharing one of my own intellectual journeys at CompLang. It is told from my perspective as a linguist, learning from computer scientists and cognitive scientists. But I hope (and am sure) that you will have similar gains in the other direction. I hope that by thinking about linguists’ approach to language, you will get to compare and reflect on your own approach as well.





In cognitive science and linguistics, researchers are interested in the questions of what are the initial state (factory settings) and final state of human language knowledge, and what a child experiences as they get from the initial state to the final state. The traditional approach is to study how humans learn languages, but in recent years some researchers have started to study this topic by looking at how neural networks learn languages. 





For example, we know that human language knowledge can be described in terms of hierarchical structures like trees. It leads to the question of where this property of languages comes from: are humans born with a bias favoring hierarchical structure? If the hierarchical structure of language cannot be learned only based on the sentences that children hear, then this innate bias is necessary. But if it can be learned only based on the sentences that children hear, then this innate bias is not required. 





Some researchers showed that a neural network language model with no prior bias for any hierarchical structure can nevertheless learn linguistic phenomena that refer to hierarchical structure only based on the input. They take this as evidence against the view that hierarchical structure is innate.





Let’s put aside the questions of whether human children and neural networks are on an equal footing in these studies. The question I was most interested in when I heard about research like this was: how can we be sure that a neural network has successfully learned a linguistic phenomenon? 





Suppose that a neural network language model can provide us with a “grammaticality judgment” for each sentence presented to it, that is whether the sentence is grammatical or not. Again, let’s set aside the question of what kind of measurements from a neural network can be interpreted as a “grammaticality judgment”. We can then ask whether the judgments made by a neural network align with those that would be made by a human. If they align, then researchers conclude that a neural network has learned the same linguistic knowledge as a human. Assuming that humans’ linguistic knowledge makes reference to hierarchical structure, so must a neural network’s.





Take the example of English verb agreement. Linguists claim that the verb always agrees in number with the subject. If the subject of a sentence is plural, then the verb must be plural, as in (1) and (2) (* indicates that the sentence is judged ungrammatical by humans):





(1) The keys are lost.  
(2) *The keys is lost.





If the subject is singular, then the verb must be singular, as in (3) and (4):





(3) The key is lost.  
(4) *The key are lost. 





Crucially, this verb agreement rule can be described by hierarchical structure, but not by linear order. For example, based on the grammatical sentence “The keys are lost,” one may think that _the verb agrees with the first thing linearly to its left_, that is “keys”. But this is not true, as is shown by the following sentences:





(5) The keys to the cabinet are lost.  
(6) *The keys to the cabinet is lost.





In fact, a rule is doomed if it only refers to the first, second or third thing linearly to the left of the verb. Instead, a rule that refers to agreement with the “subject” is successful. Since the concept of “subject” cannot be described in terms of linear order, but can be described with trees, we say that the verb agreement rule uses hierarchical structure.





Now suppose that we can show that a neural network judges correctly “The keys are lost” to be grammatical, and “The keys is lost” to be ungrammatical, can we then conclude that the neural network has learned the verb agreement rule in English, and therefore has learned a hierarchical rule? 





Probably not, because the neural network may have only learned the linear rule I just mentioned, that is the verb agrees with linearly the first thing to its left. To make sure the neural network is not adopting this hypothesis, we can test it with more complicated sentences like “The keys to the cabinet are lost.”





Suppose it still gets it right. Can we then be sure that the neural network has learned a hierarchical rule? Can we think of a linear rule that can still give the correct judgment to this complicated sentence? I think so! Such a linear rule might be: _the verb agrees with the first noun to its left that does not follow by a preposition_. This rule may sound a little complicated, but it is only based on linear order, and is sufficient to help the neural network “fake” as a human and give the correct judgments.





We can think of an even more complicated sentence to exclude this complicated linear rule, but we can always find an even more sophisticated linear rule to cover it. And we can repeat this exercise infinitely.





We can think of an even more complicated sentence to exclude this complicated linear rule, such as (7) and (8):





(7) The keys that the carpenter made are lost.   
(8) *The keys that the carpenter made is lost.





Suppose the neural network still gets it right. Can we be sure that it has learned hierarchical structure? No, because a linear rule would still be compatible such as: _the verb agrees with the first noun to its left that does not follow a preposition or “that”_. In fact, this exercise can be repeated infinitely.





What this exercise taught me is that **we can never be really sure that the neural network has learned hierarchical structure**. **No matter how difficult the test sentence is, we can always find a complicated linear rule that covers it successfully.**





Then how will we ever know that the neural network is not using an extremely complicated linear rule? How can we ever conclude from grammaticality judgments that the neural network has learned to use hierarchical structure? 





As I asked this to myself, I started to reflect on **how linguists came to the conclusion in the first place that human’s linguistic knowledge is hierarchical. Didn’t they draw this conclusion also based on grammaticality judgments, or more broadly, humans’ behavior that can be observed?** Why did no one challenge the linguists like I challenged the researchers of neural networks, and claimed that **humans just have an extremely complicated linear system? **





This might be possible, but at some point this linear system becomes so complicated that it is very unlikely that humans use it, and young children learn it. In science, if we find two hypotheses that can explain the data equally well, then researchers tend to favor the simpler one. Suppose that all humans have this bias for simplicity, and suppose that a hierarchical rule referring to the sentential “subject” is simpler than an extremely complicated linear rule,[1] then all humans will converge on the hierarchical rule. 





**If we treat a neural network like a psychological object (a human), which is what these researchers do, then why can’t we also give up as the linear rule gets too complicated, and say the neural network can’t have chosen that? Then, it must have learned hierarchical structure. **





You may wonder **whether we can really treat a neural network like a human**. For example, what is the criterion for “simplicity” for a neural network? Is it the same as researchers’ or human subjects’ criterion for “simplicity”? 





Anyway, this is my own intellectual journey at one of the CompLang talks last semester. We started from a specific project. By thinking critically about the project, I started to look back at what I had taken for granted, and reexamined my own implicit assumptions. **In the future, when I hear the claim that human language is hierarchical, I know to put an asterisk on it, and know that we actually can’t be 100% sure of that**. Furthermore, this thought process created deeper questions that lingered: if there is a criterion for simplicity followed by researchers, do human subjects and neural networks follow it too? 





**These are not the questions you can only get to by attending a talk on neural networks. You can get to the exact same questions from the other direction, by going to a linguistics class like this one**. For instance, a syntax lecture may show you many sentences, and linguists’ hypothesis based on those sentences. You can ask the same question as I did: is this the only hypothesis compatible with these sentences? Can I think of any alternative explanation? Why did linguists come to this particular conclusion as opposed to any other? What is the assumption behind this conclusion? Is it different from the assumptions behind my research? By asking these questions, I hope that you not only gain linguistic knowledge, but get to reflect on the bigger questions that relate our fields, and become a broader scientist.





But don’t feel pressured to only ask these types of questions in this class. Feel free to ask anything you want. We especially welcome clarificational questions. For example, if you hear the professor use the word VP a lot and don’t know what it means, feel free to ask. This is a new course, and we are as new to this course as you are. No question is inappropriate. By asking questions, you also help us know what works and what doesn't.





[1]: Can we be sure of this though? We would need a simplicity metric, against which we can compare different rules. Then we can tell which rule is simpler: a rule that only uses linear order; or a rule that relies on hierarchical structure like trees.  
---------------------------





Here are more thoughts that weren't put into the speech:





There should also be meta-evaluation of simplicity of sampling processes. For verb agreement, based on the sentences a child or a neural network has heard, there are always an infinite number of ways to describe the verb agreement rule that would be compatible with all the data. This infinite space of compatible descriptions includes the rules that this blog post has mentioned, as well as other strictly linear descriptions and hierarchical descriptions, but it also includes many descriptions that no researcher has ever thought of. For this reason, I think this space is massive, and more importantly, very messy, in that we cannot properly divide it into a finite number of segments.





The messiness and infinity of this description space begs the question of how children or neural networks sample and choose descriptions from this infinite and messy space.





In the speech I have assumed that a child or a neural network looks at this infinite space of descriptions, and chooses the “simplest” one, whatever that means. But one can think of a “simpler” way of sampling: instead of looking at this infinite description space altogether, a child or a neural network can just randomly take five descriptions from this space and compare them. The simplest one in these five that works is kept. If none of them works, then five more descriptions are sampled until we find one that works. Why don’t we assume this is how a child or a neural network does?





Also, I think it is useful to keep doing the exercise mentioned in the speech seriously until we find a linear description that would cover all the data concerning English verb agreement that can ever be conceived of. In other words, it is worth finding that "extremely complicated linear rule". Then we can compare this linear rule with the hierarchical rule that refers to agreement with the sentential subject. Suppose that all humans converge on one of these two rules - say, all humans actually follow the hierarchical rule - then presumably the hierarchical rule wins out because it is considered simpler by the "human language system". We can then reverse-engineer a human language system so as to guarantee the win of the hierarchical rule over the linear rule. If we do the same exercise for all the other grammatical phenomena, then eventually we will get a pretty good idea of the human language system through reverse-engineering.





For instance, to continue the exercise mentioned in the speech a bit further, while the linear hypothesis (_the verb agrees with the first noun to its left that does not follow a preposition or “that”_) could cover the 8 examples, it fails to cover the following:





(9) John said that the keys are lost.  
(10) John said that the keys is lost.





This calls for a revision to the linear hypothesis. Suppose that the linear rule scans a sentence from left to right. It matches the first verb it sees with a noun following this rule: _the verb agrees with the first noun to its left that does not follow a preposition_. Then the second verb it sees _agrees with the first noun to its left that (1) does not follow a preposition and (2) has not been matched with a verb yet_. Therefore, this linear rule can be summarized as _the verb agrees with the first noun to its left that (1) does not follow a preposition and (2) has not been matched with a verb yet_.





Can you think of an example that this revised linear rule does not cover, and think of a revision to the linear rule so that it can be covered by your revision?
