Transcript
We've been publishing our packages to NPR, but one really big factor that is missing is the lack of

a changelog.

If we make changes, we want this to be really easy for the people that depend on our libraries to understand.

So to achieve this, we could manually control our change locks.

But that's a really tedious process.

So what we want to do is follow a specific committee format and based on that, we would be able to

dynamically generate a change lock.

Now, the convict format would be using this called conventional commis, and it's a really popular

format in the developer community.

So you could check this out.

You could search for conventional commits.

And I think this was started by the Angola team back in the days, so this is a really useful website

to give you more information, but this is a basic format that the comments are going to follow a type.

This could be a feature fix, break and change an optional scope.

Maybe you worked on a specific package in the money repository.

That would be the scope.

Or maybe you worked on that or documentation.

That could be a good scope.

Then the description would be a small description of the change you make the optional body a full description

of the changes you made and a future that might contain some better information.

This could be an issue number that the specific committee results or something like that.

Now, we could only write this.

So in our editorial before we want to commit, we could get committed message and write out the format.

But it's going to be really tedious and the onboarding for the team is going to be hard.

So we do not want everybody to go through that stress.

So what we are going to do is install a package called Committee then.

And this is a package that can help us commit using a small interface, making it really easy to understand.

So Fresh begins at Def Con meets IZAN.

And also remember, we want to follow the standard code, conventional comments.

So we are going to install a package called Conventional Changelog for Committees.

And this is going to and this is going to follow conventional comments.

But like I mentioned, conventional comments.

But like I mentioned, we can derive changelog from conventional comments.

So that's a Win-Win.

Now, if we want to install this as a good package, we have to add the dash w flac that we youngbloods

that it's not for the workspace, but for the top would.

And once that's done, installing the next step is in our application, Jason, we need to configure

committees and to use this convention or committee format.

So in the parking lot, adjacent config and have chametz season.

And this configuration would have a path to the name of the conventional comedy format, so there are

other formats and committees and can take in the name of the format and then follow that convention.

So we are using the conventional chametz format in this case.

So get statures.

We have that.

So now we want to commit we can just one Yahn committees and but let's just add a script to make that

easier.

So I'm going to add and this is going to run Yahn Ghiz.

Sees that now if you check the Mojo's bin, you'd realize that there's a new CIA installed called Gates

sees it, and this is from the committee's library.

OK, so one thing that would prompt the interface for us to come in, so get statures, we would add

everything and then would want to commit.

So first of all, it's going to us what type of change does this feature fix Dark's refactored performance

test in this case?

We are going to just check in Dock's what is the scope of this change?

I'm going to skip that for now.

A short description at committee, then provide a longer description if you want any breaking changes

in this case.

Nor does this change affect any open issues.

If it affects an issue, then you would provide the idea of that issue on GitHub and it would be able

to link to that specific issue, and that's finical.

So here we are going to add no, it does not affect.

And you can see the committee's done.

So if we check the gridlock, you'd realize that we have Docs Calon at commission and that's great.

So when our team is working together on a project, we want to make sure that it follows a specific

committee format.

And when it's time for us to generate a changelog sings the whole team is following the same committee

format will just extract all of the chametz, get the specific information from there and use that to

generate a changelog.

We'll talk more about that in later versions.
