ios-bdd-bootstrap
=================

Quickly set up an iOS app for BDD development.

## What's Included

* [Cedar](https://github.com/pivotal/cedar) testing bundle with example specs
* [Frank](http://www.testingwithfrank.com/) acceptance testing with example feature spec
* [Pivotal Core Kit](https://github.com/pivotal/PivotalCoreKit) helpers for `Foundation` and `UIKit`

## Getting Started

1. Clone the repository, update the submodules, and bundle

        git clone git@github.com:joemasilotti/ios-bdd-bootstrap.git
        cd ios-bss-bootstrap && git submodule update --init --recursive
        bundle install
        
1. Frankify your app

        frank setup
        1

1. (Optional) Update the project name, organization and class prefix

## Running Specs 

* Using cucumber to run Frank feature tests

        frank build
        cucumber Frank/features/my_first.feature
    
* Using Cedar to run unit tests in Xcode
  1. Manage Schemes: `Menu Bar` -> `Product` -> `Schemes` -> `Manage Schemes`
  1. Select `Test` from the left bar
  1. Click the plus sign at the bottom
  1. Select `Specs`
  1. Run with `CMD-U`
 
## To Do
1. Create root level `Rakefile` to run Cedar specs and Frank features
1. Create script to change project name, organization and class prefix
