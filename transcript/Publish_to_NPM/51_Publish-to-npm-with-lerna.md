Transcript
Let's talk about publishing packages to NPM, NPRM is the most popular NPM package registry, a registry

is a sort of library that saves all of your packages to specific users.

We also have a gun registry that's a guitar registry.

And you can also create your own local registry or private registry for your company.

In this case, we want to publish to NPM because it's the most widely used and we can also host our

private packages for our internal use on NPM.

So get started by accreting on account of free accounts.

You can sign up.

Then I'm going to sign into my accounts.

And one stone on your dashboard, since we are using scoped packages and school packages, are those

that have the added bubble slash then the name of the package.

So does this scope right here that cannot specify that the package is not a lone wolf and is under a

specific organization.

So since we have a package called ADD that we would need to create an organization on the NPM website

that matches the scope that we npm those that any packages we publish with this prefix is actually supposed

to go under that scope.

So to do this, we can visit our dashboard and click on ADD organization.

The name of my organization is going to be study.

So obviously you're going to have to change your name because I have taken this organization.

Then I will click on unlimited public repositories and create.

OK, that's actually it, I could invite more team members, but that's all I'm going to do for now.

And you can see I have a new organization right here, so I have no packages on that, this organization.

But we'll get to that.

So that's the first step to publishing your packages on NPR.

Now we are using Bernhardt's manage our repositories.

So the process of publishing our packages is going to be slightly different.

Now, to publish a package to LPM, you could actually just visit your terminal on 1pm login to log

into your account and then you want NPM published to publish that package.

But in this case, we have three packages and we can do that for every individual package.

And when we have 12 to 15 packages, we really can keep doing that.

So we are going to use Lerner to publish our packages.

Now, the first thing we need to do is to learn of the scope of the packages, because by default,

when a package is on an organization, NPM would assume that it's supposed to be private.

So to each package.

So let's go to the foundation in the package to Jason.

We are going to add a publish config and said the access to public that we learn and NPM know that this

is a public package next would go to the react package adjacent, do the same thing, and finally I

would go to the access package to Jason and do the same thing.

OK, so now we've designated these as public and notice that we did not set the playground package to

public because we want this to be private.

It's just a playground for testing.

We also want to add private.

True.

And what would happen is Luna is going to completely ignore this wind population, but it's going to

bump its version privately now when we are using Lerner to publish all of these packages.

It's going to control the version numbers so we do not have to worry about that.

So the version number here is going to respect the version number in the not adjacent file.

OK, so we are ready to publish with NPM, but before we do that, we need to log in so our own NPM

logging, provide my username and provide my password.

And finally, provide my email for my account.

And now I have a message that says I'm locked in so we can run, you can learn to publish, to publish

all the packages.

So the first thing we need to do is make sure we follow semantic versioning now semantic versioning

respects a specific convention for publishing our packages.

If we are releasing a major version, then we are going to increment the first part of our version.

No, if we are releasing a patch, which means it does not have any breaking changes and it's just a

tiny fix in a repository, then we would have the last number of our version, no incremented.

And finally, if it's a minor version and might or might not have breaking changes, we are going to

increment the middle one.

OK.

So it really depends on the change that we are trying to publish in this case is our first time publishing

so we can choose if we want to release a major version or a minor version, it doesn't really matter

much.

But some people always start with a minor version as their first version.

So our select minor, then it would show us the changes.

So it detects the changes for each repository and shows us the new version.

For example, the foundation is going to have zero point 1.0 as the new one.

So it's changing the version that is specified there to match the one that we specify in alternate Jason

and notices that the playground is set to private because of our configuration, which means it wouldn't

publish.

So it says, are you sure you want to publish these packages?

And our answer is yes.

So it takes its time.

Communicates with guitar sings We have git repository set up, and now we have the packages successfully

published and that's it.

Now there's a number of things that you need to know.

First of all, if we want to get stutters, you would see no changes.

And if we check the Leonarda Jason, you would see that the version has changed.

So it's changed and it's committed the code.

So if I check the jetlag, you'll realize that there's a new comet called zero point one, point two.

So it creates a comet with a specific task for this release.

So this is version zero point one point zero.

And that's great.

Now, the second thing you need to remember is I've already added my origin, so I use git remote at

Origin to add my origin to the repository.

Now, if we want a remote show origin, then you would be able to see the remote of my repository and

they need to be able to push through my repository so that I can automate that process for me.

Now I'll visit the repository.

So GitHub dot com slash.

But could as large as yesterday e.

And now if you check out the repository, you'd realize that there's one sock right there, and if we

revisit the tax for this repository, you'll see that it was tied to version zero point one point zero

two minutes ago.

So this is everything that we at those behind the scenes.

Now, let's visit AMPM and give this page a refresh.

You'd see that we have three new packages, each of them at zero point one point zero, we have one

for the foundation, the success and the react, and that's it.

We have three fresh packages on NPM and we can search NPM to see that our packages are actually life.

And that's really good.

OK, thank you very much for watching.
