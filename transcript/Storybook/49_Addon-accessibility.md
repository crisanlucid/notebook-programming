Lecture thumbnail
0:14 / 7:39
Transcript
Let's talk about accessibility with storybook.

We have a component like to select and we've done our best to make it accessible, but we do not currently

have any automated tests to make sure that it works as a spectator.

And we really would not be able to get this.

We can only get one hundred percent confirmation with manual testing, but Storybook provides an add

on that can check that we have the correct area attributes, we have the correct values for the area

attributes and everything is wired up correctly.

To do this, we are going to install a storybook add-on so into the packages, react and add def storybook

Adam Ali.

Now it is installed out, go into the packages, react that storybook mean, doges for and add that,

add on to my list of items next in the source molecules, select those stories that says Xfire, I'm

going to connect this component to use the add on we just installed.

Now, to do this, I'm going to import from storybook atoms and I'll import with Ali.

And this is a decorator.

We haven't talked about decorators, but I think of it as a higher order component in Storybrooke.

So it's a function that will take in our component and then modified in some way and then return kind

of an enhanced component in this case with Ali is a decorator that will take in our component, which

is a select component, and it would run as usability tests on the component and then give us the result.

So here we are exporting.

Difford We are going to export decorator's and the first one here is with Ali.

Now that we have that we are going to start a browser and see what changes this gives us.

So Donelan.

Start storybook.

I think we should have that.

Now, if we run this.

It looks good and it opens it up in the browser.

So now if we visit the select component and you see a new type called accessibility, and when we click

on that tab, you would realize that there is violations, passes and incomplete.

Let's start with the process.

So accessibility, which is the plugin that we just installed, runs a bunch of accessibility checks

on the component itself.

For example, it ensures that all buttons have to send more checks, which means that if the text of

this button was not discernible and had some contrast issues, this accessibility test was going to

fail.

And that's really, really great that we test the combination of the success and the estimate for our

component.

Now, it also has violations for those accessibility tests that feel and let's look at what field we

have and show all area attributes have valid values, which means that we have and area attribute that

is invalid in our component.

And let's check this out.

So it sees the area controls attribute has a wrong value.

Hmm.

That's really strange because we actually provided the correct value.

Right.

Wrong.

So the problem here is we provided the idea of the list, but the list is not present on the page.

Let me show you.

So in our component itself right here, if I scroll down to the body of the component, what we are

doing is we are checking if the component is open, then we are going to render the list or else we

are going to render more.

And while this is perfect for sites users, because they are just going to see it when that on the page,

it is not the best for assistive technology because the component does not exist on the dome.

But the list should be on the dome.

It should just be hidden.

So we need to change things around so that this accessibility tests can pass.

And that's one of the really big advantages of the accessibility item.

So what we are going to do is remove this and make sure that the list is always on the page, that we

the assistive technology can actually find it so that we would still be able to link the button.

And on that list, that's the first step.

But now if we visit our component, the list is always open and now the accessibility tests are passing.

What we've broken our unit test.

So what we want to do is make sure we have the best of both worlds.

We still have our functionality and we have our usability test passing.

So to do that, we are going to add a new class to the on that list if the menu is open.

So I'm going to come here.

And then I'm going to add.

A class, so we'll check, is open.

And what other class called select overly dash dash open for the open state and else we're going to

add an empty string so this class should be able to open the overlay and this class would have a default

state.

So we would visit the select that access.

And here are the styles for the overly.

So I would add a new bradsher, the iSelect overlay.

And we need to add the open state, so an open.

That should give us the correct last name, and in here we're going to see the display is block, which

means that the default states of the overlay is going to be a display of none.

So here we're going to see display none.

So when the component is addressed, then the display would be known.

And then when the is open is such a true, then this class would be added, which gives it a display

of block.

So let's run and compare our changes before we check this out in the browser.

So I'll visit the Roots and I'll run Yan.

Def.

They should compile the access and if we refresh.

It doesn't work, but let's inspect to see if the class is actually being applied.

So if we inspect the element and click on this, it applies the class.

We have the class showing up here.

But the problem is a little typo.

I have so much to the component.

I'm going to remove the stache safe and now click again.

And all should be well.

So we have the component working again, as expected, we have usability tests passing, and we should

also make sure that the automated tests are passing.

OK, so in this lesson we learned about the storybook, Ali, Adam.

And this is going to wrap our component and one usability test on the market for that component to make

sure that we have the right words right and the right values for all of these attributes.

It would also run contrast test discernible checks for the most common accessibility issues.
