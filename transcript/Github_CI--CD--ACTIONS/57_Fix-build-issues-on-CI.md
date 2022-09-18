Transcript
We entered the last lesson with an error from the CIA involvement.

Now when John tries to warn the build command, Lerner runs build for the foundation and react packages.

But the real package falls on errors, saying it cannot locate the foundation package.

That's because the foundation package actually needs to build before the react package react to events.

The react package depends on the foundation package, but Lerner doesn't know that.

So the way to solve this is to specify our dependency in the real package to Jason.

So would come here and include ideas that E slash foundation as a dependency and for now we'll just

place in any version.

And what this will do is inform Lerner because Lerner would read the package, Jason.

And if it realizes that this reac package depends on the foundation package, it would build the foundation

package before the real package.

So let's add everything one year and commit.

At this as a fixed at foundation package, as dependancy to react, then I would push Origin Master,

this would trigger a beard and let's view what that beard results in.

We have the beard trigger, so let's visit it.

Visit the build job and view the results.

Now, this is good, we have a new member from the group.

You are making some progress now.

You can see how the CIA involvement is telling us that, hey, the code you had on your system works

on your system, but it doesn't necessarily work for everyone else.

And that's really good.

So at this point, what we are lacking is the leap forward for the success.

Now, if you check the script for success in the source scripts builder Jess, it puts the result in

a leap folder, but it doesn't really create a leap or for itself.

And that's a problem for other builds like bubble and roll up the create the leap if it doesn't exist.

But our custom script does not do that.

So we want to make sure it does that so that if the user clones the repository or other developers from

a team clone the repository, then they do not run into any issues, just like the CIA is running into

issues.

So to do this.

Let's add first make Directress Sync.

Path, door resolve.

Source.

Right now, this is not yet perfect, but let's go ahead and delete the LEAP folder right here.

OK, then segued into the packages, access and one young build.

OK, we have a success, even though the leap for that to not exist, which means that it's working

correctly.

Now let's try to run it when the four that exists and see if this would give us an error, it would

tell us that this does already exist.

So what we can do to make this easier is just wrap it in a try catch and with another catch.

So if there are any errors when trying to create it, we just ignore them.

So let's run this again and we have a success.

OK, so this is exactly what we want.

If a developer is cloning the repository, they shouldn't have to deal with misinformed issues.

And we also do not want to push the Lipe to GitHub because having builds on GitHub is really just heavy

and really not necessary.

We need the source.

OK, so we have the stats estranges.

We changed a script so that everything.

But we have to go back to the roots one year and commit.

This word.

Be sure.

And then these would be updates, ESCs says Bude script.

And then we would push this to muster and looking at this fire, I might be expecting a lot of arrows,

but I'm just going to push to my stuff so that I can actually tell us what these areas are.

Remember that I am working on the Mac OS computer and the CIA is running on an Ubuntu system, which

means that if there are things that actually work on my system that don't work on the boonchu, then

we would have errors.

And that's really good that way.

We write code that works on everybody's system.

Irrespective of what that system is.

OK, so let's say that actions we should have a new job.

That's it.

So let's visit the bills and watch the results.

So our next hour is it can find the organisms and the first thing is, number one, there is no organism.

So it's an empty folder on my system and that empty for days, not pushed to social control, which

means that in the environment of those organisms folder, it would fail.

And that's good.

So what we want to make sure is this ignores the organisms folder.

And when we have a new organism in our project, then we would add it there.

So the atoms and molecules are good because we have files in those folders.

OK, so we've done that.

I'm going to get at everything again.

Great comments, all yankovich.

Then make this a fix and then I would say update's.

Exos built for us.

OK, then I'll get pushed to master, so I would actually keep doing this process over and over.

So I resolve all of the issues.

So it most likely is going to be a while.

But stay with me.

OK, so now we visit actions.

Viscid, the CIA.

Viscid build.

And the job and watch for the next arrow.

Watch for the next error.

OK, this time around, our Bude went through without any issues, and I know you're surprised, I am

surprised, too, but that's really good, right?

So it shows that we can build our packages, look at success, then it also shows that we can run our

tests and that's successful and it also closes the test.

So that's really great.

We have our CIA passing and every time we make a change, we open the pool request or we push to master.

It's going to run to make sure everything still works as expected.
