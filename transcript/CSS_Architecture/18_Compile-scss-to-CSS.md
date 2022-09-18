Transcript
In this lesson, we are going to be compiling our SAS down success that way anyone or any team consuming

this package would simply import the compound success instead of having to deal with SARS.

They could also use us if they want, but we need to provide the access for them.

So to do this, we are going to be installing a package called LODESTARS, which is a no just package

that can compare success down to success.

Now, we are going to create a script for that in the source.

Folder and in here would have built the Jaspal.

First, in this fight, I'm going to require force so that we can read files and write files, then

I'm going to require proof.

So that we can.

Get the correct parts to files and resource files correctly.

Finally, I'm going to require source, which is no source.

So the size comes with a method called Wenda or in the sink for the sink version.

And it takes in a list of options.

First, it takes in the D.R., which is the size that we want to compare.

In this case, what we want to do is pass in AIFS, the read file sink and then would with the global

success file.

So instead of just passing global that says we are going to use path dot resolve and would pass in source

bluebottle success, that we would get the full path to this file.

Now the data is expecting a string, so we are going to call the two string method so that it passes

the result of the read to a string.

Next, we need to pass in the output style and in this case it's going to be expanded.

This could also be compressed if we want for a production build, but expand.

That is good for now.

Next, we can also provide an outflow and I'm just going to add global counts in this case.

Finally, I'm going to add a for what's called include parts.

And this tells us where to find access, for example, all of our sources in the source folder.

So we'll see path toward resolve source that we Sarcelles where to find access.

All right.

So that's a configuration.

Let's add an NPM script so that we can run this file.

And on the scripts would add build and build is going to want to source scripts, slash butut, Jess.

Now, if we want unbuild.

We have an error and this is a strange error, but I was able to look deep into it and find out what

was going on.

If you check our typography, that success, we have one font size, which is available name and it's

excess property.

Now, if you go to the node modules and search for normalized access.

You would realize that in the source variables that they have the same verbal name, but there is an

actual value and not accessed property.

So when we overwrite this variable is giving us an error because it expects this to be a number, but

it's siestas variable.

So what we want to do is in our own access, let's just use a different variable name.

OK, and this is in case you actually used this rebuilding.

And in this case, we are going to add a dash so that it's a completely different variable name and

I'm going to do the same thing for headphones.

OK, and I just realized this is text, this should be fun.

All right, so now if we want to build, we have done, which means everything is successful.

So what we want to do is actually lock the contents or write the contents of a file.

I'll show you in the script the builder, Jess, we are going to console the log.

The return from this is a constant.

Result is equal to this, and let's consider that log.

Result.

Success, because that's what the result continues.

Now, if we can build again, you can see we have a buffer we can call to string so that we get the

string.

And great, look at that, we have access locked to the console, so all we need to do is use the FA

system so that we can write this access content to a file.

Now we are going to see EFS.

The White House housing and will be right into the path door to resolve.

Source slash, lip slash global, the successful.

And the contents will be right on this result that start to stream, so the right file seeing takes

in the path to the file we want to write to.

And the second argument is the detail we want right to that file.

OK, so Cledus, then I would have to create the LEAP folder so that it's available.

Then I'm going to run this script again and.

And then check the live folder and great, we have a global access, so in this file you'll realize

that we still have a comment because we are compiling an expanded mode then if you check.

Right down at the bottom, we have the normalized success storage, for example, we have H.M.S. Body

article and all the defaults start next.

If we score right down to the bottom, we have our roots starting and that's from our route.

That successful notice that it declares some default success variables for the route.

OK, so in this lesson we wrote a basic script that can compile signs down to the size package has Arenda

Sink method, which takes in the data that we want to compile as a string.

Then it takes in the output style which could be expanded or compressed.

Then it also takes into include parts so that we can tell us where the X Files are located.

If not, it would not be able to find the foundation, slash all of the base reset or the base would.

Finally, we watch the results of that compilation to a file called Lombardozzi.

And that's what we have now.

OK, we would need to modify the script so that it compiles all of our other source files, like the

atoms, molecules and organisms.
