# Composite repository for MDEO to install MDEO and all its dependencies from a single repository

The DEV build contains the latest functionality, however this build may be unstable.

The RELEASE build contains the most recent stable build.

### Install urls

DEV

[http://mde-optimiser.github.io/mdeo_repo/develop/](http://mde-optimiser.github.io/mdeo_repo/develop/)

RELEASE

[http://mde-optimiser.github.io/mdeo_repo/release/](mde-optimiser.github.io/mdeo_repo/release/)

### Build status

DEV Build

![DEVELOP branch build status](https://travis-ci.org/mde-optimiser/mde_optimiser.svg?branch=develop)

Release Build

![Master branch build status](https://travis-ci.org/mde-optimiser/mde_optimiser.svg?branch=master)


### Repository Structure

This repository contains the MDEOptimiser maven dependencies converted from Eclipse OSGi bundles.

The repositories are organised based on Eclipse version as follows:

/repository/maven/{eclipse-version}/final/

### Updating the Eclipse version:

1. Update the repository copy path in src/build.xml:52
2. Update the target Eclipse version directory in src/uk.ac.kcl.inf.mdeoptimiser.repositories.p2.eclipse/src/uk.ac.kcl.mdeo.repository.p2.eclipse.aggr:2
3. Update the Eclipse P2 update sites in src/uk.ac.kcl.inf.mdeoptimiser.repositories.p2.eclipse/src/uk.ac.kcl.mdeo.repository.p2.eclipse.aggr
4. If required update the MDEOptimiser parent pom file to point to the newly created repository.