# `CMPSC 302` Web Development, Week 1: Basic HTML (Lab)

* Assigned: 11 March 2022, 1:30 PM
* Due: 27 March 2022, 11:59 PM

## Finding your zen

Though folks introduced CSS just before Christmas in 1996, adoption of the language didn't pick up rapidly. While
it's hard to think of the technology _not_ being used today, there existed a time when it wasn't so wide-spread.
To facilitate adoption, developer [Dave Shea](http://www.daveshea.com/) introduced the [CSS Zen Garden](http://www.csszengarden.com/), 
a site whose goal was to prove how powerful and useful the language could be. It posed a simple challenge: 
without touching the HTML of a provided page, how many different designs could one apply to the page
using _purely changes to the CSS_. (The rules also allowed for uploading custom images, but no changes to the `index.html`
file were allowed.)

The final answer? 218 (accepted designs), though the creator admits that there were thousands of submissions.

Your team goal is to create not only one entry, but a _garden_ of entries which will rely on your developing CSS
knowledge. As a group assignment, each member of your group is responsible for an entry, but you will need to 
develop a group aesthetic -- that is, style -- toward which to create individual interpretations.

### Requirements

(As with previous weeks, we will cover content over the duration of this assignment which will fulfill requirements; not everything
will be fulfilled based on initial CSS instruction.)

Given that this assignment is a bit abstract, requirements are relatively light here, though I do require:

* A `CSS` sheet which styles at least 20 individual `elements`, `ID`s, or `class`es
  * At least `5` of these should be `ID`s
  * At least `5` of these should be `class`es
* A `CSS` sheet which uses at least `1` `position` property
* An `index.html` file which links each submission by title and:
  * Features a summary (or overview) of the group concept
  * A general statement from the group about challenges, wins, frustrations, et al.

In addition, your designs must:
* Pass W3C CSS validation
* Use a color scheme which has enough contrast to be legible to all visitors
  * There is an automated check for this in the grader

## Teamwork makes the...assignment work?

**This section contains significant assignment instructions; please read!**

### `clone` the assignment

You'll `clone` the assignment using the same process we've used so far in class. The only major difference is that, instead
of your user name at the end of your repository folder's name, you'll see a group name.

#### First steps

The first step you need to take is to make a _branch_ (that is a "parallel universe" of the repository that is your personal
universe, separate from other folks' universes) by typing:

##### Technical

###### Terminal

* `git checkout -b BRANCH_NAME`
  * where `BRANCH_NAME` should be your user name
* When you `push` later, note the [small change below](#Wrap-up) in the `Wrap-up`; it's important!

##### IDE (i.e. Atom)

(For VS Code users, your branch is in the lower left, and the `+ Create new branch` option pops up
in the `Command Palette`.)

* Once you've `clone`d the assignment, your current branch is in the lower-right of your screen
  * Right now, it should read `main`
* Click the word `main` and choose `New Branch` from the dialog that pops up
* Enter a branch name in the empty text box and press `Enter`
* You're now on your branch!

Regardless of your IDE, you will see an option to `Publish` the branch; do it! After this step, resume
your normal work by moving on to the non-technical part below. This will guide your decision-making.

##### Non-technical

Your group needs to decide on a general theme -- which can be only color-based, real-world theme based...your group gets to 
decide what your garden looks like! Note that decisions here are not limited to flowers, though you could use that as your guiding
principle. The word "garden" here should be taken to mean something more akin to "collection" than "gathering of botantical objects."
(I guess that's a kind of collection, too.)

#### Next steps

This is a collaborative assignment, which means it uses `git` in a bit differently. Some of you may be familiar with
the methods described here, others of you not. While I'll get you started, it's likely that you'll run into some issues
along the way. I will also help here, though I rely a bit on seasoned hands in the groups to try to solve smaller issues
which crop up (that's a good garden pun).

To make sure we all avoid each other's work, I'm assigning teams numbers to use as file names for their `HTML` and `CSS` files.
Each member should `copy` the `_template.html` file to a new file name based on these numbers, and do the same for `_template.css`.

|Team Name |File name range |
|:---------|:---------------|
|java6     |000-010         |
|portbernerslee|011-019     |
|flightlessbirds|020-029    |
|undeveloped webbers|030-039|
|idk       |040-049         |
|netflix.chill|050-059      |

**Make sure you are _copying_ the `_template...` files and not merely renaming them.**

For example, if I make myself an honorary member of `portburnerslee`, and I'm the last to take a number, I'd rename my templates to:
`019.css` and `019.html`.

* In the `<head>` element of your `HTML` file, substitute your `CSS` file name (e.g. `019.css`) for `_template.css`

##### Final reminders

* Recall that, to send your changes to the GitHub, you need to use `git push origin BRANCH_NAME`
  * Where `BRANCH_NAME` is the branch name you made above
* To see what branch you're on at any given time, type `git branch` in your terminal
  * For folks using `Atom`, the branch you're on will show in the bottom right corner of your screen

## Making a GitHub Pages page

Given that this is a _group_ assignment, only one of you needs to do this. **However, one of you _needs_ to 
do this.**

This assignment also requires you to make your work available via GitHub Pages. For a primer on where to find it
and how to do it:

- [ ] locate and click the `Settings` tab at the top of the screen
- [ ] from the menu at the left, select `Pages`
- [ ] locate the "Source" heading; set the "Branch" as `main`, and change the second drop-down to `/docs`
- [ ] click `Save`
- [ ] One last step: make the page _public_ by setting `GitHub Pages visibility` to `Public`
  * This step is _required_ for your HTML and CSS to pass validation!
A green box will appear at the top of the page listing the random URL that you've been assigned. This is your
URL!

## Accepting the assignment

- [ ] Using either the link posted to our class Discord or the [course schedule](https://cmpsc302.chompe.rs)
- [ ] Click the link provided for the lab assignment and accept it in GitHub classroom
- [ ] Once the assignment finishes building, click the link to go to your personal repository assignment

## "Cloning" a repository

### Using the correct download link

- [ ] On this repository's page, click the `Clone or download` button in the upper right hand corner
* You may need to scroll up to see it
- [ ] In the upper right corner of the box that appears, click `Use SSH`
- [ ] Copy the link that appears in the textbox below the phrase "Use a password with a protected key."

#### Cloning

* [ ] Type `ls` in your terminal window
* You should be in your `~` directory
- [ ] Find the folder you've made to hold class assignments (may involve `cd`ing)
- [ ] Once there, "clone" the repository using the link copied above
  * If I (the instructor) were to clone my own repository, I'd enter (your link will look different):

```
git clone git@github.com:Allegheny-ComputerScience-302-S2022/cmpsc-302-week-2-basic-style-lab-<group_name>.git
```

## Wrap-up

### Submitting the assignment/saving progress

The GitHub platform is a place to store your work. So, it makes some sense that should be able to _clone_ (download) from it, and push back (upload) to it. Here, we'll learn this second part.

- [ ] `cd` to your `~` folder
- [ ] Locate your `cmpsc-302-week-2-basic-style-exercises` folder and `cd` to it.

Once in this folder, we need to tell git that there have been changes.

- [ ] Type `git add -A` and press `Enter`
* This tells git to look through the _entire_ folder structure for new changes and "stage" them

- [ ] Type `git commit -m "YOUR COMMIT MESSAGE"` to "label" the commit
* This is typically something like `git commit -m "Fixing a typo"` -- the message in quotes should be as descriptive as possible, while still remaining somewhat short

- [ ] To send all changes to the server, type `git push origin BRANCH_NAME`
  * where `BRANCH_NAME` is the name of the branch you're working on
- [ ] At the prompt, input the password associated with the `SSH Key` you created earlier in this exercise (yesterday)

Once the process finishes successfully, we're done!
