## Sinatra versus Rails Exploration

### Setup:

First, clone down the Rails project:

```terminal
git clone https://github.com/turingschool/job-tracker.git rails_project
```

And then clone down the Sinatra project:

```terminal
git clone https://github.com/turingschool/bike-share.git sinatra_project
```
Now cd into each project, run `bundle` on each project, and you're ready to go. We will only be looking at the code base and not interacting with the app. If you wanted to run the server and interact with the app, you would need to create your database, migrate your migrations, etc.

### Exercise:

1. Take a look at this stripped down Sinatra app and this stripped down Rails app. How are they different and how are they similar? Identify 5 differences, and for each one describe 1-2 implications. What effect does that difference have for each framework? If you don't know exactly, draw on your knowledge and experience and make some educated guesses/inferences. Also, practice your research skills to look into the differences.
```
They both use: Capybara web-based test and ActiveRecord
Rails uses jQuery-rails, which is a fast, small, and feature-rich JavaScript library.
Rails uses JBuilder which is an integrated development environment (IDE) for the programming language Java 
Jbuilder gives you a simple DSL for declaring JSON structures that beats manipulating giant hash structures
Rails uses Spring which is a Rails application preloader. It speeds up development by keeping your application running in the background so you don't need to boot it every time you run a test, rake task or migration.
```
1. Consulting blogs and commentary you find online, identify 3 similarities between Rails and Sinatra.
```
Rails assumes you are using a database, Sinatra makes no such assumption

Rails is a full fledged web framework, including database access, a templating language to generate HTML files, routing, plugins, etc. Sinatra basically lets you respond to certain addresses by some text. 

A huge benefit of Sinatra is its stability. You trade the convenience of a few Rails generators for your own design decisions. Writing in Sinatra can give developers and businesses API stability because the framework rarely changes. You own your code and you decide when it should change.
```

1. Consulting blogs and commentary you find online, identify 3 things that distinguish Rails, advantages.
```
Rails is solving issues for you Sinatra never can, since it can make more assumptions about your application. You get everything set up for you

The Rails generators and structure provide conventions that Sinatra doesn’t.
```
1. In your Rails project, what does the `routes.rb` file inside of the `/config` directory do? What does this correlate to in our Sinatra app?
```
The routing module provides URL rewriting in native Ruby. It's a way to redirect incoming requests to controllers and actions
```

1. We teach Sinatra by adding some structures that Sinatra doesn’t need, but help you make the transition between Sinatra and Rails. What does a stripped down implementation of Sinatra look like, and what are the pieces we’ve added for educational purposes?

