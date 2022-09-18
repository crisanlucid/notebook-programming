Transcript
Let's try some automated tests for our components in the packages we are put out into that.

And first, we need to install the packages we need for first we need just and would also install the

types for just.

That would be our testing framework.

Next, we would need Bubu.

Precent envy, and when she used TypeScript and just to write a test score for test group to work with

Jess, we need Babbo.

So would install Babo.

Preset typescript.

And since we are right and we actually installed bubble.

Parishad react next for testing, libraries will install, testing, libraries, slash, react and testing

library.

Suggests the.

Installing.

OK, so once it's done in Starling, we need to create a just configuration file, so that is that config,

the jazz file, and in here I'm going to export a just configuration.

First, we want to define the roots of our project.

And in here we have just one huge.

So we'll get the directory source.

Next, we want to define the.

Rejects use to find our test, so in this case, we would find all files that have the test and INTs

or TSX.

Finally, we need a set of files.

So this would be such a force after in the.

And I'll pass in the Woods directory and would have just set up the seats for.

And this fire would be executed after the involvement has been set up.

So just to set up the case and in this file, we want to just imports import testing, library slash.

Just do that way, it extends the just expect given us some more helpful and intuitive assertion methods,

then we need a bubble configuration so that bubble control spiral to test.

So we'd have a bubble.

That conflict just would also export a config.

In here, the first thing we want to find is our presets, so the first said we want is the bubble slash

preset N.V..

And we need to get a version of JavaScript that would support all the features we need in this case,

just to get the current version of note, and you need to have a really recent version of notes so that

it supports all the features, like a single page arrow functions and things like that.

I'm working with node version 12, so I'm going to go next.

I would add Bubu slash preset typescript.

And also at Bubu, slash presets react.

OK, that should be all we need to add a test now, how would we structure our test in this case?

We already have a folder for each component.

So in here, I'm going to add select dots, spec, dot, dot, CSX, and this is where our test would

live.

Now, remember the Gest config?

This should be the test.

I think I have to rename that to the test.

OK, so in here, the first thing we want to do, just as a test is to import, react and select components

that we are going to test then would also import render.

Form testing library reacts.

So our first guest, let's just test that it renders all options pastorate.

So it's really important that if we pass in three options, then other three options available in the

dropdown.

So first, let's get Consed and you will do and other select.

And let's just get some default props, for example, the Konstanz options would be equal to some default

options.

Maybe we should visit our playground slash index and get our default options from there.

And then OPEC is here and now we can pass in options into options and from this method we can get.

By wall, so get the get all by room method and in us select every last item, has a wall of menu item

review so we can get all by that wall and expect that there should be three of them.

So let's expect that gets all by wall.

Menu item Widjojo.

Should have left off three or we should say should have plenty of options that left.

OK, so now to run as just us, we haven't added any scripts, so that's viscid package to Jason and

then we would add a test script and this would one just verbose so that I can see clearly what test

cases there are.

Now, we can also want to watch mode.

So I could test watch and this would onion test in what mode?

For now, let's run one test.

And it feels, of course, why, because it can find an accessible element with the goal of menu item

REIJO, we obviously have to make sure we click on the button.

So what we are going to do is, first of all, find the button and then click on it and then expect

to see all those items.

So to click on the button, yeah, I'm going to get by test iji.

And we can visit the select and give this button a data test that we can use to find so here this would

be G.S. Select Button.

And now in our test, we can pass in, get by test DGSE, select Boxun.

Now, we need to click on this so we can get the fire events from TESTIN Library and fire the events

on this fire event or click.

Get by test iji so not we are clicking on it, we'll run our test again.

And great, we have a successful test, so what happens if the elements are not rendered?

Let's visit the select and let's say something happens and this does not return the correct thing.

It returns.

No.

What happens then?

We will not test.

And great artist feels says it couldn't find those elements, and that's really good because artist

is supposed to give us the security we need.

OK, so Cledus of.

And that's the basics of writing says for a select component.
