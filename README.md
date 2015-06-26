# Template for OneGov Cloud Python Modules

A cookiecutter template for OneGov Cloud Modules, the Seantis way.

Be sure to change the LICENSE after creating a project - GPL v2 might not be
what we want (but it is what our clients mostly request).

Based on [https://github.com/seantis/python-module](https://github.com/seantis/python-module).

# Usage

To use install cookiecutter:

    pip install cookiecutter

And create a new package with the wizard:

    cookiecutter https://github.com/seantis/onegov-module

(The result will be stored in a new directory named after the package)

# Features

The resulting package can be added to Travis and Coveralls. Just add them
with your Github Account on their websites. All config options have been set
already.

Do have a look at travis.yml once you've done that to setup automatic PyPI
deplyoments.

Also, use bumpversion to release new versions. The package has been setup
correctly already.

    pip install bumpversion

For a patch release (0.0.x):

    bumpversion patch

For a minor release (0.x.0):
    
    bumpversion minor

For a major release (0.x.0):
    
    bumpversion major

If you have setup travis with PyPI deplyoments, you can use git push --tags
to trigger a PyPI release.

# More Information

https://github.com/audreyr/cookiecutter
