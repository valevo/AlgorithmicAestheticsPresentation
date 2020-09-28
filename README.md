# Algorithmic Aesthetics Presentation


- Algorithmic Aesthetics = aesthetics of art produced by algorithms? or = aesthetic judgements by algorithms? <br>
  spoilers: at the end of this section, we'll look at aesthetic judgements of music by a computer!

# -1. Why?

- why would we even care what the computer (scientist) has to say about the aesthetics (of music)?

- usually, when computer science meets art, the computer scientist's job is done (and sent back to the dark basement) once the tool is created <br>
  -> artists then discuss the aesthetics of the created art among themselves <br>
  -> this section is a computer scientist's perspective on such a discussion 
  
- my opinion: putting aesthetics, specifically the aesthetics of the music created by our AI, into an algorithmic perspective is not just an excercise 
  but can also enrich the discussion: <br>
  it helps to connect to concepts and lines of thought not previously considered (also in a sense of providing feedback) <br>
  it can help understand better what AI does and how it changes out environment (including music) <br>
  it provides yet another mirror to our understanding of music as a whole and specifically the aesthetics we treat it with
  


# 0. Disclaimer

 - aim of this section: we'll be looking at aesthetics from a computer science perspective which means translating it into mathematical concepts (don't worry, you won't see any formulas)
   
 - it is doubtful whether human aesthetics can be fully captured by mathematics at all; <br>
   so, at least for the moment, no approach can fully cover the nature of what humans find aesthetically valuable; <br>
   on a related note, aesthetics likely has strong subjective aspects, so there likely isn't a unified/objective theory that works for any human and any context
   
 - with this in mind, the approach to measuring aesthetics I present in the following is only **one** approach of many neither me nor the original authors 
   would claim that it perfectly captures human aesthetics <br>
   it is remarkable, however, how close to human we can get by the argument and method, especially seeing how **simple** it is 
   (this is a play on words, simplicity will be a core concept
   
 - so this story is to be taken more as prototypical story from algorithmic science and not as "the" solution
   
# 1. Wittgenstein on Aesthetics

  - famous and highly influential philosopher of mind, language and science in the first half of the 20th century
  
  - has become somewhat of a favourite to AI and cognitive scientists for providing philosophical foundations 
  
  - his account of aesthetics is from the notes taken during a few lectures

## 1.1 What is an Aesthetic Judgement?

  - Wittgenstein starts with the observation that people tend to use words like "right" or "correct" when making aesthetic judgements
    (and not so much "beautiful" which is used more as a gesture) <br>
    e.g. "this is the right way of reading Goethe's poem", at the tailor: "make the sleeve a bit shorter for the right length"
    
  - according to Wittgenstein, aesthetic judgement is distinct from appreciation: 
    e.g. someone who doesn't speak English may still appreciate the sound of an English poem but could not make aesthetic judgements, 
         i.e. could not say if it was read "right" or whether the rhymes are "correct"
    

## 1.2 "Rules"

  - the crucial question then becomes: how have people learned in which situations to use the word "right"? <br>
    note: with this question in mind, aesthetic judgements are closely connected to linguistic expression

  - Wittgenstein's answer: in order to make aesthetic judgements, one must know the "rules" <br>
    one learns the "rules" from experts, peers, etc. 
    e.g. one needs to know English to be able to be able to admire the way in which words were used
    e.g. a trained musician might be able to make more detailed aesthetic judgements than someone who rarely listens to music <br>
    
  - what is an aesthetic judgement then becomes an expression of how much an object adheres to the "rules" in the eye of the observer 
   
  - comment: clearly, the way Wittgenstein sees aesthetics it is a societal or cultural concept, 
    i.e. what we find aesthetic is dictated by our cultural norms and values


# 2. Towards Simplicity: "Rules" and the Predictive Brain
 
  - for now, I'll just use the word "simple" like it's an everyday word but describe later what it denotes in the algorithmic context

## 2.1 "Rules"

  - although Wittgenstein may not have intended it, his view on aesthetics connects to simplicity, namely in two ways:
    1. society has a preference for simple "rules" (evolutionary pressures, psychological principles (see below), etc), so if an object adheres to the "rules" and is therefore judged to be aesthetic, then it is also inherently simple
    
    2. the less simple (i.e. the more complex) an object, the higher is its chance to violate the "rules" (any rule, in fact) <br>
       e.g. cooking: the more steps and the more ingredients in my cooking, the higher the chance to ruin the meal
       e.g. if I compose a highly complicated song, I run a high risk of producing something that is not according to the specific set of "rules" in my cultural context
 
 - the _simplicity_ of an object conditioned on the rules of society is equivalent to the thing's _adherence_ to those rules <br>
   => this is a mathematical consequence of the theory of Kolmogorov complexity


## 2.2 The Predictive Brain

  - there is a path from aesthetics to simplicity which is very much parallel to the one derived from Wittgenstein: the predictive brain; <br>
    a framework in cognitive science and neuroscience, the theory of the predictive brain assumes that our brain constantly predict what happens next 
    and then learns by comparing the reality to the predictions 

  - attempting to avoid uncertainty (evolution! -> uncertainty is dangerous), the predictive brain strives to surround itself with highly predictable things and contexts <br>
    simple things are easier to predict simply because they are more likely to occur (cf. likelihood principles and principles of symmetry and grouping; compare also to betting: one wouldn't want to bet on a very complicated event) and so by extension, the brain strives to be surrounded by simple things (in the converse, highly complex enivornments are usually those in which predicting the immediate future is very difficult, i.e. where there's a lot of uncertainty)
  
  - if we extend this (evolutionary) principle to those things and contexts we produce ourselves (e.g. art), then we should expect that we have a preference for making simple objects (because of the reward from our brain) <br>
  hence, treating aesthetics as related to preference, we arrive at simple art having higher aesthetic value than complex, unpredictable art 
  
  
## 2.3 Simplicity in Aesthetics More Conretely

 - examples of simplicity in society include simple design patterns in building and everyday objects, simple traffic rules, simple greeting protocols <br>
   societies abandon simple principles only when really necessary (which is the definition of preference)

 - examples of simplicity in art include symmetry in painting, recurring motives in music, simples harmonies in music, reduced colour schemes in painting, abstract art <br>
   cf. the more Picasso progressed in his career, the more reduced his painting of human anatomy became

 - simplicity need not be absolute but may be conditioned on expressiveness ("given that I want to express X, what is the simplest way of doing so")
 
 - simplicity may be in the details or in the very basics, hence "hidden" from the viewer <br>
   e.g. a drawing of Donald Duck may seem rather complex but is "behind the scenes" based on very simple circular and elliptic shapes


# 3. Simplicity and the Computer

- in the mathematical perspective, objects are simple if there are short descriptions which allow their exact reconstructions (analogy: a cake vs the recipe which was used to make the cake; some cakes look very complicated and fancy but actually have simple recipes and vice-versa) <br>
  crucially, this notion of simplicity can be reproduced in computer science (i.e. mathematics) (because programs, i.e. binary strings, are really just descriptions ("recipes") of objects) => the simplicity of an object is equal to the length of the _shortest_ computer program which can reproduce it (goes under the fancy name of Kolmogorov complexity)
  
- simplicity (and the length of programs) is in fact one of the central subjects of computer science and has brought influential results to the field
  
- simplicity is very closely related to patternedness: objects are simple if they exhibit highly regular, patterened structure (e.g. by repeating the same simple pattern over and over) and not simple if they have a lot of random aspects to them <br>
  e.g. an Escher drawing is simple, a Pollock painting is not simple

(- on a technical note, unfortunately, there is no program to calculate the shortest program which can reproduce an object, so the simplicity of objects cannot be directly computed)

- (BUT:) simplicity can be very easily approximated in practice by off-the-shelf compression programs, such as gzip etc <br>
  apart form the philosophical appeal, this aspect makes the theory of aesthetics as simplicity very appealing because of its convenience


## 3.1 Additional Notes
- simplicity can be conditional: different observers may find the same object differently simple because of their individual previous experiences <br>
  crucially, this aspect can be captured in mathematics/computer science => I won't go into this now



# 4. Measuring the Aesthetics of AI Music

- got 450 MIDI samples from vNine, our own music AI & 200 human songs from the Eurovision Song Contest from the past years, also in MIDI format

- (load songs into Python and) simply compress them with a few off-the-shelf compression algorithms (literally 5 lines of code) 

## 4.1 Measuring Aesthetics by Simplicity Seems to Capture something

  [LISTEN TO SAMPLES]


## 4.2 Human Music is more Aesthetic

  - what: distribution over complexity (compression) values 
    -> 0 means not complex, i.e. very simple
    -> values range between 0 and 1, i.e. can be seen as a percentage (values are bound to be well below 0.5 because anything above would be more noise that non-noise which isn't music)

  - human music is skewed towards


  - human music is measured to be less complex than AI music [SHOW DISTRIBUTION]
  
  - slightly ambivalent news: good since human artists are better but also disappointing since our art is not very complex
  
  - was however to be expected: with our simplicity preference, we produce simple songs within the space of all possible songs <br>
    although not surprising this fact alludes to the mirror effect our project aims at

## 4.3 The Music Space

  [DISCUSS 3D SPACE EMBEDDINGS]



# Miscellaneous Notes



### More Wittgenstein

- according to W., creative inventions don't break with all of the old rules but still adhere to the great many of them <br>
  => objection to why creativity exists even in experts' output 


### More Mathematics

 - the other way around: aesthetics as a principle in selecting theories and proving 
    => choice of theories or proofs (often) done by aesthetic value when indistinguishable otherwise 
    => simple (and therefore more aesthetic) objects/events/theories are more likely (to be correct, cf. overfitting) according to most theories of complexity, cf. also Occam's Razor 
    
    
### More on vNine
    
 - applying automated aesthetic measurements/judgements to the music produced by/with our Neural Net fits into the agenda of using AI as a mirror for ourselves: <br>
   it is arguably impossible for us to explore certain areas of the musical space, but this can be done with the help of our Neural Net; the measured aesthetic value of music in such areas and our own subjective judgements in comparison shed light on our aesthetics and taste 
   
   
 - agency and aesthetics: assigning agency to our Neural Net in connection to the fact that we do not quite understand its inner workings implies that we do not have a clear conception of the Net's aesthetic and need to figure out empirically what that is and how closely it matches ours

 - even with an AI-based tool, aesthetic musical pieces do not come for free but evolve out of a feedback process that takes much tweaking <br>
  => this is notable insofar as one may expect otherwise: since the Net is quite literally trained to the "rules" (cf. Wittgenstein) of music, it could be expected that its outputs are trivially aesthetically pleasing => samples of pieces during that evolution <br>
  => could be seen as a drawback: because a lot of tweaking is required to obtain something acceptable, one could argue that the Net's aesthetic is our own




# Papers

Wittgenstein: Lectures and Conversations on Aesthetics, Psychology and Religious Belief

[Bertin-Mahieux et al. (2011) The million song dataset](https://www.researchgate.net/profile/Paul_Lamere/publication/220723656_The_Million_Song_Dataset/links/0c96053bffb4d84a17000000.pdf)

### Computer Science: Theory

[Scha & Bod (1993) Computational Esthetics](http://www.remkoscha.nl/compestE.html)

[Schmidhuber (1997) Low-Complexity Art](https://www.jstor.org/stable/1576418)


### Computer Science: Applied

[Lopes & Machado (2019) Complexity Analysis of Escher’s Art](file:///home/valentin/Downloads/entropy-21-00553-v2.pdf)

[Gucluturk & van Lier (2019) Decomposing Complexity Preferences for Music](https://www.frontiersin.org/articles/10.3389/fpsyg.2019.00674/full#B36)

[Sbert et al (2007) Conceptualizing Birkhoff's Aesthetic Measure Using Shannon Entropy and Kolmogorov Complexity.](https://www.researchgate.net/publication/220795251_Conceptualizing_Birkhoff's_Aesthetic_Measure_Using_Shannon_Entropy_and_Kolmogorov_Complexity)

[Zhang et al (2018) Computational aesthetics and applications](https://link.springer.com/article/10.1186/s42492-018-0006-1)


### Anthropology

[Root-Bernstein (2002) Aesthetic cognition](https://www.tandfonline.com/doi/pdf/10.1080/02698590120118837?casa_token=nCwE7JTHehIAAAAA%3ABJ2R18heLYCmz81awLugrNfWeiezkTlxhHZXDyJ_AeH_76tR5WPxtTitM0ww_UaiksO_3fuO81_tew&)

[Christenson (1979) ON THE VIRTUES OF SIMPLICITY: SOME COMMENTS ON STATISTICAL ANALYSIS IN
ANTHROPOLOGY](https://www.jstor.org/stable/pdf/25667524.pdf); only cited by 7 papers that seem unrelated, so may not be the best source

[Ingham (2007) Simplicity and Complexity in Anthropolgy](https://www.emerald.com/insight/content/doi/10.1108/10748120710735220/full/html#idm46027260810752)
