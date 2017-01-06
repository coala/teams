Development Plan
================

For 0.6, we would like to make cib more modularized. Currently, cib uses
a lot from the
`dependency_management <https://gitlab.com/coala/package_manager>`__
package where we have the requirement classes. It also requires some work to
make it available to as many platforms as possible.

One of the things we struggle with is having distribution requirements.
Currently we don't treat those. We should ideally have one requirement class
for each kind of operating system, such as DnfRequirement, WindowsRequirement,
etc. and have the DistributionRequirement class treat them all generally,
by finding out the user's OS.

Cib also lacks some features from famous package managers, such as
shell autocompletion.

Roadmap
-------

- Make distribution requirements     - **Incomplete**
- Add shell autocompletion           - **Incomplete**
- Label issues correctly in the repo - **Incomplete**
- Catch EOF and keyboard interrupts  - **Incomplete**
- Add --verbose mode for debugging   - **Incomplete**
