Lecture thumbnail
0:16 / 6:35
Transcript
We are going to set up a continuous integration pipeline, so, yes, what we want to achieve on GitHub,

we have GitHub actions and this permits us to run processes in the cloud.

Now, if we want to build on our local computer, we can confirm that the build works.

But if we are working with a team of individuals, then this wouldn't be obvious to everybody.

So it's best to run these processes in the cloud that we we know that they work correctly, independent

of what local environment they are running.

And all of our teammates can collaborate on how these processes work together.

So to set up GitHub actions, since we are already using GitHub as a repository, we are going to add

the GitHub folder to our project.

And in here we can add workflows Foda and India.

We can create any GMO file we like and get would to take that as a process that it's supposed to run

now.

Yes, our aim we have about three or four important processes.

If we check our package for Jason, we have the build and we have the test.

Now, we can also do the publish on c.a, but let's go ahead and get started with the buildOn test.

So for the build, we want to make sure that our packages can build correctly.

Maybe when we want to publish a new version, we have to make sure it builds correctly and everybody

can observe and make sure that everything works as expected.

So the first thing we would do is give a name to this process and would call this build and test.

See, now we are going to get a win to run this process.

So, for example, do we want to run this every time a user opens a new poll request?

That would be a great idea so that it runs against that users bunch and makes sure that everything still

works with all the packages.

So let's stay on and let's start with a push.

And this is going to be brunches.

And the main bunch we are using is my.

That's our roots brunch where the packages are actually published from.

Now, we can also see Paul on this call request branches.

M. So whenever a request is reached against M..

This process would be run and whenever there's a push of code to master, this process would be won.

Now, the push would involve merging in a pool request or pushing directly from a local involvement.

Whatever process gets called into my state will triggered this process.

So now we have to get a win to run this process.

We need to target what this process is about.

So we need to define the jobs.

So in the jobs, we are going to define the Butte's for this job and we need to tell GitHub what operating

system to run this job on.

And ideally, this should be the operating system that your applications would run on.

And the most popular in this case is runs on Ubuntu.

So we're going to see this process runs on Ubuntu later.

So GitHub is going to provide the latest environment and one jobs on.

So the next thing is to find the steps for this job.

And the first thing for us to do is pull in our GitHub repository.

So we are going to use actions, slash checkout's at version two.

And what GitHub would do is it's going to run this action called Check-Out.

So this is an action created by GetUp!

And it's going to run this action which would clone or check out our repository into the Ubuntu system

that was just set up.

Now we have access to our system so we can go ahead and run on some other steps.

The first step would be one in here is called install dependencies.

So we need to install all of our dependencies before proceeding.

So the name of this process or this step is installed dependencies and the common good one is called

Yune.

Now, the next one is going to have a name of build packages.

And this is important so that we know that our packages can actually build.

Nothing has broken.

So for this would once again build.

Now the next step is of name, also major test.

And for this we are going to run YAHN tests and that should actually be very OK for us.

So we are testing two important things.

We can install the dependencies with no issues.

Then we test that.

We can build the packages correctly and we can also run Automator tests.

And that's actually all we need to set up get workflows.

So a really descriptive father tells GetUp what to do in the cloud.

So let's go ahead and check this out.

I would add everything and then we are going to run yankovich.

And we want to select.

CIA and we are going to see sets of GitHub actions, and for the long description, this would be build

and run tests on CIA.

So there are no breaking changes.

And it does not affect any open issues, so now I'm going to push to master and if everything works

correctly, GitHub would read this YAML file, notice that this process should be triggered when we

push the master and immediately start running our job.

So I've pushed your master.

Now we visit the repository, click on the action stop and you would notice that there's a new built

and Taci workflow down here.

So if I select that, you'd realize that our committee that we just committed right now set up GitHub

actions has created a new process and you can see it's in progress.

So let's kick into that.

And you'd realize that this process has just one job.

So let's go into that job.

So this job is called Buerge.

So that's the name right here.

And that's what you see on the left sidebar.

So you can give this whatever name you like.

Now you can have multiple jobs if you are doing different things with your repository.

So for us, it has checked out the code and you can click on every step to see the output.

You can see that it fetches the GitHub repository.

Check out to the specific Gref next.

It's installing dependencies.

OK, we can see some output coming in, right.

The.

Notice that the install dependencies step is done, it installed all of the dependencies, now it's

running to build packages step and look at that.

We have the build actually running and giving us some errors.

It says he cannot find this module.

So not just that the built step fails and once it fails, the automated test is not run and it marks

the job as field.

So if we revisit the roots of the repository, you can see that there's a Red Cross showing that the

litas comet actually.

Right.

And that's really good.

OK, so let's stop here for now.

And we are going to do bobwhite.

RCI is filling in the next.
