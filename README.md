# ruby-installfest

Today is our first day working with **Ruby**! Here's what we need to get started!

### What do we need?

To get started, we need a version control software (like **NPM**), and a runtime developer console (like **Node**).

### Removing RVM (in case you have it)
**RVM** is another popular version control software, but we'll be using [**rbenv**](https://github.com/rbenv/rbenv). These two are completely incompatible, so we'll have to make sure to remove all traces of rvm in case we have any.

Type in the following commands to remove rvm, and follow in the instructions with each command.

```sh
cd ~
rvm implode
gem uninstall rvm
ls -a
rm -rf .rvm
rm -rf .rvmrc
```

Once this is done, all traces of RVM should be erased.

### Installing RBENV

The installation process for RBENV is relatively simple (paraphrased from the documentation):

1. Install rbenv.

```sh
brew install rbenv
```

2. Set up rbenv in your shell, and follow the instructions to set it up in your shell.

```sh
rbenv init
```

3. Close your terminal window and open up a new one for your changes to take effect.

4. Verify proper installation with this rb-env doctor script:
```sh
curl -fsSL https://github.com/rbenv/rbenv-installer/raw/master/bin/rbenv-doctor | bash
```

5. Install Ruby 2.6.3
```sh
rbenv install 2.6.3
```

This may take a little while, so be patient.

### Installing Pry

After we've installed our version of Ruby, and our Ruby version control manager, it's time to install our runtime developer console. Ruby already comes with **IRB**, but [Pry](https://github.com/pry/pry) has several advantages to it.

Installing Pry is as easy as installing the gem:

```sh
gem install pry
```

Once you've installed, you can enter the console by typing `pry`.

```sh
pry
[1] pry(main)>
```
