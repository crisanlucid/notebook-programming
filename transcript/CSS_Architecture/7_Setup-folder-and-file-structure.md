Transcript
Of the football codes yesterday.

And this is where all the source code would exist.

I'll start by creating an exercise folder which would contain all of the stars for our project.

Keep in mind that we are going to extract this into a separate NPM package to be reused across all teams.

So whatever decisions we make should be geared towards that goal.

In here, we are going to have our source for the that would hold all the source code and we are going

to have a global success for this file is going to contain global configurations that are required for

any team using the design system in the source code.

I would also have a foundation folder.

This is going to contain the style guide for our design system.

If we visit our example design system and check out the Stargate, you'd realize that here we have the

grid, the typography, color palette and some sizes.

So when the design system is given to you by a designer, that's most likely going to be something that

closely relates to this, that defines the fundamentals of the system.

So this is where we would have our foundation.

Some people call this abstract is up to you and your team.

Now, in here, we are going to have some files would have on those colors that success where we would

define all of our colors for the system.

Next would have typography.

That success for the typography of the project next would have variables that success.

Now we are going to define reuseable variables here so that we would use this on our atoms, molecules,

organisms.

And this would also export the possibility of rewriting our size variables for anyone using the design

system.

Now, one more important thing the foundation is going to have is make sense of success and we are going

to have common system functionalities in this file.

For example, a mixin that can make it easier for us to define responsive stars.

Now, that's what our foundation is going to have in.

The source would also have atoms and would also have molecules, would also have organisms.

When we want to start a bottom component, for example, in the atoms would create the button that says

on style it and if that component was a molecule, it would go higher and so on.

That's the basic structure of our design system.

First, we have the global dot file, which would contain things like CSFs resets to completely reset

the project so that it's ready for our design system.

Then we have the foundation folder which contains the clause that says, and all of this is going to

come from our design, the typography, reusable variables for our project and make sense for reusable

functionality.
