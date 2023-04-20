---
title: "Advanced Function"
author: "Emma DiCienzo"
date: 2023-01-25
categories: ["R"]
tags: ["R Markdown"]
---



# My Advanced Function
The advanced function I decided to create was a consonant counter. Any application that needs to count the consonants in a word can benefit from using this function. It may be applied, for instance, to a program that counts the consonants in a given text or to a spelling or pronunciation app that examines the phonetics of words.

The function could also serve as a foundation for more difficult text processing jobs. It could be used in conjunction with other functions, for example, to count the frequency of a particular consonant or to find words that include a specified amount of consonants.


# Here is the code I produced to create this advanced function.

```{r, echo=TRUE, eval=FALSE}
consonant_counter <- function(word) {
  vowels <- c("a", "e", "i", "o", "u")
  num_consonants <- 0 # initialize the counter at 0
  
  #iterate over each character in the word and check if it's a consonant
  for (char in strsplit(word, "")[[1]]) {
    if (char %in% vowels) {
      #if the character is a vowel, skip to the next character
      next
    } else {
      #if the character is a consonant, increment the counter
      num_consonants <- num_consonants + 1
    }
  }
  
  return(num_consonants)
}
```


