# Explaining the point of HoTT on FOM
## Urs Schreiber 2014-10-22

There is a mailing list "Foundations of Mathematics" -- or FOM for short. 

http://www.cs.nyu.edu/mailman/listinfo/fom/

This tends to be dominated by what one might call traditional set-based foundations. In any case, ever since homotopy type theory arrived on the scene

http://ncatlab.org/nlab/show/homotopy+type+theory

one sees contributors on the list refer to it by hearsay and publically wonder as to what the point of it may be, as if speaking of some mystical animal of which one heard rumours. More recently Prof. Harvey Friedman, who sort of dominates the list, was repeatedly asking for someone to tell him what the point actually is (never forgetting to add that whatever the point should be, it would be handled better by somebody trained in traditional foundations, such as himself).

In reply to this, one sees users mentioning the usual perceived advantages of HoTT as a theory of sets

http://ncatlab.org/nlab/show/set+theory#ReferencesInHomotopyTypeTheory

for instance that it provides quotient types, that it provides isomorphism invariance.

But this is like praising a car for having a horn, like praising an jumbo jet for having wheels, like praising CERN for inventing the WWW. It's true and it's neat, but it misses the Elephant in the room. In fact it misses the infinity-Elephant in the room.

The following used to seem too obvious to me to re-amplify much. But as time passed by, I grew to realize that the following is not actually widely appreciated, in fact it is being downplayed by some prominent practitioners. But instead, it deserves to be shouted from the rooftops. The following I posted to FOM October 22, 2014 .

http://www.cs.nyu.edu/pipermail/fom/2014-October/date.html

>>>
It had been mentioned here before that homotopy type theory [1] offers some advantages for formal set-based mathematics, such as providing quotient types and isomorphism invariance. What seems not to have been mentioned much before here is that the key point of homotopy type theory however is that it goes way beyond this in that it provides a native (i.e. direct, synthetic, see below) formalization not just of constructive set theory, but of homotopy theory [2] (aka algebraic topology). And the neat thing is: of homotopy theory in its modern and most powerful incarnation in the guise of infinity-toposes [3].

Just like plain dependent type theory is the internal language of locally cartesian closed categories, so homotopy type theory is the internal language of locally cartesian closed infinity-categories, and
homotopy type theory with univalent type universes is the internal language of infinity-toposes [4, 14]. This means that homotopy type theory provides a "structural" foundation of the kind that William Lawvere had found in topos theory [5], but refined to homotopy theory in the refined guise of infinity-topos theory.

My statement that the mathematics of homotopy theory and algebraic topology is beyond the scope of what may practicably be implemented in tradtional set-based foundations was not meant to be provocative. Looking at the mathematics that has been implemented in set-based foundations over the years [6] and extrapolating this progress into the future, it seems uncontroversial to me that the formalization of just the basics of simplicial homotopy theory [7] and higher topos theory [8] in traditional set-based mathematics is prohibitively tedious, and that using traditional set-based mathematics to engage in the formalization of proof of theorems of practical interest in these fields is out of the question, not in principle of course, but for all practical purposes.

And yet, homotopy type theory natively knows about all this.

For instance the formal proof [9] of the Blakers-Massey theorem [10] does not need to begin by first formalizing what a simplicial set is, what a Kan fibrancy condition is, what the infinite tower of homotopy groups is, what weak homotopy equivalences are, what homotopy pushouts are, how they reflect in long exact sequences of homotopy groups; because all this is native to homotopy type theory. Accordingly, the proof [9], on top of being a formal proof, is elegantly transparent and of actual practical interest. Moreover, since the formal HoTT proof [9] generalizes the traditional statement to more general infinity-toposes, it is actually a genuine new mathematical result of genuine interest in modern homotopy theory, to practicing mathematicians not concerned about foundations. This seems to be a kind of achievement unheard of [6] within the traditional formalization of set-based mathematics.

The reason why this may happen with homotopy type theory, the reason why homotopy type theory provides not just any but provides a practical foundation for mathematics including modern homotopy theory/algebraic topology, is that it provides a "synthetic" language for these topics, which allows to formally speak about the basic concepts natively without the need to first formalize several textbooks worth of material starting from bare set theory to even get started.

To my mind these are statements of the obvious to anyone who looked into the matter. The fact that they are not more widely appreciated is not due to this being possibly controversial, I believe, but because the intersection of the sets of researchers who genuinely appreciate modern homotopy theory in the guise of higher topos theory and those who appreciate formal logic, type theory and what it means to have an internal language of a higher topos is very small.

Indeed, also various practitioners of homotopy type theory care only about the truncation of the theory down to set theory, to "hsets" [11]. The crucial relation of homotopy type theory to higher topos theory was Steve Awodey's vision [12]. It has been realized notably by Mike Shulman [13,14], Peter Lumsdaine [15] and others and deserves to be more widely known.

Mike Shulman's 2012 course notes [16] are possibly still the best introduction on this matter. Anyone trying to get an idea of what the point of homotopy type theory is as a new practical foundation for modern high-level mathematic rooted in homotopy theory and higher topos theory could do worse than starting with these notes.


[1] http://ncatlab.org/nlab/show/homotopy+type+theory
[2] http://ncatlab.org/nlab/show/homotopy+theory
[3] http://ncatlab.org/nlab/show/(infinity,1)-topos
[4] http://ncatlab.org/nlab/show/relation+between+type+theory+and+category+theory
[5] http://ncatlab.org/nlab/show/ETCS
[6] https://plus.google.com/+UrsSchreiber/posts/YS6asZLgbbj
[7] http://ncatlab.org/nlab/show/Simplicial+homotopy+theory
[8] http://ncatlab.org/nlab/show/Higher+Topos+Theory
[9] https://github.com/dlicata335/hott-agda/blob/master/homotopy/BlakersMassey.agda
[10] http://ncatlab.org/nlab/show/Blakers-Massey+theorem
[11] http://ncatlab.org/nlab/show/set+theory#ReferencesInHomotopyTypeTheory
[12] http://ncatlab.org/nlab/show/homotopy+type+theory#Awodey
[13] http://ncatlab.org/nlab/show/homotopy+type+theory#Shulman12
[14] http://ncatlab.org/homotopytypetheory/show/model+of+type+theory+in+an+(infinity,1)-topos
[15] http://ncatlab.org/nlab/show/higher+inductive+type#ShulmanLumsdaine12
[16] http://ncatlab.org/nlab/show/homotopy+type+theory#ShulmanCourse﻿


----

### Andrej Bauer
I cannot find your post on FOM archive, by the way. Gosh, some of the stuff there is painfully difficult to read. The only thing worse than arrogance is arrogance combined with ignorance.﻿

### Andrej Bauer
I would propose the following challenge: formalize the construction of real numbers. I am not even aware of a published account that actually proves everything that needs proving (such as associativity of multiplication).﻿

### David Corfield
I haven't tuned into FOM since the dark days of Colin McLarty's valiant defence of category theoretic foundations against the naysayers. The ground was not fertile for the emergence of any intellectual curiosity for a foundations that can speak to important developments in central parts of mathematics and mathematical physics.﻿

### Andrej Bauer
I left the list a while ago (fed up with moderator's whims) and whenever I check out the archive I am glad I am not there anymore.﻿

### Dee Roytenberg
Not sure about "aka algebraic topology". I mean, I know what you mean but to most practicing mathematicians, algebraic topology is but a rather specialized and technical subfield of mathematics, so they won't get what the bid deal is. E.g. they'll wonder why homotopy theory should form foundations of mathematics if one needs the set of real numbers to even define what "homotopy" is? (wrong, of course). You'll need to find a way to convince them that the "higher stuff" is more fundamental than its topological incarnation. 

(And btw, what is special about the 1 in (oo,1) from the foundational perspective? I.e. why isn't there an "(oo,n) type theory"? That's my own question)﻿

### Gershom B
The list is moderated, so posts take time to appear, and indeed now it is there.

In any case, here is a question: you write that hott with univalence is "the internal language of infinity-toposes". Then I go to the n-lab page and am told to see the page on higher topos theory for more (http://ncatlab.org/nlab/show/higher+topos+theory). Then I go there and am told that (∞,1) categories have been explored, but otherwise rather little is known. So can we make such a bold claim yet? Or is the claim rather "whatever we want an infinity-topos to be, HoTT seems to get us there?" Or is the answer "infinity-1 is good enough"? Or is the answer "we really need to update that page" :-)?﻿

### David Roberts
I posted something in response to Friedman, after Tim Chow (who I find much less dogmatic) pointed out that the proper response to Urs' prior posting is not to harrumph about non-logicians doing foundations, but to take up the challenge of actually trying to formalise mathematics in set theory. It's here: http://www.cs.nyu.edu/pipermail/fom/2014-October/018249.html. If people could point out a date by which Blakers-Massey was proved, I'd be grateful.﻿

### David Roberts
+Dee Roytenberg I would point them to Voevodsky's proof of the Minor and Bloch-Kato conjectures. In his recent video interview, VV mentions how these are purely algebraic questions (and even number theoretic), and their proof required motivic homotopy theory, which we now recognise as sitting in the infinity-world.﻿

### Chris Brav
I have the same question as Gershom B. About HOTT and (\infty,1)-categories: what is the state of affairs? I asked Lumsdaine and Voevodsky about this a number of time in the last year. VV said that he considered a good formulation of (\infty,1)-categories in HOTT the most important open mathematical problem in HOTT, the difficulty being (as usual) to talk about homotopy coherent associativity in a way that is less than 'prohibitively tedious'. Both Lumsdaine and Voevodsky said it wasn't even clear how to talk about loop spaces in a way better than usual.

### David Corfield
In the nLab spirit of not wanting the hard work of answering questions to be lost in ephemeral media, perhaps we should look to form a HoTT as Foundations FAQ along the lines of the string theory FAQ page
http://ncatlab.org/nlab/show/string+theory+FAQ

### Urs Schreiber
+Chris Brav +Gershom B Regarding models in (infinity,1)-topos: I had given direct pointers, see here: http://ncatlab.org/homotopytypetheory/show/model+of+type+theory+in+an+(infinity,1)-topos . More literature is linked to here: http://ncatlab.org/nlab/show/relation+between+type+theory+and+category+theory .

It has all been sorted out:

1) the rectification necessary on the model category in which one interprets is given by Lumsdaine-Warren;

2) The conditions necessary to check to have a model of HoTT without univalence in locally Cartesian closed Categories is due to a result that was independently given by Cisinski and Shulman and by Gepner and Kock

3) Shulman had shown that univalence is interpreted in a certain class of presheaf (infinity,1)-toposes. Gepner and Kock in their article showed also how univalent universes are interpreted in general (infinity,1)-toposes. However they glossed over the issue of strictifying the universe.

4) That is solved by adopting weak Tarskian type universes. (See the above links).﻿

### Urs Schreiber
+David Roberts I had intentionally not pointed to the suggestion that one might prove the Milnor conjecture formall in HoTT, because, while this would in itself be an excellent suggestion, the publically existing such suggestion goes along with the further suggestion that one should do this in the hset-truncation of HoTT. I doubt that this is feasible, by reasons expressed above. I didn't want to say this more explicitly, but it's the subtext of the line where I say that some HoTT practitioners try to downplay the homotopy-theoretic nature it has. I find this scores high on the scale of missed opportunities.﻿

### David Roberts
+Urs Schreiber I agree with your point. One can take what I wrote and make it just a link between algebraic topology/homotopy theory and "important mainstream mathematics", as Dee was asking.﻿

### Urs Schreiber
+Dee Roytenberg So Friedman was asking what one might mean by "high-level math" that would not be suitable for formalization in set-theoretic foundations. I was trying to find the most suitable name for it that people might recognize. While of course "algebraic topology" -- as already witnessed by by the unfortunate abuse of the term "topology" -- is not a good term for the abstract idea of homotopy theory, it is the de factor headline under which most of the work in homotopy theory is actually being published. And if one reads "topology" as a standin for "homotopy", as one has to, and reads "algebraic" as a standin for "abstract/axiomatic" (which is not far off), then it's not too bad, I think.﻿

### Urs Schreiber
+David Corfield While I also find the nature of the discussion on the list by and large less productive than it could be, at this point I thought it's time to try to inject some genuine information about HoTT into it.

(It strikes me, however, that specialists on foundations would rather comment the gossip and ask for information on a public list than simply go and read the primary sources.)

### Urs Schreiber
+David Roberts read your followup message to FOM now http://www.cs.nyu.edu/pipermail/fom/2014-October/018249.html

LOL, as they say. :-) It's fun. Maybe this is really what some readers there are after.

### Andrej Bauer
I have a new suggestion: Harvey Friedman should formalize **any** piece of mathematics that is above high school level.﻿

### Michael Shulman
Is Blakers-Massey actually completely formalized somewhere?&nbsp; The Freudenthal suspension theorem in the HoTT/HoTT library is still incomplete.

The gauntlet is fun, but of course it's not really fair because it's not comparing apples to apples. Claiming that a HoTT formalized B-M applies to all (oo,1)-toposes depends on the fact that all (oo,1)-toposes model HoTT, which is not yet formalized anywhere, let alone in HoTT where we don't yet even know how to define an (oo,1)-category.﻿

### Urs Schreiber
+Michael Shulman there is this code here

https://github.com/dlicata335/hott-agda/blob/master/homotopy/BlakersMassey.agda

which I suppose is what the HoTT book refers to on p. 300, where a table lists the Blakers-Massey theorem as "proven by computer".

I don't want to engage in whether its "fair" and other allusions to competition which are part of human vanity and outside the mathematics itself. I rather consider this to be a reply to Friedman's question, as to what the point of HoTT is.﻿

### Andrej Bauer
It's not worth expanding much energy on getting the FOMers to understand. They do not want to understand, they just want to know they're superior to everyone else.﻿

### Chris Brav
+Urs Schreiber I shouldn't have said that I have the **same** question as Gershom B. Rather, I was asking a somewhat similar question (what is the state of defining (\infty,1)-categories in HoTT). The answer seems to be (as +Michael Shulman has pointed out) that it isn't known how to do it. (Though I'd really like to see it done, since I'd like to be an end user rather than a developer of HoTT.)

I think the point that Urs is making is that HoTT is natural if you think models of (\infty,1)-topoi are natural. Or is it something more than that?

Also, it seemed from Friedman's comment that he was 'more suspicious' that such things were not rigorous means he really missed Urs's point, which is that HoTT can be modeled in (\infty,1)-topoi, the only known models of which are built in sets and would presumably &nbsp;be considered fairly rigorous by most people.

### Urs Schreiber
+Chris Brav wait. There is ordinary proof that HoTT has interpretation in (infinity,1)-toposes. For that we do not need to define (infinity,1)-categories internal to HoTT and indeed that's part of the point, that HoTT already knows what (suitable) (infinity,1)-categories look like "from inside".

What Mike was referring to was the fully formal proof (or lack thereof) of the statement (which does have ordinary proof) that HoTT has models in (infinity,1)-toposes. One might want to try to prove this formally within HoTT itself. This is related to the general issue of eventually erasing all recourse to set theory and consider HoTT and only HoTT and build its models inside itself.

While that would be nice, it goes quite a bit further than what is at issue here. If one really adopted this position that we speak of nothing but what has fully formal proof, then of course the discussion pretty much collapses. For instance we also don't have fully formal proof that axiomatic set theory has a model in the category of sets or the like.﻿

### Charles Rezk
I wish I knew for sure that the proof in [9] is "elegantly transparent and of actual practical interest". Unfortunately, I can't make any sense of it (I would very much like, and I've tried to). It is basically a big pile of (uncommented!) agda code, and conveys essentially little meaning for me. I can't even identify a statement of the theorem in it.﻿

### Michael Shulman
By "fair" I didn't mean to talk about competition and human vanity, but to say that we shouldn't exaggerate what we can do with HoTT by pointing out how difficult it would be to do in set theory something that we haven't actually done in HoTT either.﻿

### Michael Shulman
+Charles Rezk yeah, that is the curse of formalized proof -- that when people have formalized a proof they may neglect to explain it to human beings.﻿

### Urs Schreiber
+Charles Rezk, +Michael Shulman that code was the reply to Mike saying that the theorem has not been computer-formalized yet. (Mike?)

The claim that that code translates to a nice ordinary language proof was the content of a talk that +Peter LeFanu Lumsdaine gave in Barcelona a while back. As far as I know there is going to be a proccedings article to go with this, though the publishing process of these proceedings takes place on geologic time scales. The abstract of Peter Lumsdaine's talk is here:

http://www.crm.cat/en/Activities/Documents/AbstractsTypeTheory.pdf

"One such result, the Blakers-Massey connectivity theorem, is of particular interest in that all classical proofs use some specifics of their settings (usually, Top or SSet) not available to us; so the type-theoretic proof was, by necessity, new in parts. This allowed us, as a by-product, to translate the proof back into classical language and obtain the theorem in wider generality than was previously known: we show that it holds in any infinity-topos (in the sense of Lurie).
I will introduce the Blakers-Massey theorem and our approach to it, and discuss the process of translating a type-theoretic proof into infinity-categorical language."

I'll check with Peter if he has a writeup that he could share.﻿

### Urs Schreiber
+Michael Shulman the kind of work that you say needs to be done for this to be "fair" is the work necessary to formally show that foundations in HoTT are equivalent (or whatever the technical term is) to set-theoretical foundations (with the necessary qualifiers added for both). Of course this would ultimately be good to have. But the whole point here is that if one accepts HoTT foundations, then one does not need to do this to prove, say, Blakers-Massey. You would of course need to do it to formally show that this is the same theorem as something that one would call Blakers-Massey in formal set theory. But we need to start somewhere, and if we decide to start by translating the informal statement of Blakers-Massey to HoTT instead of ZFC to start with, then it may be proven there.﻿

### Michael Shulman
+Urs Schreibe I agree with that much. But there was also a claim that by proving it formally in HoTT we have automatically formalized the corresponding result for (oo,1)-toposes, and that's what I'm taking issue with.﻿

### Urs Schreiber
+Michael Shulman I certainly see what you mean, but I am wondering if this is not taking the level of "formal proof" a step beyond its usual meaning. Please help me try to understand this in traditional foundations first: applying this level of "formality" means that before accepting any formal proof in set theory as formal -- say Goedel incompleteness in general toposes -- we first need to formally show that the models in which we interpret the statement are really models of the axioms. &nbsp;Has that actually been done? Is there fully formal proof that toposes are models of constructive set theory?﻿

### Michael Shulman
I don't know, but certainly I think that is what we would need in order to say that the proof of some statement _in a general topos_ has been fully formalized. When working _inside_ set theory, to say that some statement like "Goedel's incompleteness theorem holds in an arbitrary topos" has been proven, we need to prove firstly that the theorem follows from the axioms of set theory, then also prove that the axioms are validated in any topos. That's just as true of formal proof as informal proof.﻿

### Urs Schreiber
Okay, I certainly see the point. If this is a fine print that matters, then of course I should be saying that there is fully formal proof of Blakers-Massey in HoTT which translates to a usual informal proof in any infinity-topos.

(By the way, what's a good way to say "not fully formal, but formal in the ordinary traditional sense of mathematics"? Saying "informal" seems not to capture this.)﻿

### Michael Shulman
(Yeah, that's a problem; maybe "rigorous" or "precise"?)﻿

### David Roberts
Yea, I kind of overstepped the mark a bit. But Mizar has had 40 years head start, so I reckon it evens out.﻿

### Urs Schreiber
+David Roberts ah no, don't get me wrong, I think it's good that you stated it in this way. It made _me_ laugh, because that's not how I usually think of raising interest in mathematical questions, but you are absolutely right that it seems some of the people on the list might be attracted to just this kind of comparison.

If it serves to increase awareness of "the issue", and it likely does, then it's very good.﻿

### Charles Rezk
+Urs Schreiber +Michael Shulman For what it's worth, it's long been known (to me, at least) that BM holds in any infinity topos, via the clumsy proof which ratchets up from classical BM in Top.  I think HoTT proof is mainly interesting in that it should translate into a new proof for Top.﻿

### David Roberts
And one HF now has the arrogance to refer to himself as a "true foundationalist", "entirely open" to new foundations. What is this I don't even...﻿

I need to go for a hard bike ride to cool off.﻿

### Gershom B
A friend reminds me "The only way to win at FOM is not to play"

edit: I am however glad to see that HF evinces a good knowledge of the work of of noted category theorist "MacClane"﻿

### Urs Schreiber
+Charles Rezk I seem to remember Peter Lumsdaine verbally citing you for this. Haven't thought about it much, so you argue locally/stalkwise?

+Gershom B as with much public discussion, the goal is not to win an argument against someone determined not to give in, but to provide useful information for the many silent bystanders and, on the web, the many more and ever more future readers. It's a bit about helping information percolate through the web.﻿

### Urs Schreiber
+Charles Rezk in fact on the nLab page [1] I have been crediting you for this ever since the entry came into existence over a year ago. But maybe it would be good to add to just the mentioning of your name there also a pointer to some kind of record. Or maybe directly record your proof there. Or something

[1] http://ncatlab.org/nlab/show/Blakers-Massey+theorem

### Charles Rezk
+Urs Schreiber Yeah.  "N-connected", "pushout" and "pullback" are all operations that can be computed stalkwise.﻿

### Dan Licata
+Urs Schreiber Favonia formalized Blakers-Massey in Agda; the code is here, I think: https://github.com/HoTT/HoTT-Agda/blob/1.0/Homotopy/BlakersMassey.agda but you should ask him what version to cite. The one in my library is not complete.﻿

### Urs Schreiber
+Charles Rezk thanks. But then it would still seem an improvement to have a fully internal proof, without reference to a site, no?

### Urs Schreiber
+Dan Licata thanks, but help me, how does that code compare to the one linked to here: http://ncatlab.org/nlab/show/Blakers-Massey+theorem#LumsdaineFinsterLicata13 .

? (Please feel invited to add information/links to that entry as need be.)﻿

### Urs Schreiber
+Dan Licata oh, I see, your are telling me to replace the link to your site with the one by Favonia. Okay, am doing so now.﻿

### Charles Rezk
+Urs Schreiber Oh sure.  But I think having a new proof for spaces, which only uses a few basic ideas (truncation,  decent), and no general position arguments would be great in itself.  I spent a bit of time looking for one and failed.﻿

### Urs Schreiber
+Charles Rezk okay, excellent. Thanks for the comment.﻿

### Dan Licata
For the HoTT Blakers-Massey proof: Peter Lumsdaine, Eric Finster, and I came up with a proof (using Agda a bit, but not trying to give a complete formalization). Favonia (a PhD student at CMU) formalized it in a separate Agda repository, and should get credit for giving a computer-checked proof of the theorem. There are a couple of partial formalizations in my Agda repository that explore some different options (trying to match up with infinity-topos language better), but none are complete, or suitable for anyone to look at at this point. So the one in Favonia's repository is the only complete computer-checked proof. I've moved the file you linked to originally so no one will get confused and try to read it. ﻿

### Urs Schreiber
+Dan Licata thanks for the information! I have rearranged accordingly on the nLab page and am citing now also +favonia mlatus here: http://ncatlab.org/nlab/show/Blakers-Massey+theorem#Favonia

### David Roberts
I've just unsubscribed from FOM. I can get set theoretic or foundational help from MathOverflow if and when I need it.﻿

### favonia mlatus
Thanks!﻿

### Urs Schreiber
Would it be hard to add a minimum of documentation to the code of the Blakers-Massey proof? Just a little commentary that would indicate roughly what the code does at which point? That might increase immensely the practical value of that code to others.

### Dan Licata
My advice for someone who wants to understand the proof would be: understand chapter 8 of the HoTT book, up to the Freudenthal suspension theorem, at which point after reading the basic definitions in the formalization (what the codes fibration is), you should be able to finish the proof yourself. &nbsp;Blakers-Massey follows the same structure, but with some more complicated definitions. &nbsp;But I'm not sure if that serves your rhetorical purposes :) Peter and Eric and I have been planning to write exactly the paper you want, but it hasn't made it to the top of the queue yet :(﻿

### Urs Schreiber
You must have been giving talks about this where you provide a more
generous commentary, no? I have heard Peter give an excellent such a
talk at CRM in Barcelona (that's where I got the whole idea of this
thread here) but apart from the talk abstract, I have no record of 
that talk that could usefully be shared.

### Michael Shulman
If one wanted to really try to explain (oo,1)-toposes to a set theorist, one could make an analogy to forcing. When you prove something in ZF, it's automatically also true in all forcing extensions. The same is true for constructive set theory, except that there are more forcing extensions since we don't have to force LEM; those constructive notions of forcing (which also subsume permutation models) are called "sites" and their models are called "1-toposes". Now in HoTT we have an even more general sort of forcing appropriate for homotopy theory, whose models are called (oo,1)-toposes.﻿

### Urs Schreiber
+Michael Shulman excellent, here we go: http://ncatlab.org/nlab/show/homotopy+type+theory+FAQ#WhatIsHoTTForSetTheorists

### favonia mlatus
+Urs Schreiber I mostly followed Dan, Peter and Eric's approach, with some divergence in the wrap-up proof of the main theorem, which I tried to make clearer and more understandable (than the draft I just copied down).﻿

### favonia mlatus
The core lemma that is also used by Freudenthal has been ported to the new Agda library by +E. Cavallo.

### Urs Schreiber
+favonia mlatus where did you "make it more understandable"? Do you mean your code at https://github.com/HoTT/HoTT-Agda/blob/1.0/Homotopy/BlakersMassey.agda ?

What I am asking for is whether you (or somebody) might write documentation for this code that makes understandable to the uninitiated what the proof is doing.

Recall what's happening above. Charles Rezk is an expert on all the mathematics that is involved. And he is eager to see the idea of the new proof, because he had been looking for such a kind of proof, he said, without finding it. But, alas, he is not an expert in Agda coding. The code behind the above link means nothing to him. Indeed, if I am reading the above exchange correctly, then even Mike Shulman, who on top of that is an expert on the coding, isn't sure what the proof is doing.

This is a pity. But there will be a way to say what the proof does "informally". If that description could be added publically visible somewhere, so that people like Charles Rezk could absorb it, that would be most useful.﻿

### Charles Rezk
+favonia mlatus's code is more approachable than the code I was looking at before, though I am now stuck at "cross-path"; I have an idea of what sort of trick it is supposed to involve (from the Freudenthal proof), but there isn't really an explanation for it.

Here is one question I have: the Freudenthal proof in the Book (which I think I understand pretty well) makes use of the fact that (Omega Sigma X) is the fiber of the path fibration over (Sigma X), and that the total space of this fibration can be built explicitly from pieces, based on the usual decomposition of (Sigma X). This is satisfying: the same decomposition is how you recognize that the James construction JX models (Omega Sigma X), and the James construction is the source of a (different) proof of Freuthenthal.

If the Blakers-Massey proof runs on similar lines to the Freudenthal proof, I would expect to see an analogous construction show up, so that a key object (perhaps the pullback of X --> P <-- Y where P is the pushout, or perhaps a path space lim({x} --> P <-- {y}), or perhaps a homotopy fiber lim({x} --> P <-- Y)), is seen as the fiber in some explicitly constructed fibration. But I don't know what this should be.﻿

### Charles Rezk
BTW, this is how I understand the proof of Freudenthal given in the book: http://www.math.uiuc.edu/~rezk/freudenthal.pdf

### favonia mlatus
+Urs Schreiber I made some efforts to make it understandable for people who are **already** familiar with Dan, Eric and Peter's informal proof. My difficulty is that, due to the lack of appropriate background knowledge, my intuition is usually not (immediately) understandable to others. I am happy to share my insights but I need to cooperate with others.

+Charles Rezk "Cross" refers to the Z-shaped path in one visualization of their informal proof. I made up the name.﻿

### Urs Schreiber
+favonia mlatus where is "Dan, Eric and Peter's informal proof" ?﻿

### favonia mlatus
+Urs Schreiber It was once on some black board of IAS last year when I kept bothering them for something for Agda. Sorry but I'm not aware of other sources...﻿

### favonia mlatus
+Charles Rezk "cross-equiv" mimics the equivalence (8.6.9) of the HoTT book in the case of Freudenthal. If you move all the "merid"s to one side then it's an equivalence about Z-shaped paths.﻿

### Urs Schreiber
+favonia mlatus I see thanks. What I am trying to ask you is whether it would be possible to add to your code some more hints that would make it understandable to people who were not at that board in that room at that time. Would it be hard? Just a few hints? Such as those you just gave to Charles? Charles is a good gauge: if he barely understands what's going on, this means that essentially nobody else will understand anything. Which is a pity, given your effort of writing that code!

(I am really somewhat thrilled by this. You have a proof of something that Charles Rezk is still trying to understand. This is exciting. It shows that something powerful is going on with the HoTT business. I wonder if you are fully aware of how peculiar this situation is...)﻿

### Bas Spitters
+Andrej Bauer There are several formalizations of the reals, some even compute. What did you mean?﻿

### Andrej Bauer
I meant: do you know of a published account (as in "on paper in a book") where all the details of the real numbers construction are actually proved, where they don't say "we leave the remaining 12 cases of associativity of multiplication to the reader"?﻿

### Bas Spitters
+Andrej Bauer Oh, dead trees, as they say. Landau's Grundlagen perhaps?﻿

### Andrej Bauer
The fact that nobody every does this, and that the real numbers are so important for everyday mathematics, tells us something about the ability of mathematicians to replace the mathematical method with wishful thinking and betting one's existence on a hunch.﻿

### Michael Shulman
+Andrej Bauer or maybe it tells us something about the ability of human mathematicians to recognize symmetries and patterns? A computer may need to be told explicitly how to prove each of the dozen cases, but a human can do one or two of them and see immediately that the pattern will generalize to the others.﻿

### Andrej Bauer
In the particular case of associativity of multiplication, I agree there is a lot of symmetry, but in my experience the whole thing just gets skimmed over. For instance, nobody say "a lot of the cases are symmetric, so there are just 5 essentially different ones to consider" but rather something like "let's check the case where all three numbers are positive, and leave the other cases to the reader". This is not actually recognition of symmetry but laziness. I understand we can't have the full proof in every book (or even one which takes account of symmetry), but we don't seem to have a proof at all, or at least not one that is easy to find. And after associativity there is still distributivity...﻿

### Andrej Bauer
For instance, the Coq standard library just takes the easy road and axiomatizes the reals (in a rather horrible way), so they don't have to check anything.﻿

### David Roberts
What if someone writes down the field (R,+,*,0,1) as a ZFC set in all its "glory"? And proves it is a complete ordered field? Yuk.﻿

### Bas Spitters
+Andrej Bauer We have checked it in corn (at least twice). I know there are other formalizations too.﻿

### Charles Rezk
So, I believe I understand the proof of Blakers-Massey as coded by +favonia mlatus. At least, I understand enough of it that I can fill in the rest.

It is a most excellent proof!

Here are a few things I've learned.

1. The theorem involves the pushout P of a diagram X <-- f -- Q -- g --> Y, and asserts the connectivity of the tautological map from Q to the (homotopy) pullback of X and Y over P. Everything in the statement is sliced over P. Since slices of an infinity-topos are an infinity-topos, this means that if we want to prove the theorem in an arbitrary infinity-topos, we might as well assume P is the terminal object.

That is, we reduce to the following statement: if X <-- f -- Q -- g --> Y has contractible (homotopy) pushout, then Q --> X x Y is (m+n) connected if f is m-connected and g is n-connected.

This means that in reading +favonia mlatus's code, for the most part you can pretend that P is not there; so you don't have to keep track of paths/identities in P, and you don't have to worry about transporting things along paths in P. This simplification makes things much easier to absorb.

2. There is one thing that always puzzled me about Blakers-Massey: the hypotheses do not merely assert that f is m-connected and g is n-connected: you also need to require that m and n are at least -1. This proof makes it clear why that is. Because m and n are at least -1, the composites Q --> P are also ( - 1 )-connected (surjections).

If we simplify and assume P=*, then this just means Q is (-1)-connected. Thus, to prove the result, it suffices to prove it after taking the product of everything with Q. 

The proof in the code actually does this: it directly involves constructions which live over the diagram Q x X <-- Q x Q --> Q x Y (whose pushout is Q).
(This is pretty explicit in the code: the new factor of Q is precisely the "(q_00 : Q x_0 y_0)" which appears in the module declaration in BlakersMassey.agda . It took me a while to realize its significance.) 

### Urs Schreiber
Excellent, +Charles Rezk, thanks. Are you going to write this up in the spirit of your note on Freudenthal which you linked to above? Would be most useful.﻿

### Charles Rezk
+Urs Schreiber I could, though I'd rather wait until +Dan Licata et al have their paper.﻿

### Charles Rezk
Actually, I think i take back point 2. Blakers-Massey (in the form I stated it), is still true if either m or n is -2. This proof doesn't deal with that case; it is a fairly anomalous case, though.﻿

### favonia mlatus
+Charles Rezk Thanks. I feel flattered by having you analyze the code.﻿

### favonia mlatus
+Charles Rezk If you have suggestions on the organizations and/or the words that I can add to make it _really_ understandable, I'm all ears.﻿

### Urs Schreiber
+Charles Rezk, +favonia mlatus yes, please. Don't keep this a secret for much longer, for the sake of the subject. Give credit to the people who came up with the proof and of course don't scoop their publication, but please produce an intelligible account of what's going on somewhere.
