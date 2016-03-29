
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

Create a vector named "zip" with 5 elements, each one a digit of Princeton's zip code (08540)

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
# The sct section defines the Submission Correctness Tests (SCTs) used to
# evaluate the student's response. All functions used here are defined in the 
# testwhat R package. Documentation can also be found at github.com/datacamp/testwhat/wiki

# Test whether the function str is called with the correct argument, object
# If it is not called, print something informative
# If it is called, but called incorrectly, print something else
test_function("c", 
                not_called_msg = "you didn't call `c()`!"
                #, incorrect_msg = "you need to give `c()` some arguments"
)

# Test the object, good_movies
# Notice that we didn't define any feedback here, this will cause automatically 
# generated feedback to be given to the student in case of an incorrect submission
test_object("zipcode")

# It's always smart to include the following line of code at the end of your SCTs
# It will check whether executing the student's code resulted in an error, 
# and if so, will cause the exercise to fail
test_error()

# Final message the student will see upon completing the exercise
success_msg("Good work!")
```
