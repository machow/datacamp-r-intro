
---
title       : Basic R
description : Something about variables and data structures
attachments :
  slides_link : https://dl.dropboxusercontent.com/u/22292695/0c-rbasics.pdf

--- type:VideoExercise lang:r xp:50 skills:1
## Install R and Rstudio

*** =video_link
//player.vimeo.com/video/160766949




--- type:NormalExercise lang:r xp:100 skills:1
## Vector basics (1)

Create a vector named "zipcode" with 5 elements, each one a digit of Princeton's zip code (08540)

*** =instructions
- more instructions here

*** =hint
- use the `c` function, for example..
- `c(1, 2)`

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}

# vector with Princeton's zip code
zipcode <- 

```

*** =solution
```{r}

# vector with Princeton's zip code
zipcode <- c(0, 8, 5, 4, 0)

```

*** =sct
```{r}

test_function("c", not_called_msg = "you didn't call the `c()` function!")

test_object("zipcode")

test_error()

# Final message the student will see upon completing the exercise
success_msg("Good work!")
```


--- type:NormalExercise lang:r xp:100 skills:1
## Functions (1)

Check the class of "zipcode", and assign it to the variable `zip_class`.

*** =instructions
- more instructions here

*** =hint
- `zip_class <- ` is the beginning of assigning a variable
- use the `class` function

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}

zipcode <- 83201

```

*** =solution
```{r}

zipcode <- 83201

zip_class <- class(zipcode)

```

*** =sct
```{r}

test_function("class", not_called_msg = "you didn't call the `class` function!",
                       incorrect_msg = "did you pass `zipcode` to the `class` function?"

)

test_error()

# Final message the student will see upon completing the exercise
success_msg("Good work!")
```


--- type:NormalExercise lang:r xp:100 skills:1
## Strings

Write the string `Strings have "quotes" around them`

*** =instructions
- more instructions here

*** =hint
- Remember that there are two ways to write strings.

*** =sample_code
```{r}


```

*** =solution
```{r}

'Strings have "quotes" around them'


```

*** =sct
```{r}

test_output_contains('"quotes"', 
    incorrect_msg="string does not match"
)

test_error()

# Final message the student will see upon completing the exercise
success_msg("Good work!")
```





