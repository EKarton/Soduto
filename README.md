# Soduto

## What is it?

Check it on [soduto.com](https://www.soduto.com)

## Building

* Install [Homebrew](https://brew.sh/):

    `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

* Install `libtool` and `automake` using Homebrew:

    `brew install libtool automake`

* Checkout Soduto repository with dependent submodules: 

    `git clone --recurse-submodules https://github.com/soduto/Soduto.git Soduto`

* Open project `Soduto.xcodeproj` with XCode
* Change your signing team to your own personal team in `Soduto > Signing & Capabilities > Sudoto` and `Soduto > Signing & Capabilities > Sudoto Browser`
* Build target `Soduto`

## Debugging

* To see logged messages of Release build of Soduto:
    * Open `Console.app`
    * On Action menu select "Include Debug Messages"
    * In Search field enter "process:Soduto category:CleanroomLogger"

* To switch logging level in `Terminal.app` run command (with `<level>` being an integer between 1 and 5):

    `defaults write com.soduto.Soduto com.soduto.logLevel -int <level>`
