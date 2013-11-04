# NPM The wizard

A web based GUI for authoring & publishing modules.

It's considered pretty easy to publish npm modules already. 
However that is not good enough. There is still github, travis,
testling, licence files, package.json's and other ceremony to 
deal with.

However thankfully this can be automated and stream lined.

## Concept

A web based GUI for writing small modules. At it's core writing
a module should be simple. 

 1. You write and export a function
 2. You write an executable example for the module
 3. You write a few test cases
 4. You cleanup the README. You publish the module. You're done.

Those are the four steps that are unique to each module you author.

## Design

![the flow](http://i.imgur.com/QJrOpWT.png)
![page 1](http://i.imgur.com/vW2n9WV.png)
![page 2](http://i.imgur.com/np2Ne2H.png)
![page 3](http://i.imgur.com/YvMLcaY.png)
![page 4](http://i.imgur.com/cZWBvwk.png)

### Wizard mode.

The GUI makes these easy. There is a simple flow of text editors,
one for each step. 

First you write or paste the implementation (from a lib folder). 

Then you change over to the example. You write the example and then execute it right there in the browser to verify your module works.

Then we move onto the tests, we write and execute them again to
verify that our module does what we want. At any point you can
switch back to fix the implementation or example.

When you feel good about the code you have you fix up the README
with some docs / motivations / jokes and then your good to go.

You hit publish and BAM, github repo is created, package.json is
created. Your tests run on travis, they run on testling, they run
on sauce. Your example gets uploaded to runnable. your module gets
published.

### Education mode.

You can also use the GUI in education mode. This is like the wizard
but we show step by step how we construct your github repo and how
we talk to all the third party services.

We have sections explaining some of the choices made and we have 
bash snippets showing how you can do all the steps from the command
line.

You can also fork the entire program and run it on your own servers
with your own opinionated defaults.

## Target audience

 - Prolific authors like @dominictarr, @substack and @Raynos want
    an easier way to publish their smaller modules with low friction.
 - Authors that are new to NPM and only have a few modules can use
    the app in education mode to see a set of recommended choices
    and techniques for authoring modules
 - Frontend developers that don't use the command line can get a
    gentle introduction to npm and modular development.
 - Reclaim useful modules sitting in lib folders. These modules are
    mostly a "will publish once I have the time" type of module.
 - Empower offline development of modules in your chromebook.
