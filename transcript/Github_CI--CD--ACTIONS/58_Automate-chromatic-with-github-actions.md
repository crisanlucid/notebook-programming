Transcript
Another great thing to add to our workflow is the visual regression test with chromatic, so at the

moment, if we visit the package, Dodgson's react.

We have a command called Chromatic and it uses or or at the project token in line.

And this is not always secure, especially if you are an enterprise or working on the private company

project.

So what we are going to do is, first of all, copy this project and then visit Gizab and we set the

settings and on the settings, viscid secrets.

And we can add a new secret to the repository, so here I'm going to page the value and the name of

the secret is going to be chromatic project chokin.

Then I would add this secret, then back to my editor.

I'm going to visit the site of YAML file and I'm going to add a new step.

The name of this step is going to be visual regression test.

Now, for this step, there's something I need before I actually provide the one command, and that's

an environment.

Now, the involvement variable would be chromatic project token.

That way we can specify or we can reference the environmental can instead of the inline value we have

currently.

And this is going to be the value of those secrets from our repository DOT Chromatic Project Choucoune.

So Komati Project Tokin is the name of the secret here and that's what we assess.

So now that we've declared N.V., we can run.

The common young test chromatic now we need a command that can run chromatic from the React Packages

folder.

So what we'll do is add a good Common Core test chromatic.

And this is going to run a chromatic command from the react folder.

So in the react in the package, though, Jason, I'm just going to call this test chromatic.

And then in the woods, I'm going to say this.

Should one young learner run test chromatic?

And of course, it would run only in the packages that have this test, chromatic command.

So in here, we want to get rid of this and then add in line and we want to add in line the chromatic

token.

So I'll just copy this and pasted that.

So this is referencing the involvement that we've declared in the CFA and the involvement is getting

its value from the secrets.

And when we look at our logs, we wouldn't see the value because it's securites encrypted.

OK, so that's basically all we need, the Yantis Komachi command from the wood is going to run on one

testicle magic and in our pockets, Jason, for the relief package, we have a schematic command which

is going to run chromatic and provide the project token to be this.

All right.

So time to see this in action.

Get at everything, Yankovich.

I would say this is seet then this would be such a chromatic in envy.

I would push this to muster.

And once I pushed it to muster, it should trigger my guitar workflow and I would visit the actions

for that.

Review this.

I'll click on that.

Viscid the specific job and this should start any second.

OK, so this runs successfully.

You can see that Komachi successfully authenticates.

You can also see that it uses the project Tolkan.

But since it's a secret, you can see there's an asterisks masking the value, which is great.

Then it wants a storybook command, builds ships to take, and now we have ours because there is an

issue with the snapshots.

So a test would be able to tell us, hey, there's something wrong with the changes and you need to

review them.

So we would copy this.

Your visit chromatic and you can see that there's one on review change.

So if we click on that, you can see that it's related to the time when we did the green change so we

can go back and approve this change because we want you to go back to the normal.

So once this has been accepted, we can come back to our board and click on we want all jobs and they

should pass successfully.

OK, so what did we learn in this lesson in the settings of your guitar repository?

You can set up a secret and this secret should be the hidden token or whatever you get from a service

that runs in the cloud.

And you can reference that as an environment visible in your site or YAML found that way you do not

have to expose your tokens if you do not want your.
