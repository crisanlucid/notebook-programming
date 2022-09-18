Lecture thumbnail
0:14 / 5:05
Transcript
In my experience, when you have a foundation as one of the packages in your design system, it's highly

recommend that you have some tests to make sure that it does not unintentionally change.

With time for this, I recommend adding some just snapshot tests so that when the CIA is running, it

could pick up any changes that are on the Internet.

So first, in the foundation package, we need to add some just configuration for the test.

So just the config digests.

And even though the workspace installed just globally right here is highly recommended to add just to

your pocket adjacent, just in case you want to move the foundation out of the repository, the list

of dependencies should be available.

So I would.

Into packages, large foundation then I would add, just and types, just in fact, basically all of

these packages that are needed except the testing libraries, because the foundation just needs some

just snapshots.

We also do not need the Riak present.

OK, so that's installing the just configuration is going to exports.

And objects, and in this case, we do not need any set of files or anything like that, all we need

is the declaration and a regex for the test.

So here the wood is your source and test regex is going to be six.

Next, we need a probable configuration to work with just so bubble conflict or just is going to be

almost exactly like what we have here.

So we could either copy this and paste or we could modulate on exports.

Because you require and would require from the react bubble that config file, and this makes the bubble

configuration reusable across projects.

Now you can move this to the root of your mono repository so that it's reused across many packages.

But I always hold back on doing that until it's actually required for maybe four or five packages.

OK, so now in the package that Jason, we need to add a script.

This would be test and this would one.

Just so for the test, I would open the source folder and add on the score on the test folder.

And in here I would add a font size that.

Test.

Yes, and I have to make sure that actually matches the test rejects I have here, so I do not want

an empty test.

So I will test a snapshot of form sizes.

And now I would wonder, just using my Yantis common.

And it looks like everything is working, just is able to run those types of tests.

So we want a snapshot of the Fonzi.

So I'm going to import font size.

From site.

And I'm going to expect.

Font size, too much snapshot.

And the snapshot is written now, I would do the same thing for spacing.

Then I would copy the contents from here and import speccing.

OK, so one that so he takes the snapshot and now we have two snapshots written in our snapshots folder.

So it has a shape or object representation of what these frozen objects should look like.

Now, if we want to run all the tests in our projects, we can add a script to our base repository and

this would be test and this can run Yahn learn run tests.

And so let's go back into the woods and try to run test.

This should one from both packages and endorse.

I think I should add, the verbals flag to the foundation also so that it kind of gives perspective.

When you're looking at the test from S.I, it gives you perspective on what best run and more details

about it.

OK, snapshots of font sizes when well, same for these and clear description of all the tests, that

one here.

OK, so that's what I recommend running for your foundation, JavaScript.

Just a basic snapshot that makes sure that it does not change unintentionally.

I also recommend using your config packages by requiring them.

And if you have to change something from the Bible, you can always export an object and spread the

default and overwrite what you need.
