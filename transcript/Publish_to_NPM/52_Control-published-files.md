Transcript
Here I have an empty folder and we use this to test the packages that we just installed.

So this is what I highly recommend doing, Yahn, in it, that's why.

Or initialize a new project, then you can add your package.

So adds that E slash access adds years that E slash foundation adds that e slash reachout.

And I think the package to Jason names messed up.

I'll be name this then one to install.

All right, that's it in the latest version of each package listed in our package adjacent.

Now, what we're interested in is looking at the node modules to see what was actually shipped in the

yesterday if we have the REACT Foundation and success.

So let's look at the foundation first.

Should realize that we have the CSS config, the Jason file here.

We also have the adjust configuration, the bubble configuration and the source folder.

Hmm.

Interesting.

Now let's check the Lipford and you see that there's just one file indexed or file and it's exporting

nothing.

Hmm.

That's also interesting.

And we have all of these tests that we do not need.

That's really strange now in this package, though, Jason.

The reason why we have this lab is because Maine is listed as the main file or the main export, and

that's why it published it.

But generally, it wouldn't publish any files that I get ignored.

Now, this is our main project.

And if we check the foundation.

Get ignore, you'd realize that I'm ignoring library, and that's very important so that we do not push

compiled code to GitHub.

It's really just heavy to carry around.

What we want to do is push the source code to GitHub and then we can compare and publish to NPM.

So that's what is happening.

NPM is checking the get ignore file and it's ignoring the library folder and it's publishing just the

main file.

And if we check the react, it's doing exactly the same thing and is also publishing all of these files

that I would not care about when using the package.

Now let's check the access.

And it's doing the same thing, completely ignoring the library and publishing a bunch of source files

that would actually be important to our users if they are trying to override using access.

So let's fix this.

To fix this, we need to change a configuration in the package that Jason called files.

So in the foundation, I'm going to add a foul's value and this is going to contain Lipe.

And this means that everything in the library should be published and everything out of the library

should not be published.

So this is a white list and only files that are listed in this files key would be published to 9pm.

So the source in this case would be completely ignored.

Now, let's do the same thing for the REACT package.

So in the package to Jason, I would add a new forcefield.

And now for the access in the package to Jason, we would add the forcefield.

This would match Lipe because we want to publish our life and we are also going to add the source because

we want to actually ship the source in case the user wants to override the source that we wrote.

OK, so that's a change.

Let's go ahead and add everything.

Comi message fix files for packaged adjacent files.

Now that we've committed, we can one young learn, not publish, but before we do that, one thing

we can do is we set up adjacent at the Woods and other publish.

Come on.

And this would give us the opportunity of running again sassed, for example, and also young Bude to

make sure everything's fine before we actually run and learn, run, publish or not publish so we can

make sure everything is fine before we proceed to publish it.

So now you can run.

Publish.

And first, it's running our test.

Looks like the test passed now it's trying to build.

Looks like the beard was successful and now it's publishing, so it's going to ask what change we made.

Now we have to choose if it was a patch, which means this is just an internal change to our application

or Tyahnybok fix or change in documentation, something small like that or Manel, which means that

we are actually creating something that is impactful, a new feature, a tiny improvement or something

like that.

And the major, which means we are completely publishing a new version.

In this case, it's just a tiny patch.

Next, you can see the package that changed all of them.

And notice the playground's are listed because we didn't touch it.

So we are going to say, yes, we want to publish these packages.

It's going to create the tax.

Push to get up, push to NPM.

And it's done.

OK, so now let's come back to our test project where we are testing our application.

Then we are going to come to the package to Jason and change this to zero point one point one zero point

one point one and two point one point one, then one million to install the litas versions.

OK, that's done now let's visit the normal, just give this a good refresh, check the GST and we check

the foundation.

You'll notice that it has just a lip foda and now it has the font size, which is the actual JavaScript

that we need with the index suggests you can see that it exports or provides the whole thing and this

test should actually not be compiled.

Right.

This shouldn't be here and it's already ignored.

So that's fine.

Now, if we check the results, you see that we have the library, we have the next chance, we will

have the typescript definitions.

We have the ASMs, we have the molecules right there.

Next in the access file, we have the source with all of the sets for the atoms, the base foundation.

We also have the library with all of the access files for the individual atoms, components and global.

All right.

So that's great.

So in this lesson, we learned about the FOUS where we can control from our packages and exactly what

we want to publish to NPM.

Another thing to remember is when we are pushing to GitHub, we want to push the source and ignore the

life and we will push into NPM.

We want to push the life and ignore the source.
