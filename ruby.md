# Ruby

## Installing RBENV for ruby version control

1. First install `rbenv`, a Ruby version manager with:

```
brew install rbenv ruby-build
```

2. Now we need to setup rbenv to load into terminal everytime we open terminal. Run the command:
```shell
code ~/.zshrc
```

Next, at the very bottom of this file, add the following lines:

```
export PATH="$HOME/.rbenv/bin:$PATH"
eval "$(rbenv init -)"
```

3. **Hard close your terminal and reopen.**

## Installing Ruby

1. Now install the current version of Ruby with

```
rbenv install 3.0.0
```

This command will take a while. Grab a coffee!

2. We will also need to set this new ruby version as our default version. We can do this with: 

```shell
rbenv global 3.0.0
```

**Hard close your terminal and reopen again.**

we can check this with:
```shell
rbenv versions
```

We should see an asterisk next to `3.0.0`

We can test to see if we're using rbenv by typing the command in terminal:

```shell
which ruby
```

The output should return a line in the terminal that looks something like this:

```shell

/Users/<YourUsernameHere>/.rbenv/shims/ruby

```

## Ruby packages

Let's install some useful ruby packages that we will need.

```shell
gem install pry
gem install rspec
gem install rails
```

# SQL

1. Install `PSQL` using homebrew

```shell
brew install postgresql
```

2. Start the postgres service (this will run in the background)

```shell
brew services start postgresql
```

3. Create a database with your user name

```shell
createdb `whoami`
```

> Those are back ticks! The ``whoami`` in backticks will get replaced with whatever your username is.
