# README

clone this repo,
then "rails db:migrate"
then "rails c"
then \/\/\/\/\/

Screw around with this stuff:

        > u2 = User.find(2)
        > c1 = u2.comments.first should return that user’s comment. #comments returns an array with comments, which is why we need to use #first to actually retrieve the comment itself.
        > c1.user should return that comment’s author User (u2).
        > p1 = Post.first
        > p1.comments.first should return the comment c1.
        > c1.post should return the post p1.

If any of those don’t work, double check your associations. Sometimes the error messages can be helpful in prompting you for how to set up those associations.
