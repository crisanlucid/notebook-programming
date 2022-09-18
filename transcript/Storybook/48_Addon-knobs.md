Transcript
Let's add the storybook for the color component, and you realize that it's slightly different from

the solar component and we'll talk about why in the atoms color, let's add color the stories, the

TSX file and first world import we are.

Then would import the components of.

And first, we need to export the An object with a title that sees color.

And for this to show up in the browser, we need to export one use case.

So let's just export Konstanz Common.

And this would return color.

And the Difford required Wallachia a tax code, so let's just passing pink and now you can see that

we have color.

Now you can see that color is on the and others group.

And what we do to render select on the molecules is by adding molecules in front of its name and it's

automatically going to know how to group that.

So if we want group to be on the atoms, we can just add atoms with a pipe operator and now Atoms is

in its own group.

So we have the example use case for column, but if we check the color, it doesn't show anything because

we need the success and the success we need is number one import.

Yes, that slash access library Collado access.

And we also need to isolators.

It sees the module cannot be found.

Let's make sure that module actually exists.

So SASE library.

I'm strange.

We do not have the color.

Let's check the react source code and it makes use of the width and the height and yeah.

So it doesn't have a color, it just has the utilities.

OK, so now we have a success so you can see that it's rendered in the browser, so does the little

square right there.

Now we can export more.

And so for example export Konstanz.

Custom dimensions, and this would explode the color pass in the hex code of pink, and you can see

the custom dimensions there, but we do not have any custom dimensions.

So we need to pass in the width, for example, of.

XXL and the heights of XXL.

OK, so the first one is the common, and it just has a basic with and higher than the second one is

custom dimensions with a different with and height.

And that's really good.

Now with something like this, we have the pink, which is dynamic, so we can have a red blue, a different

hex code.

But the story right now does not really demonstrate such capabilities.

So what we want is a solution where the user can play around and provide their own props to see how

powerful our components are.

To do that, we are going to be adding a package called storybook knobs.

So open a new terminal into packages.

React and Def Story.

Beaugard Knob's.

OK, once that's done.

We can add that add on to add ons, R.E. and Storable would automatically register that now in the component

itself we can import from that package and the first thing we can get is a text variable.

Now, this variable is a function, and what we can do with it is instead of parsing being statically,

we can pass in text and call it as a function under.

The first argument is the name of this purpose.

So we can see hex code and the second argument is the default and this would be pink.

And now I'm just going to start storable for my terminal so that you can re register all the add ons

and it looks like it's successful.

So if we check that out in the browser, we have this new section called Knob's and you can see that

we have hex code and we have pink.

So it gives us the possibility with Xbox because we have this text very well coming from the package,

it gives us the possibility of exiting the hex code value.

So let's say we wanted to try to black.

You can see that the component automatically renders with black and that's really, really cool.

Now let's do exactly the same thing for the case of dimension's.

And if we reset the custom dimensions, this one is really big.

We can change this to red and that's really good.

We can change this to green and that's perfect.

Let's look at the case for the width and the height.

We want to use that to be able to customize with on the height in the browser.

But we have a fixed set of values.

If not, the customization wouldn't work.

So in this case, we would import select from the add Dunlop's and we need to provide a fixed set of

values.

So for us, we would pass in select and we need to pass in aname.

This would be with and we need to pass in a set of options.

So let's say extra small, small, extra, extra large.

These are part of the possible options and the final argument is the default.

So would pass in extra extra large as the final argument.

And now if we check the browser, check out the custom dimensions, you'd realize we have a with right

there and look at that, it's a select box and the user can select whatever they want and that's really,

really good.

Now, we need to do the same thing for the height.

So I'm just going to copy.

But first, let me break this down so that it's readable and that I would copy what we have for the

height, for the width and pasted for height.

Rename this to height and we're good to go.

But then this is not all the options that are possible.

So instead of hard coding this, we can import the foundation.

From art, that E slash foundation, and what we need from here is space in so space.

And if we check that.

Contains all of the space in values, so back to our stories, we can pass in object dot values and

pass in the space in.

And now if you check the with we have all the options right there.

Now, we should do the same thing for the height, objective values and pass in the height it renders

correctly.

And we have all the possible options.

Right.

And that's really, really good.

Now we have some typescript errors.

It says the width has a problem.

We can assign string to one of these options, and that's because the foundation actually exports the

wrong type.

I'll show you, if we revisit the spacing from the foundation, you'd realize that it exports an object

without a fixed type for that object.

So I'm going to copy this object and provide it as the type.

So look at that.

The type and the object is exactly the same that we the values are of specific types, not string.

So does the known type, the X.

So this is a specific string type and this is the type in for the spacing.

And now if we visit the stories, we still have the same error, but we can run the Bude, so one young

build to build that.

And now let's check out the foundation again, if you check the space in the dots, you would realize

that the types of change, so they are no longer type string.

And now if you check all the stories, everything is good again.

So I highly recommend exporting the right types from the packages.

It's not something we've been very keen with, but the font size, for example, does the same thing.

We should probably make sure that the type is fixed like this, that we when we generate types for the

font size, it's exactly the correct thing.

OK, so in this lesson we installed a package called Add on Knobs, and this is a really nice way to

customize the props or the properties of a component that we are rendering in the browser.

In this case, we were enjoying the color component and we used the text knob to render an input where

the user could customize the hex code from.

And we use the select to render a select box where the user could select height for the rendered component.
