# -1. Why?

- Algorithmic Aesthetics = aesthetics of art produced by algorithms? or = aesthetic judgements by algorithms? (spoilers: in this section, it is the latter)

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
 

## 2.2 The Predictive Brain

  - there is a path from aesthetics to simplicity which is very much parallel to the one derived from Wittgenstein: the predictive brain; <br>
    a framework in cognitive science and neuroscience, the theory of the predictive brain assumes that our brain constantly predict what happens next 
    and then learns by comparing the reality to the predictions 

  - attempting to avoid uncertainty (evolution! uncertainty is dangerous), the predictive brain strives to surround itself with simple things <br>
    simple things are easier to predict, so our brain is 
  
  - if we apply this principle to those things and contexts we produce ourselves (e.g. art), then we should expect them to be simple <br>
    hence,
  
  
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

  - human music is measured to be less complex than AI music [SHOW DISTRIBUTION]
  
  - slightly ambivalent news: good since human artists are better but also disappointing since our art is not very complex
  
  - was however to be expected: with our simplicity preference, we produce simple songs within the space of all possible songs <br>
    although not surprising this fact alludes to the mirror effect our project aims at

## 4.3 The Music Space

  [DISCUSS 3D SPACE EMBEDDINGS]






