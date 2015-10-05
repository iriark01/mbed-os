# Reporting Bugs or Issues with mbed OS

Please report bugs in the individual GitHub repositories using GitHub's [issues mechanism](https://guides.github.com/features/issues/). If you're uncertain where the bug needs to be filed, please as on the [mbed forums](http://forums.mbed.com/c/mbed-os).

Please ensure that you're using the latest builds of all modules, because using old builds might cause issues. Use ```yotta outdated``` to list the submodules that might have been updated. 

If you see old versions, use ```yotta update -l``` to update your project, then try running your code again. If your bug still happens, file a bug report. 

**Tip:** More information on using yotta can be found [here](http://yottadocs.mbed.com/).

## Writing good bug reports

* Please explain the setup you're running, including your power source, in as much detail as possible.

* Don't hesitate to attach schematics of complicated setups.

* Sending photos of your setup explaining where peripherals are attached helps us to reproduce the bugs you submit.

* Please attach the output of ```yotta list``` to your bug report. This helps us identify packages and versions.

* Also attach the version of yotta itself using ```yotta version```.

* Please attach the output of ```yotta outdated``` to your bug report (unless it's empty).

* We are particularly interested in your toolchain versions and the specific versions of the development boards used.

* A good practice is to build a debug version of the software and attach the console output of the affected module to your bug report. Selected modules support multiple levels of verbosity that might require configuration changes to generate output on the debug console. We are happy to help you identifying the right settings.

* Try to iteratively boil down bugs to the smallest possible setup that reproduces the bug - ideally without depending on specialized hardware. It that's not possible, we need to know what other software is running in the background. Please be as detailed as possible.

* We might request a compiled firmware and the sources. This allows us to reproduce the bug on one of our development boards.
