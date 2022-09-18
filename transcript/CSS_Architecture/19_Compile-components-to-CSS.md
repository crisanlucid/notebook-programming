Transcript
In this lesson, we are going to be compiling our components down to success.

We just compiled the global that successful.

So we want to do the rest for atoms, molecules, organisms.

Now, this is the idea.

Let's say we have an atom with the button that says foul and we have maybe a button container.

With display aflex.

What we want to do is compound the button that successful to a library slash button that says that we,

the user, can import only those styles for a specific item or only the stars for a specific molecule

organism.

So for us, we go to our built address file and I'm going to extract this into a method called compound.

So COMPAR is going to be called a function.

That returns this dot says the string, and what this would do is it would take a path and it would

take in a far name.

So what we'll do is the path is the origin and the file name would be the destination.

So I would make this into a complete function and get results from here.

So this is the idea, we get the result and we call first, right, farseeing and we write to the output.

So this is going to be the file name and this is going to be the path.

OK, so this is a compound function and just a test that this works, we can call compound with sourceless,

large global success and sourceless Lipe slash global success.

That's the origin and that's the output.

And let's clear this up so that we know it actually works with one unbuild.

We have an error area, can I for us of the fine, let's check that there should be an error.

And that's because we are calling it here, so I would remove that and now we have resorted to string

one this again and it's done.

So that works.

Now we need to do the same thing and we need to call the compartment thought for all the molecules,

atoms, organisms.

So the first thing I would do is create a method.

First, let me delete this.

And this method is going to be called get components.

It would fetch all the components and give it to us in an hour, so let our components.

Each quarter and every then the types of components we have, the atoms, molecules.

And organisms, so this is the idea, I want to go into the atoms for the fetch all of the components

from there and push through the all components are we go to the molecules for our fetch, push them

to the other components, go to the organism's fetch, push them into the other components that we would

look through all the components and compare.

OK, so to do this, I have put the types here so that we know which food we are going into.

Then I'm going to say types that for each type.

What we want to do is Konstanz or Fous, and we are going to say fast with Directress Singh so that

we can read the order and the foda is going to be source slash type.

So if we were at Atom's, it would be sourceless atoms, molecules would be sourceless molecules, same

thing for organisms.

And when we read this is going to give us an array of all of our stuff we found what we want to do is

map through each file and return a path.

Dawid Wisoff.

For the final four now, we are going to modify the map once we know what we have, but what we want

to do is all components is equal to will spread all components and then would spread all fires.

So we are adding all the files to the component and then would return all components.

Now I'm going to console that log the result of Colin get components so that we see what we have.

That way we can debug.

So console that log, get components now with one Yambuk and you can see our first component is the

access button that success.

And that's why we need to map so that we can put the type here so that it's the correct folder and we

are going to put the resolve file, but not just file.

We are going to have SCIP and file.

And now if we want that, you can see that we have success at Tom's bottom dot success and that should

be correct.

Now, one thing we could do is instead of mapping and returning this, we could just return an object.

With input to this and then output is going to be Lipe slash the file name, but what we want to do

is slice the file names so that we remove the access and then we are going to add success.

So we remove access and we access.

So if it was a button that says it would become button access.

OK, now we want to run Bude again so that we see the log and now you can see that we have an object

input.

Is this an output is this and that looks great.

Now the final step is to loop through all the components, so get components for each component.

We are going to call compile on the component the inputs and components that outputs.

OK, so let's do this and see what we get with one young boat.

We have an error that says no such file arms change.

I think it can't find the file correctly.

Yeah, the source is missing.

So I think that has something to do with the way we resolve.

So let's check the input.

And in here, we probably want to do this instead.

Source slash type.

Slash.

Found, OK, and then the path that resolve code in the compound should do the job of finding it correctly.

So let's run this again.

We still have the same error.

It can't find the light.

And I think that's for this one.

So it should be Source Lipe.

And let's do this one more time.

And we have a success so you can see the leap forward that has a button that says and this contains

just a styles for the bottom six us.

Now we are going to be doing something like importing the foundation from the bottom as well so that

we have access to the variables.

And this would be foundation slash all I think, foundation slash.

Oh, OK.

So that we the button can have access to all of the variables declared in the foundation if we build

this just to make sure it works.

You can see the button now has all of these things, the comments, but it has access to all the variables

and we have the access right there.

OK, so that's basically it.

One final test is to create a molecule.

Maybe this would be Puno the success and would have the Jesse Puno container.

And this would have a display of flags position absolute.

And also important, the foundation slash all.

OK, so let's run our build script.

And if you check the results, you can see we have global access panel, that success and Butson, not

success.

All right.

So let's try to recap the script that we wrote in this lesson.

First thing we did is we created a compound function.

It takes in an input and an output.

It calls the Sacerdote when the sync, which gives a result and then writes the result to the output

file.

Now we call it compound on the global file so that we can compare the global success.

Then we created another function called Get Components.

And what this does is it goes into the atoms, molecules and organisms folder and finds the components

declared in that folder and then loops through each one of them maps and provides the path to the input

and the output.

Then we add that to all components and then we look through all the components and compile them that

way.

We have a light for the right here, which is the result of our source.
