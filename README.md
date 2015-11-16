# ActiveRecord Validations Lab

## Objectives

- Apply a validation requirement using validates macro
- Identify when validation occurs in the lifespan of an object
- Introspect on the ActiveRecord::Errors collection object on an AR instance
  - use valid?
  - use errors
- Generate full_messages for errors
- Check an attribute for validation errors
- common validation macros
  - scope on uniqueness
  - validation configuration options
- Add a custom validation error to an AR model

## Notes

Author#name uniqueness
Author#phone_number format (matches 9 numbers)
Post#title present
Post#content minimum 250, custom error message
Post#summary maximum 250
Post#category within ["Fiction", "Non Fiction"]
(what other custom validation options like :on or :if can we flex here?)

Clickbait#title present
Clickbait#content maximum 500
Clickbait#clickbait? validates :title, :clickbate, custom validation
  - must include "Top X", "Guess", "Believe", "Secret", or some clickbait algorithm

I think if we can think of a custom validation to add to Post I'm good with that but otherwise why not introduce another class to isolate the custom validation on
