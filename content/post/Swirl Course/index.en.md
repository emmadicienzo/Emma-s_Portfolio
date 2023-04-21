---
title: "Swirl Course"
author: "Emma DiCienzo"
date: 2023-04-20
categories: ["R"]
tags: ["R Markdown"]
---


# My Swirl Course 
The swirl course I decided to create was a Beginners IPA course that teachs the user about using the International Phonetic Alphabet (IPA) for the English language. In this course, there are three lessons. The first lesson is on English consonants, and here, the user learns how to classify English consonants, as well as the IPA symbols for the consonant sounds. The second lesson is on Enlgish vowels, and here, the users learns how to classify English vowels, learn the IPA symbols for each vowel sound, and learn the diphthongs used in English. The final lesson is on transcription, and here, the user gets to put their knowledge to the test by practicing transcribing some English words. 

The purpose of this course it to help first year students enrolled in LINGUIST 1A03 practice and learn about the IPA. This course is a great tool for them to study for both their quizzes, midterms, and exam in a fun and interactive way. It will also help them become familiar with R programming, in preparation for their upper year courses! 

This course is also open to anyone who isn't in LINGUIST 1A03 and just wants to learn about the IPA for fun!


# Here is the code I made for the English consonants lesson: 

```{r, echo=TRUE, eval=FALSE}

- Class: meta
  Course: Beginners IPA
  Lesson: English Consonants
  Author: Emma DiCienzo 
  Type: Standard
  Organization: your organization's name goes here
  Version: 2.4.5

- Class: text
  Output: Welcome to the first lesson of the IPA for Beginners Swirl Course! In this lesson we will be learning about English consonants!
  
- Class: text
  Output: The goal of this first lesson is to help you learn the manner, place, and voice of each English consonant, as well as its corresponding IPA symbol.
  
- Class: text 
  Output: It is important to remember that consonats are classified according to how they are produced. There are three ways to classify them; first is voicing, second is place of articulation, and third is manner of articualtion. 
  
- Class: text 
  Output: First, let's learn the different places of articualtion. 
  
- Class: text 
  Output: There are 8 places of articulation that English consonants can be classified as. They are bilabial, labiodental, dental, alveolar, post-alveolar, palatal, velar, and glottal. 
  
- Class: text
  Output: Bilabial sounds are produced by pressing both lips together. Labiodental sounds are made by pressing the top teeth and bottom lip together. Dental sounds are produced by placing the tongue between the top and bottom teeth. Alveolar sounds are made by placing your tongune at the ridge right above and behind your top teeth. Post-alveolar sounds are produced by placing your tongue slightly behind the alveolar ridge. Palatal sounds are made by bringing the tongue body up close to the hard palate. Velar sounds are produced by placing the back of your tongue up agianst the velum. Glottal sounds are produced by the larynx. 

- Class: text 
  Output: Now onto the different manners of articualtion. 
  
- Class: text 
  Output: There are 6 manners of articulation that English consonants can be classified as. They are stops, naslas, flaps, fricatives, approximants, and affricates.
 
- Class: text
  Output: Stops occur when the airflow is completely obstructed. Nasals occur when the airflow in the mouth is obstructed, but air is allowed to flow through the nasal cavity. Flaps are like a stop because it has a complete obstruction of the vocal tract, but the obstruction is so short that air pressure doesn’t build up. Fricatives occur when you hold the articulators close together and allow air to flow turbulently through the small space. Approximates occur when you bring your articulators close together but let the air flow smoothly. Affricates are a combination of a stop followed by a fricative.

- Class: text
  Output: Finally, a consoant can be either voiced or voiceless. 
  
- Class: text
  Output: Now that we have reviewed the basics, lets start learning the IPA symbols for each English consonant sound!
  
- Class: text
  Output: We will first begin with the stops.
  
- Class: text 
  Output: In English there are 6 stops. They are [p], [b], [t], [d], [k], and [g].
  
- Class: text 
  Output: Both [p] and [b] have the same place of articulation, which is bilabial. [p] is voiceless, and produces the "p" sound in words like peach, tap, and apple. [b] is voiced, and produces the "b" sound in words like ball, about, and rib.

- Class: text
  Output: Both [t] and [d] both have the same place of articulation, whcih is alveolar. [t] is voiceless, and produces the "t" sound in words like till, internet, and night. [d] is voiced, and produces the "d" sound in words like dog, adore, and kid.

- Class: text 
  Output: Both [k] and [g] both have the same place of articulation, whcih is velar. [k] is voiceless, and produces the "k" sound in words like cave, luck, and ticket. [g] is voiced, and produces the "g" sound in words like give, and bring.
  
- Class: text 
  Output: Now that we have reviewed the stops, let's test your knowledge!
  
- Class: exact_question
  Output: How many English consonants are classified as stops? 
  CorrectAnswer: 6
  AnswerTests: omnitest(correctVal=6)
  Hint: The answer is an even number.
  
- Class: mult_question
  Output: Which of the following stops are voiceless?
  AnswerChoices: p;d;g
  CorrectAnswer: p
  AnswerTests: omnitest(correctVal= 'p')
  Hint: Say the sounds outlound and place two fingers on your vocal coards. If you feel them vibrate, then the sound is voiced, if you don't then the sound is voiceless.

- Class: text_question
  Output: What is the articulatory description for the IPA symbol [k]? 
  CorrectAnswer: voiceless velar stop
  AnswerTests: omnitest(correctVal='voiceless velar stop')
  Hint: Remember when writing your description, write the vocing first, place of articulation second, and manner of articulation third.
  
- Class: mult_question
  Output: Which stops have a palce of articulation at the alveolar?
  AnswerChoices: k and g;p and b;t and d
  CorrectAnswer: t and d
  AnswerTests: omnitest(correctVal= 't and d')
  Hint: These sounds are produced by placing your tongune at the ridge right behind your top teeth.

- Class: mult_question
  Output: Which stop produces the "b" sound in the word ball?
  AnswerChoices: b;p;k
  CorrectAnswer: b
  AnswerTests: omnitest(correctVal= 'b')

- Class: text
  Output: Now let's move onto the fricatives. 
  
- Class: text 
  Output: In English there are 9 fricatives. They are [f], [v], [θ], [ð], [s], [z], [ʃ], [ʒ], and [h].
  
- Class: text 
  Output: Both [f] and [v] have the same place of articulation, which is labiodental. [f] is voiceless, and produces the "f" sound in words like phone, raffle, and leaf. [v] is voiced, and produces the "v" sound in words like video, above, and love.
 
- Class: text 
  Output: Both [θ] and [ð] have the same place of articulation, which is dental. [θ] is voiceless, and produces the "th" sound in words like thin, author, and wealth. [ð] is voiced, and produces the "th" sound in words like there, weahter, and breathe.
  
- Class: text 
  Output: Both [s] and [z] have the same place of articulation, which is alveolar. [s] is voiceless, and produces the "s" sound in words like celery, passing, and bus. [z] is voiced, and produces the "z" sound in words like zebra, deposit, and blues.

- Class: text 
  Output: Both [ʃ] and [ʒ] have the same place of articulation, which is post-alveolar. [ʃ] is voiceless, and produces the "sh" sound in words like shell, ocean, and brush. [ʒ] is voiced, and produces the "je" sound in words like genre, measure, and rouge.
  
- Class: text 
  Output: Finally [h] has the place of articulation at the glottal. [h] is voiceless, and produces the "h" sound in words like hill, and ahead.
  
- Class: text 
  Output: Now that we have reviewed the fricatives, let's test your knowledge!
  
- Class: exact_question
  Output: How many English consonants are classified as fricatives? 
  CorrectAnswer: 9
  AnswerTests: omnitest(correctVal=9)
  Hint: The answer is an odd number.  
  
- Class: mult_question
  Output: Which of the following fricatives are both voiced?
  AnswerChoices: v and ʒ;h and ð;ʃ and s
  CorrectAnswer: v and ʒ
  AnswerTests: omnitest(correctVal= 'v and ʒ')
  Hint: Say the sounds outlound and place two fingers on your vocal coards. If you feel them vibrate, then the sound is voiced, if you don't then the sound is voiceless.

- Class: text_question
  Output: What is the articulatory description for the IPA symbol [θ]? 
  CorrectAnswer: voiceless dental fricative
  AnswerTests: omnitest(correctVal='voiceless dental fricative')
  Hint: Remember when writing your description, write the vocing first, place of articulation second, and manner of articulation third.
  
- Class: mult_question
  Output: Which fricatives have a palce of articulation at the post-alveolar?
  AnswerChoices: ʃ and ʒ;s and z;f and v
  CorrectAnswer: ʃ and ʒ
  AnswerTests: omnitest(correctVal= 'ʃ and ʒ')
  Hint: These sounds are produced by placing your tongue slightly behind the alveolar ridge.

- Class: mult_question
  Output: Which fricative produces the "z" sound in the word calls?
  AnswerChoices: z;s;v;ð
  CorrectAnswer: z
  AnswerTests: omnitest(correctVal= 'z')  
  
- Class: mult_question
  Output: Which fricative is produced at the glottal? 
  AnswerChoices: h;f;ð;ð
  CorrectAnswer: h
  AnswerTests: omnitest(correctVal= 'h')  
  
- Class: text
  Output: Next, let's learn about affricates.    
  
- Class: text 
  Output: In English there are 2 affricates. They are [tʃ], and [dʒ].  
  
- Class: text 
  Output: Both [tʃ] and [dʒ] have the same place of articulation, which is post-alveolar. [tʃ] is voiceless, and produces the "ch" sound in words like chip, achieve, and ditch. [dʒ] is voiced, and produces the "j" sound in words like jump, adjoin, and bridge.
   
- Class: text 
  Output: Now that we have reviewed the affricates, let's test your knowledge!
  
- Class: exact_question
  Output: How many English consonants are classified as affricates? 
  CorrectAnswer: 2
  AnswerTests: omnitest(correctVal=2)
  Hint: The answer is an even number. 
  
- Class: text_question
  Output: What is the articulatory description for the IPA symbol [tʃ]? 
  CorrectAnswer: voiceless post-alveolar affricate
  AnswerTests: omnitest(correctVal='voiceless post-alveolar affricate')
  Hint: Remember when writing your description, write the vocing first, place of articulation second, and manner of articulation third.
   
- Class: text_question
  Output: What is the articulatory description for the IPA symbol [dʒ]? 
  CorrectAnswer: voiced post-alveolar affricate
  AnswerTests: omnitest(correctVal='voiced post-alveolar affricate')
  Hint: Remember when writing your description, write the vocing first, place of articulation second, and manner of articulation third.
     
- Class: mult_question
  Output: Which makes affricates different than the other manners of articulation? 
  AnswerChoices: they have double articulation (stop and fricative);they have only one place of articuation;they don't have a place of articulation
  CorrectAnswer: they have double articulation (stop and fricative)
  AnswerTests: omnitest(correctVal= 'they have double articulation (stop and fricative)')    

- Class: mult_question
  Output: Which affricate produces the "ch" sound in the word chill?
  AnswerChoices: tʃ;dʒ;
  CorrectAnswer: tʃ
  AnswerTests: omnitest(correctVal= 'tʃ')  
  
- Class: text
  Output: Next, let's learn about nasals.
  
- Class: text 
  Output: In English there are 3 nasals. They are [m], [n], and [ŋ].  

- Class: text 
  Output: All English nasal sounds are voiced. [m] has a bilabial place of articulation and produces the "m" sound in words like mill, hammer, and broom.  [n] has an alveolar place of articulation and produces the "n" sound in words like nice, sunny, and soon. [ŋ] has a velar place of articulation and produces the "ng" sound in words like singer, and wrong.
  
- Class: text 
  Output: Now let's test your knowledge on nasals!  
  
- Class: exact_question
  Output: How many English consonants are classified as nasals? 
  CorrectAnswer: 3
  AnswerTests: omnitest(correctVal=3)
  Hint: The answer is an odd number. 
  
- Class: text_question
  Output: What is the articulatory description for the IPA symbol [m]? 
  CorrectAnswer: voiced bilabial nasal
  AnswerTests: omnitest(correctVal='voiced bilabial nasal')
  Hint: Remember when writing your description, write the vocing first, place of articulation second, and manner of articulation third.

- Class: text_question
  Output: What is the articulatory description for the IPA symbol [n]? 
  CorrectAnswer: voiced alveolar nasal
  AnswerTests: omnitest(correctVal='voiced alveolar nasal')
  Hint: Remember when writing your description, write the vocing first, place of articulation second, and manner of articulation third.
 
- Class: text_question
  Output: What is the articulatory description for the IPA symbol [ŋ]? 
  CorrectAnswer: voiced velar nasal
  AnswerTests: omnitest(correctVal='voiced velar nasal')
  Hint: Remember when writing your description, write the vocing first, place of articulation second, and manner of articulation third.
   
- Class: mult_question
  Output: Which nasal produces the "ng" sound in the word song?
  AnswerChoices: ŋ;m;n
  CorrectAnswer: ŋ
  AnswerTests: omnitest(correctVal= 'ŋ')    
 
- Class: text
  Output: Next, let's learn about approximants.
  
- Class: text 
  Output: In English there are 4 approximants. They are [l], [ɹ], [j] and [w]. 
  
- Class: text 
  Output: All English approximants sounds are voiced. [l] and [ɹ] both have the same place of articulation, which is alveolar. [l] produces the "l" sound in words like lamb, chiily, and hall. [ɹ] produces the "r" sound in words like river, hurry, and star.
  
- Class: text 
  Output: On the other hand, [j] and [w] both have different place of articulation. [j] has a palatal place of articulation and produces the "ye" sound in words like yellow, and royal. [w] has a bilabial place of articulation and produces the "w" sound in words like water, and flower.

- Class: text 
  Output: Let's test your knowledge on approximants!   
  
- Class: exact_question
  Output: How many English consonants are classified as approximants? 
  CorrectAnswer: 4
  AnswerTests: omnitest(correctVal=4)
  Hint: The answer is an even number. 
 
- Class: text_question
  Output: What is the articulatory description for the IPA symbol [ɹ]? 
  CorrectAnswer: voiced alveolar approximant
  AnswerTests: omnitest(correctVal='voiced alveolar approximant')
  Hint: Remember when writing your description, write the vocing first, place of articulation second, and manner of articulation third.
  
- Class: text_question
  Output: What is the articulatory description for the IPA symbol [w]? 
  CorrectAnswer: voiced bilabial approximant
  AnswerTests: omnitest(correctVal='voiced bilabial approximant')
  Hint: Remember when writing your description, write the vocing first, place of articulation second, and manner of articulation third.
   
- Class: mult_question
  Output: Which approximants have a palce of articulation at the alveolar?
  AnswerChoices: l and ɹ;j and w
  CorrectAnswer: l and ɹ
  AnswerTests: omnitest(correctVal= 'l and ɹ')
  Hint: These sounds are made by placing your tongune at the ridge right above and behind your top teeth
  
- Class: mult_question
  Output: Which approximant produces the "ye" sound in the word you?
  AnswerChoices: j;w;l;ɹ
  CorrectAnswer: j
  AnswerTests: omnitest(correctVal= 'j')  
  
- Class: text
  Output: Finally, let's learn about flaps.  
  
- Class: text 
  Output: In English there is only 1 flap approximants. It is [ɾ]. [ɾ] produces sounds like the double t in words like butter and the d in words like pedal.
  
- Class: text
  Output: It is important to remember that flaps only occur between vowels when the second syllable is unstressed!
  
- Class: text 
  Output: Congradulations! You have sucessfully completed the first IPA lesson on English Consonants! ALl of your hardwork is paying off! Please proceed to the next lesson on English Vowels.

```

# Here is the code I made for the English vowels lesson: 

```{r, echo=TRUE, eval=FALSE}

- Class: meta
  Course: Beginners IPA
  Lesson: English Vowels
  Author: Emma DiCienzo
  Type: Standard
  Organization: your organization's name goes here
  Version: 2.4.5

- Class: text
  Output: Welcome to the second lesson of the IPA for Beginners Swirl Course! In this lesson we will be learning about English vowels!
  
- Class: text
  Output: The goal of this second lesson is to help you learn the way English vowels are classified, as well as its corresponding IPA symbol.

- Class: text 
  Output: Vowels are classified according to 4 pieces of information; tongue height, tongue backness, lip rounding, and tenseness.

- Class: text 
  Output: Tongue height refers to how high your tongue is placed and there are three ways to define this height; high, mid, and low.

- Class: text
  Output: Tongue backness refers to how far back your tongue is placed and there are three ways to define this backness; front, central, and back.

- Class: text
  Output: Lip rounding refers to if the lips are rounded or not while producing the vowel sound. If the lips are rounded, then the sound would be described as rounded. If the lips are not rounded, then the sound would be described as unrounded.

- Class: text
  Output: Tenseness refers to if the vowels are either tense or lax. Tense vowels are made with greater tension in the muscles of the vocal tract than lax vowels. 

- Class: text
  Output: A good way to help you remember which vowels are tense and which vowels are lax is to look at the IPA symbol. Those IPA symbols that look like regular English letters are tense, and the IPA symbols that don't look like regular English letters are lax.
  
- Class: text
  Output: Now that we have reviewed the classifications, lets start learning the IPA symbols for each English vowel sound!  

- Class: text
  Output: We will begin learning the IPA symbols for the front vowels. 

- Class: text 
  Output: In English, there are 6 front vowels. They are [i], [ɪ], [e], [ɛ], [æ], and [a].
  
- Class: text 
  Output: Both [i] and [ɪ] are high vowels. [i] is unrounded and tense, and produces the "ee" sound in words like see, heat, and piece. [ɪ] is unrounded and lax, and produces the "i" sound in words like pin, hit, and lick.

- Class: text 
  Output: Both [e] and [ɛ] are mid vowels. [e] is unrounded and tense, and produces the "aye" sound in words like sway, place, brain. [ɛ] is unrounded and lax, and produces the "eh" sound in words like ten, siad, and head.
  
- Class: text
  Output: Both [æ] and [a] are low vowels. [æ] is unrounded and lax, and produces the "ah" sound in words like mad, hat, and fan. [a] is unrounded and tense, and produces the "aw" sound in words like far and cart.
  
- Class: text 
  Output: Now that we have reviewed the front vowels, let's test your knowledge!
  
- Class: exact_question
  Output: How many English vowels are front vowels? 
  CorrectAnswer: 6
  AnswerTests: omnitest(correctVal=6)
  Hint: The answer is an even number.

- Class: mult_question
  Output: Which of the following front vowels is tense?
  AnswerChoices: e;æ;ɪ
  CorrectAnswer: e
  AnswerTests: omnitest(correctVal= 'e')
  Hint: Remeber, tense vowels look like regular English letters!
  
- Class: text_question
  Output: What is the articulatory description for the IPA symbol [æ]? 
  CorrectAnswer: low front unrounded lax vowel
  AnswerTests: omnitest(correctVal='low front unrounded lax vowel')
  Hint: Remember when writing your description, write the tongue height first, tongue backness second, roundness third, and tenseness fourth. Don't forget to add "vowel" at the end of your desciption!
  
- Class: mult_question
  Output: Which front vowels have a high tongue height?
  AnswerChoices: i and ɪ;e and ɛ;æ and a
  CorrectAnswer: i and ɪ
  AnswerTests: omnitest(correctVal= 'i and ɪ')
  Hint: These sounds are produced by placing your tongune at the ridge right behind your top teeth.

- Class: mult_question
  Output: Which front vowel produces the "ee" sound in the word glee?
  AnswerChoices: e;æ;i
  CorrectAnswer: e
  AnswerTests: omnitest(correctVal= 'e')
  
- Class: text
  Output: Now let's move onto the central vowels.

- Class: text 
  Output: In English, there are 4 central vowels. They are [ə], [ɨ], [ɚ], and [ɝ].

- Class: text
  Output: There are 3 central vowels that are mid vowels. They are [ə], [ɚ], and [ɝ]. 

- Class: text 
  Output: The first central vowel is [ə] which is unrounded and lax, and produces vowel sounds that are unstressed such as the sounds in words like believe, cinamon, and surround. 

- Class: text 
  Output: The second central vowel is [ɚ] which is unrounded and lax and produces r-quality vowel sounds in unstressed syllables such as the "er" sound in words like weather, and editor. This normally appears at the end of a word. 

- Class: text 
  Output: The third central vowel is [ɝ] which is unrounded and lax and also produces r-quality vowel sounds in unstressed syllables such as the "er" sound in words like bird and fur.
  
- Class: text
  Output: When determining if a vowel is stressed, try saying the word outloud like you are calling a pig. For example, try calling out the word bother like you would call a pig. The vowel sound that is higher pitched is unstressed, and the other is stressed.

- Class: text
  Output: The final central vowel is [ɨ] and is a high vowel. [ɨ] is unrounded and lax, and produces the "eh" sound in unstressed syllables that are a suffix in words like roses, and wanted.

- Class: text 
  Output: Now that we have reviewed the central vowels, let's test your knowledge!
  
- Class: exact_question
  Output: How many English vowels are central vowels? 
  CorrectAnswer: 4
  AnswerTests: omnitest(correctVal=4)
  Hint: The answer is an even number. 

- Class: mult_question
  Output: Which of the following central vowels is a high vowel?
  AnswerChoices: ɨ;ə;ɚ;ɝ
  CorrectAnswer: ɨ
  AnswerTests: omnitest(correctVal= 'ɨ')

- Class: text_question
  Output: What is the articulatory description for the IPA symbol [ə]? 
  CorrectAnswer: mid central unrounded lax vowel
  AnswerTests: omnitest(correctVal='mid central unrounded lax vowel')
  Hint: Remember when writing your description, write the tongue height first, tongue backness second, roundness third, and tenseness fourth. Don't forget to add "vowel" at the end of your desciption! 
  
- Class: mult_question
  Output: Which central vowel produces the "er" sound in the word bother?
  AnswerChoices: ɚ;ɨ;ə;ɝ
  CorrectAnswer: ɚ
  AnswerTests: omnitest(correctVal= 'ɚ')    

- Class: text
  Output: Next, let's learn about back vowels.

- Class: text 
  Output: In English, there are 6 back vowels. They are [u], [ʊ], [o], [ʌ], [ɔ], and [ɑ].

- Class: text 
  Output: Both [u] and [ʊ] are high vowels. [u] is rounded and tense, and produces the "ouh" sound in words like pool, and blue. [ʊ] is rounded and lax, and produces the "oo" sound in words like book, and push.

- Class: text 
  Output: There are 3 back vowels that are mid vowels.They are [o], [ʌ], and [ɔ]. [o] is rounded and tense, and produces the "oh" sound in words like throw, hole, and dough. [ʌ] is unrounded and lax, and produces the "uh" sound in words like bus, and munch. [ɔ] is rounded and lax, and produces the "or" sound in words like store, and corn.

- Class: text
  Output: The final back vowel is [ɑ] and is a low vowel. [ɑ] is unrounded and lax, and produces the "aw" sound in words like dog, and father.

- Class: text 
  Output: Now that we have reviewed the back vowels, let's test your knowledge!
  
- Class: exact_question
  Output: How many English vowels are back vowels? 
  CorrectAnswer: 6
  AnswerTests: omnitest(correctVal=6)
  Hint: The answer is an even number. 

- Class: mult_question
  Output: Which of the following back vowels is a low vowel?
  AnswerChoices: a;o;ʌ;ʊ
  CorrectAnswer: a
  AnswerTests: omnitest(correctVal= 'a')

- Class: text_question
  Output: What is the articulatory description for the IPA symbol [ɔ]? 
  CorrectAnswer: mid back rounded lax vowel
  AnswerTests: omnitest(correctVal='mid back rounded lax vowel')
  Hint: Remember when writing your description, write the tongue height first, tongue backness second, roundness third, and tenseness fourth. Don't forget to add "vowel" at the end of your desciption! 
  
- Class: mult_question
  Output: Which central vowel produces the "oh" sound in the word bother?
  AnswerChoices: o;u;ɔ;a
  CorrectAnswer: o
  AnswerTests: omnitest(correctVal= 'o')

- Class: text 
  Output: In addition to these basic vowels, English also has diphthongs. Diphthongs are complex vowel sounds where the tongue moves from one position to another to produce a vowel that changes from one sound to another. There are four diphthongs that English uses. They are [aɪ], [aʊ], [ɔɪ], and [ju].

- Class: text 
  Output: The [aɪ] diphthong produces a "eye" sound in words like sky, smile, and dye.

- Class: text 
  Output: The [aʊ] diphthong produces a "ow" sound in words like now, sound, and frown.

- Class: text 
  Output: The [ɔɪ] diphthong produces a "oye" sound in words like joy, spoil, and noise.  
  
- Class: text 
  Output: The [ju] diphthong produces a "you" sound in words like you, few, and cue.    

- Class: text 
  Output: Now that we have reviewed the diphthongs, let's test your knowledge!

- Class: exact_question
  Output: How many English diphthongs are there? 
  CorrectAnswer: 4
  AnswerTests: omnitest(correctVal=4)
  Hint: The answer is an even number. 
  
- Class: mult_question
  Output: Which diphthong produces the "ow" sound in the word crown?
  AnswerChoices: aʊ;ju;ɔɪ;aɪ
  CorrectAnswer: aʊ
  AnswerTests: omnitest(correctVal= 'aʊ') 
  
- Class: mult_question
  Output: Which diphthong produces the "oye" sound in the word boil?
  AnswerChoices: ɔɪ;aʊ;ju;aɪ
  CorrectAnswer: ɔɪ
  AnswerTests: omnitest(correctVal= 'ɔɪ') 

- Class: mult_question
  Output: Which diphthong produces the "you" sound in the word stew?
  AnswerChoices: ju;ɔɪ;aʊ;aɪ
  CorrectAnswer: ju
  AnswerTests: omnitest(correctVal= 'ju')  
  
- Class: mult_question
  Output: Which diphthong produces the "eye" sound in the word cry?
  AnswerChoices: aɪ;ju;ɔɪ;aʊ
  CorrectAnswer: aɪ
  AnswerTests: omnitest(correctVal= 'aɪ')  
  
- Class: text 
  Output: Congradulations! You have sucessfully completed the second IPA lesson on English vowels! You're now a master at knowing the IPA! Please proceed to the next lesson where you will get to practice transcribe words using the IPA.

```

# Here is the code I made for the Practicing transcription lesson: 

```{r, echo=TRUE, eval=FALSE}

- Class: meta
  Course: Beginners IPA
  Lesson: Practicing Transcription
  Author: Emma DiCienzo 
  Type: Standard
  Organization: your organization's name goes here
  Version: 2.4.5
  
- Class: text
  Output: Welcome to the final lesson of the IPA for Beginners Swirl Course! In this lesson you will get the chance to practice transcribing words using the IPA symbols learned in the previous two lessons!
  
- Class: text
  Output: The goal of this finallesson is to help you practice all the knowledge you learned in the previous lessons.

- Class: video
  Output: Before we begin the lesson, please type Yes to open a link that will take you to an online IPA keyboard, which will come in handy when you compelte some paractice questions in this lesson. 
  VideoLink: https://ipa.typeit.org/full/

- Class: text 
  Output: Now that you have opened the link, let's begin the final lesson! 

- Class: text_question
  Output: Write an IPA transcription for the word ant.
  CorrectAnswer: [ænt]
  AnswerTests: omnitest(correctVal='[ænt]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer]  

- Class: text_question
  Output: Write an IPA transcription for the word rain.
  CorrectAnswer: [reɪn]
  AnswerTests: omnitest(correctVal='[reɪn]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer]  

- Class: text_question
  Output: Write an IPA transcription for the word save.
  CorrectAnswer: [seɪv]
  AnswerTests: omnitest(correctVal='[seɪv]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer] 

- Class: text_question
  Output: Write an IPA transcription for the word water.
  CorrectAnswer: [wɔtɚ]
  AnswerTests: omnitest(correctVal='[wɔtɚ]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer]

- Class: text_question
  Output: Write an IPA transcription for the word bottle.
  CorrectAnswer: [bɑtəl]
  AnswerTests: omnitest(correctVal='[bɑtəl]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer]

- Class: text_question
  Output: Write an IPA transcription for the word mouth.
  CorrectAnswer: [maʊθ]
  AnswerTests: omnitest(correctVal='[maʊθ]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer]

- Class: text_question
  Output: Write an IPA transcription for the word flower.
  CorrectAnswer: [flaʊɚ]
  AnswerTests: omnitest(correctVal='[flaʊɚ]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer] 

- Class: text_question
  Output: Write an IPA transcription for the word blooming.
  CorrectAnswer: [blumɪŋ]
  AnswerTests: omnitest(correctVal='[blumɪŋ]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer]

- Class: text_question
  Output: Write an IPA transcription for the word identify.
  CorrectAnswer: [aɪdɛntəfaɪ]
  AnswerTests: omnitest(correctVal='[aɪdɛntəfaɪ]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer]

- Class: text_question
  Output: Write an IPA transcription for the word English.
  CorrectAnswer: [ɪŋɡlɪʃ]
  AnswerTests: omnitest(correctVal='[ɪŋɡlɪʃ]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer]
  
- Class: text_question
  Output: Write an IPA transcription for the word phonetics.
  CorrectAnswer: [fənɛtɪks]
  AnswerTests: omnitest(correctVal='[fənɛtɪks]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer]
  
- Class: text_question
  Output: Write an IPA transcription for the word strawberry.
  CorrectAnswer: [strɔbɛri]
  AnswerTests: omnitest(correctVal='[strɔbɛri]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer]
  
- Class: text_question
  Output: Write an IPA transcription for the word linguistics.
  CorrectAnswer: [lɪŋɡwɪstɪks]
  AnswerTests: omnitest(correctVal='[lɪŋɡwɪstɪks]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer]

- Class: text_question
  Output: Write an IPA transcription for the word articulation.
  CorrectAnswer: [ɑrtɪkjəleɪʃən]
  AnswerTests: omnitest(correctVal='[ɑrtɪkjəleɪʃən]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer]
  
- Class: text_question
  Output: Write an IPA transcription for the word undergraduate.
  CorrectAnswer: [ʌndərɡræʤəwət]
  AnswerTests: omnitest(correctVal='[ʌndərɡræʤəwət]')
  Hint: Don't forget to put your transcription in square brackets! [your_answer]
  
- Class: text 
  Output: Congradulations! You have sucessfully completed the final IPA lesson! You're now a master at transcribing words using the IPA! 

```



