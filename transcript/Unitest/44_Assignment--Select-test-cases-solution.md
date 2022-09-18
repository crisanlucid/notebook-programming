Transcript
Let's go through the test cases from the assignment.

First, we need to test that when a customer in the options is passed in, then it should be used to

display the options.

So to do this first, we are going to mount the component and we are going to pass in a custom, render

options.

So render options is going to be to function.

This comma shouldn't be here.

And this would return an ally with a detailed test iji.

Of custom render.

Option now, I think this is flogging because we have to receive some props and it should be render

option, OK?

That seems to look good.

So first we rent the element with a detail tested.

So here we could actually receive option.

And then.

When option dot label.

OK, so by doing this, we are also testing that when the option passes in some props when arranging,

so the first thing we do is to get all.

I tested, so if this rendered correctly, then we should have three options with this customer and

the option to test it.

So I expect to get all my test iji for the customer and the option that you have loads of options that

lenth.

OK, so if we check the test, I think once Fien.

So cannot find an element by nature tests iji strange, LED's Dymock.

So called a Duboc method to see the state of our dome at this point, and we can run only this test.

Of course, select is not open at this point, so I'm going to get by test.

And I'm going to fire an event to open the Butson.

And now if we want to test.

Everything passes, but we have this red arrow that sees each element should have a unique key, so

I'm just going to get recommended fops.

And then spread the recommended props.

And now there's no error because the recommended fops contains the key.

Now, we might want to test a couple of things, like making sure that the right folks are passed to

this element, for example, clicking on the customer and the option and making sure that it actually

selects.

But I'll leave that to you.

Next test we have is to make sure that the on option selected pope is called.

So I would run this test in isolation, then I would copy this render.

And then I'll pass in a prop called On Option Selected, and this would be a just function.

So for us to be used as just function I'm going to see on option selected is a quote suggests the function

and I would pass in.

This is the problem, so now we need to fire a friend or click on the button, so copy this line and

do the same thing.

Next, we need to select an option.

So I would get all by one and then click on the first one so I would fire events.

Start, click.

Get all by war and the war is minorites average, you and I will get the first one.

So I'm firing an event on the first one so we can get the book at this point and see the state of the

dome.

And if you look at the state of our dome, notice that the text in the bottom is now the name of the

first select element, and that's great because it's selected.

So at this point, we want to see that our mock function was called because we successfully selected

an element.

So we are going to expect on options selected to have been caught with.

Options first, so let's see if that's the case and we have a feeling test because it was called with

the option on the index and that's what we expect.

So we would pass zero as the first index because we are clicking on the first item.

We are also expecting to receive the first item here and the first index.

OK, awesome, that passes.

Clean this up.

And our next test is to make sure that the bottom level changes to the selected option level and we

can pretty much duplicate all of this test.

And then we move this assertion and this prop because we don't need it, but in this case we are having

a click on the button and on the first element.

So now we can expect.

Get buy test tested, so would get the button.

And then we are going to expect you to have text content options, zero dark label, no future contest,

that's great.

If we go back to the select and for some reason the button does not render the correct text.

Test fails and tells us that it's not the correct thing and that's good.

OK, so now we have a snapshot test left.

We need to take a snapshot of the component when an option has been selected.

So we are pretty much going to copy this.

And then we are going to get the Sparkman's method and we expect this to match a snapshot.

OK, so that one takes a snapshot.

So let's look at the snapshot.

And if you see the snapshot right here, you can see that the text for the Butson is the first selected

option and there is nothing else, which means the model or the menu is closed.

So we want to take another snapshot in this case, the base state, which means we wouldn't be clicking

on anything.

So I'm just going to move this and delete these two and we can take a snapshot of this.

And if we update's OK, so we have the second snapshot, so let's check this out.

So the second case is the.

Bass states, so the bass state has please select an option.

And no menu items displayed, so we also want to take a snapshot of the open stage, so we are going

to copy pretty much everything here except clicking on the menu item so that it doesn't lose the menu.

And we can also get rid of this method.

And if we check our chest.

Great, so let's check our snapshot and it would be at the top, so we have please select an option

and then we have the other list.

You can see the list items right there.

And that's really great.

It means this works.

So we have snapshots for all our three cases and also some other tests that would be really interesting

to add, for example, is to make sure that we can customize the label of the select.

So we should probably add that so tests can customize.

So that label.

And what we would do is render the component as usual and would pass in a labor text.

This is a cost labor.

And what we want to do is get the method called get by text and would expect to get by text.

This is a custom label that should be in the dorm.

And now if we check our chest, that's great.

So for some reason, if the select does not render the correct label, maybe it was put in place select.

And we check our tests, are tests breaking because it can find.

Let me read that text, but now if we pass in the real label, we have a successful test, and that's

good.

The whole point is for the test to give us security.

So there are many, many more test cases that you might want to write.

And I highly recommend right into as much test coverage as possible, because this is a reusable component.

If it breaks, it breaks all of the packages that depend on it.

Also, a final note on testing keyboard events.

This is almost impossible to do because Jazz Dome, which is the fake dome library we are using in our

test, does not support all of the native keyboard events.

So I highly recommend manually testing this as much as possible in the browser, automating this with

something such as Perpetua, which is a full fledged browser.

In any case, we've heavily tested this in the browser and this should give us enough confidence.
