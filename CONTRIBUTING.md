# Contribution Guide

[![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)](https://www.tensorflow.org/)
[![Discord](https://img.shields.io/badge/%3CHALitosis%3E-%237289DA.svg?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/KgrChecyQt)
[<img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" />](./LICENSE.md)


> So, ya wanna beat HAL 9000?

## Welcome!

We're delighted that you're considering contributing to our attack framework for ML engineers and hackers in our life and death battle with Artificial Intelligence!

If you haven't already, please [join our discord](https://discord.gg/KgrChecyQt), introduce yourself and feel free to discuss any ideas for contribution - we're open to ideas and you may even find some collaborators for your own contribution.

You can find more info on our project in our wiki, issue trackers and documentation. 

## First-Time Contributors

If you would like to contribute to HALitosis but don't know where to start, you can take a look at issues labelled with the tag `good-first-issue` or [join our discord](https://discord.gg/KgrChecyQt) to speak to more experienced HALitosis contributors to discuss some ways you could help or your own ideas, we have a welcoming community that follows our [Code of Conduct](CODE-OF-CONDUCT.md).

Once you have decided how you would like to expand HALitosis, you can take a fork of the main branch and begin your work - and also follow the rest of this guide to help you write quality code for our users.

It is recommended that you develop your contribution with the use of a Python virtual environment such as `venv` or `pyenv`, for security and version tracking purposes - we also need to check which dependencies that you are using!

## Contributing to Code

If you are writing a new feature for HALitosis, we use the [Python PEP8 Style Guide](https://peps.python.org/pep-0008/) and run our code through `pylint` which can be installed with:

```sh
pip install pylint
```

We recommend that you use atomic commits (one commit per functional unit of code) and long commit messages that explain the what, how and why of your commit to fully document your code as you go:

```
Short one line title

Longer description of what the change does (if the title isn't enough)

An explanatoin of why the change is being made.

Perhaps a discussion of context and the alternatives that were considered.
```

Here is an example of one of these commit messages that help with our workflow:

```
Correct the colour of FAQ link in course notice footer

PT: https://www.pivotaltracker.com/story/show/84753832

In some email clients the colour of the FAQ links in the course notice footer was being displayed as blue instead of white. The examples given in PT are all different versions of Outlook. Outlook won't implement CSS changes that include '!important' inline[1]. Therefore, since we were using it to define the colour of that link, Outlook wasn't applying that style and thus simply set its default style (blue, like in most browsers). Removing that '!important' should fix the problem.

[1] https://www.campaignmonitor.com/blog/post/31819301/outlook-2007-and-the-inline-important-declaration
```

The flipside of this, is if you use a tool like the [GitLens plugin for VSCode](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens), you can see these kind of commit messages for previous contributors giving expansive documentation for each line of code.

Alongside atomic verbose commits, we recommend that you expand on the docs to include the new features that you've implemented which are built with `sphinx` which can be installed with,

```
pip install sphinx
```

These steps are to be taken as well as to adequately comment on your code as shown in PEP8 so that others will be able to follow your work as you go.

All tests are located within the `test` directory, we ask that you pass all tests on the `main` branch, as well as, writing your own unit tests for new features that you are adding.

## Contributing Documentation

Documentation for HALitosis is written using `sphinx` which can be installed with:

```
pip install sphinx
```

Whilst direct code documentation is always useful, its also helpful to sanitize and link-up our documentation, as well as writing tutorials for HALitosis or community guidelines to help our users get the most out of HALitosis.

## Code Review

Prior to merging your branch or fork, we will review your code to see that all new features follow our style guide, repository organization, and are properly tested and documented.

We are also busy and so we might take some time to respond or even  ask you to change some things about your contribution before we can accept it - but we are still so grateful, please be patient!

## Bug Reporting

If you've found something wrong with HALitosis and you can't find a resolution anywhere, you can open an issue with the tag `Bug` in Github's issue tab.