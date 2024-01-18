# Python Virtual Environments

A beginner's guide on effectively managing Python virtual environments using different tools
in Python ecosystem.

Popular Python virtual environment management options:
* [1] [venv](venv/README.md)
* [2] [virtualenv](virtualenv/README.md)
* [3] [virtualenvwrapper](virtualenwrapper/README.md)
* [4] [pipenv](pipenv/README.md)
* [5] [poetry](poetry/README.md)
* [6] [pyenv-virtualenv](pyenv-virtualenv/README.md)
* [7] [conda](conda/README.md)
* [8] [hatch](hatch/README.md)
* [9] [pdm](pdm/README.md)
* [10] [pew](pew/README.md)
* [11] [tox](tox/README.md)
* [12] [nox](nox/README.md)
* [13] [rye](rye/README.md)

## Your Choice?

It's glad that the Python ecosystem offers numerous options for managing virtual environments and dependencies. Yet, for beginners, 
this abundance may lead to the common question: Which one should I choose? 
In this section, I aim to share my experience and opinions to guide beginners to make right choices.

#### 1. Want to start an virtual environment in quick?
None could be more easy than `venv`, as it is a Python (>=3.3) built-in module, nonthing needs to be installed, just running command `python -m venv` to use it.
If you simply want to create a virtual environment for your Python project, and don't want to install third party packages for this purpose, then go for with `venv`.
As a beginner, you could start with `venv` and `pip`, where use `venv` to create virtual environment, and use `pip` to manage environment dependencies.

Please notice that `venv` does not support older versions of Python (<3.3 or 2.x), you will need to a third-party tool to help in this case.

#### 2. `virtualenv` + `pip` would be a popular option to start with.
`virtualenv` instead is an independent library to create isolated Python environments, and a subset of `virtualenv` has been integrated into the standard library under
the `venv` module. If you try to use a third-party library to manage Pyton virtual environments, then I highly recommend learning and trying with it.
Compared to `venv`, here are some advantages of `virtualenv`:
* it is faster
* it is extendable
* it can create environments for any python versions.
* it is upgrade-able via `pip`.
* it has rich programmatic API.

Besides, several other popular tools like `virtualenvwrapper`, `pew`, `tox` and `nox` are depending on `virtualenv` and build abstractions on top of it.


#### 3. Use wrappers to make virtualenv easier

`virtualenv` wrappers provide convenient commands to help create and delete virtual environments, otherwise managing the development workflow and making it easier 
to work on multiple projects without dependency conflicts.

`virtualenvwrapper` and `pew` are popular wrappers built on top of `virtualenv`, and both of the are great choices. The `workon` command is really convenient to help
switch environments when working on multiple Python projects with different dependencies.

For `virtualenvwrapper`:
* `virtualenvwrapper` automated tests run under these shells on OS X and Linux with bash and zsh. 
* Windows users need to usea separately distributed re-implementation iwth `virtualenvwrapper-win`.
* `virtualenvwrapper` is a set of shell functions defined in Bourne shell compatible syntax.

For `pew`:
* It would luanch a subshell when activating the environment.
* It is completely shell-agnostic and thus works on bash, zsh, fish, powershell, etc.
* It is invoked starting with `pew` in commands.

As a zsh user under both Ubuntu and MacOS, I personally like the command style and syntax of `virtualenvwrapper`, like `mkvirtualenv`, `rmvirtualenv`.
And I have been using it for years, there is no reason for me to switch from `virtualenvwrapper` to `pew` yet. 
But again, both of them are great, the choice depends on your work environment and personal flavor.

#### 4. Look for automated testing under multiple Python versions?

TODO:

#### 5. How do you manage multiple Python versions on your machine?

TODO:

#### 5. Do you want dependency management with the tool?

TODO:

#### 6. Just try something new with experimental features

TODO:

## Contact

If you have any question about this opinionated list, do not hesitate to contact me [@jgujerry](https://twitter.com/jgujerry) on X (Twitter) or open an issue on GitHub.


## License

This project is released under [MIT License](LICENSE)
