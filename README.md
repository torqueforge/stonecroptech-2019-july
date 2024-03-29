# Practical Object-Oriented Design Class 2

## Dependencies

You will need:

* git
* a modern version of Ruby (2.x or greater)

## Setup

Clone this repository:

```bash
$ git clone git@github.com:torqueforge/stonecroptech-2019-july.git
```

Change directories so that you are in the project:

```bash
$ cd stonecroptech-2019-july
```

Install the dependencies:

```bash
$ gem install bundler # if you don't have it
$ bundle install
```

## Sanity Check Setup

To verify that everything is set up correctly, run the following command:

```bash
$ ruby sanity_test.rb
```

You should see the following output.
```bash
$ ruby sanity_test.rb
Run options: --seed 62459

# Running:

.

Finished in 0.001317s, 759.3014 runs/s, 759.3014 assertions/s.

1 runs, 1 assertions, 0 failures, 0 errors, 0 skips
```

## Track and fetch all the remote branches

    #!/bin/bash
    for remote in `git branch -r`; do git branch --track ${remote#origin/} $remote; done
    git fetch --all
    git pull --all
