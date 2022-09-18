Transcript
Now we are going to have other packages, such as a library that implements our design system, maybe

a view library, as well as a library or an angular library.

Now, these libraries could exist in their own separate repositories and we manage them completely independent

of each other.

But this has proven to become problematic as the packages begin to increase.

So a really popular approach today is to use a mono repository strategy.

And most companies such as Microsoft, Google, Babo and many open source projects have found that this

skills really well.

So we are going to begin setting up our repository today.

The idea behind the repository is to kind of manage all of the packages, especially those that are

interdependent in one repository and one workspace.

So let's get started by creating packages folder.

And this is where we are going to put all of our packages.

This is because we can have other related folders.

We do not want them to be mixed with the packages.

So I would move the X into the packages folder and now we have our first package.

If we have a view library, react library, we're going to put them into this packages folder.

The next thing we want to do is at the root of our project.

We are going to initialize a new NPM project so young in age.

That's why.

And we could call this a device that is called.

But this is actually going to be private because this is not the repository we are publishing.

This is just a wrapper around our whole packages.

So the first package we need to set up our repository is called Lenno.

So Young at Def Learner and Learner is going to give us some really useful comments that can help us

publish our packages to NPM really easily commit Pooja's change locks and so much more.

So we'll use Lenat in combination with the workspaces which we'll talk about in a bit to achieve this.

OK, learn and start, the next step is for us to initialize a new Loana project would do that with

young learner in it, and if we check the node modules, you'd realize we have the bill.

And this as a learner, been right here.

And that's what we're using with young, so young learner in it is going to generate the learner, the

Jason file that we see here.

So this is going to have by default, the packages for the indicating to learn that all of our packages

exist in this folder and has a basic version.

Now we want to integrate learner with young workspaces.

So the first thing we do in the adjacent Jason of the Woods is to set the private option to true.

That we know that this is a private package that is not going to be published.

It is just a package that is going to be used to manage the workspace.

Next, we need to add some options to the package to Jason, and we'll add a workspaces option, which

would be an object and would have packages.

And this is also selling yarn.

The packages for the project and the packages here would be packages slash star.

Now, Young is going to know that we have a workspace and this is the root of our workspace.

Now, we also need to learn that we are using yarn as a workspace.

So we are going to see the NPM clients for Lernout.

Two years is young and use workspaces.

Is such a true another nice option.

I love to have with Lerner is to add stream and this is going to show some really good locks when we

start developing.

OK, so Young is actually ready to work with workspaces.

Now, I'll show you something really cool.

Now that we've configured for workspaces, I'm going to remove RF.

All the node modules, so this one at the root and the ones in the packages.

And if I refresh my editorial, you can see all of them are gone now at the root of the project, I

would warn Young.

Now, John is going to install the dependencies and there's also going to install the dependencies for

our packages.

OK, so it's done installing our refresh, my editor, and now if you check the source folder and check

the node modules, you'd realize that it has no dependencies in the node modules folder and it's using

a similar link so that it can have the bin, not if you check the node modules.

Otherwise you'd realize that all of our packages, such as Starling's, have been hoisted to this main

wood folder.

And you'd also realize that we have a package called Agitatedly and it contains our access package and

if we have any other packages in future, it's going to be at the top.

So in a workspace, Yang is going to hoist all of the dependencies from the packages that we are developing

and put them in this wood for that, that we we do not need to install one package more than once.

So if we had 10 packages here that all use Nordman, then Nordman would be installed just once at the

wood.

Now in the success folder in the package, though, Jason, we have a build script with the mono repository

setup.

Let's set up a script at the root and add a build.

And here I'm going to see John run the run build.

And this is how we can use Lerner to run a specific script in all of our packages.

And that's really cool because most all of our packages would have a build step so we can build all

of the packages at once.

So let's run this command to see what it does.

So I would one young build at the roots and it's filling.

But look at this.

It's detecting the packages we have in the packages folder and it's running young build on all of the

detected packages.

You can see it's one in one build on the success package right here.

And we have an error.

And remember, we said the packages, all the dependencies in the node modules are hoisted and now the

normalized X, as is also hoisted and builds creep cannot find it.

So we can we can you to ignore some of these packages and not hoist them, especially when it's causing

us troubles.

So in the workspaces, we are going to add a no hoist option and this option is going to take in star

star slash, normalize access.

And we are telling this to completely ignore Hoisin when it comes to this package.

Now we are going to remove our f all node modules and this is what I recommend doing, then initialize

the workspace again with yarn by running yarn.

OK, now that that's done, let's check our package, the success and let's check the dependencies in

the node modules and refresh, and now you can see that there's a normalized success in the node modules

of the access package.

And that's because we added these low hoist flag and Yahn did not hoist this package that way.

When we want to build, it's going to be able to find the normalized access that we are importing.

So that's one you can build from the roots and this should build the access package.

And you can see that it executed the common in one package, which is the exit package.

And we have a success.

And that's great.

We can build all of our packages at once even if we have 50 packages.

OK, so let's go through exactly what we achieved in this lesson.

The first thing we did is move the success folder into a packages folder.

Now, Packages is going to contain all of our packages for our design system.

For example, a package of your package is a package or an angular package or maybe just a package with

reusable utilities.

Next, we installed a package called Lerner.

And Lerner is a really cool dependency that can help us manage our mono repositories.

Mono repositories are really scalable and most of the best companies use it.

It's much more scalable than having each package in a separate repository.

Next, we generated another Jason.

And first of all, we declared that the packages for this mono repository are located in the packages

for the next.

We declared that the plans you use is young and we said we are using Yune workspaces and we also added

a stream option so that we can see some output when we want to learn the commands.

OK, now we went to the package to Jason and we added a workspaces FLAC and once this workspace is here,

Yang is going to automatically detect that this is a young workspace and it requires that we specify

where the packages are located.

And if we do not want to take advantage of hoisting, then we can exclude some packages.

And hoisting basically is a method for Yan to move all of the dependencies of all of the packages that

we have into a node modules folder that we if 10 packages are using Babbo, all the packages right here

do not need to install the Bible dependency.

But the bubble dependency will be installed just once at the root and the rest can consume it.

That's really, really cool.

But some packages such as normalized success do not have some good support for hoisting because we are

importing it using an absolute path so we can exclude these packages using the new hoist option.

Also, for a young workspace, we need to set priorities through at the root because this package,

Dodgson is not intended for publication, but for development of the workspace.

All right.

I hope that all makes sense.

Please make sure to practice this and reach out if you have any questions.
