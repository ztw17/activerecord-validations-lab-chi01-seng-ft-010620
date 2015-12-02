# ActiveRecord Validations Lab

# Basic Validations

Add validations to these models such that...

1. All authors have a name
1. No two authors have the same name
1. Author phone numbers are exactly ten digits
1. All posts have a title
1. Post content is at least 250 characters long
1. Post summary is a maximum of 250 characters
1. Post category is either `Fiction` or `Non-Fiction`

# Custom Validations

Finally, add a custom validator to `Post` that ensures the title is
sufficiently clickbait-y. If the title does not contain "Won't Believe",
"Secret", "Top [number]", or "Guess", the validator should false.
