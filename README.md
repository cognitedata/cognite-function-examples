# cognite-function-examples

[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)

This repository contains a set of Jupyter Notebooks showcasing the use of Cognite Functions. 

## Requirements

The code examples in this repository are written in Jupyter notebooks. In order to display and run the code, you need to install `jupyterlab` and the
Cognite Python SDK:

```shell
pip install jupyterlab cognite-sdk-experimental
```

## Authentication

For all the examples here, we will be authenticating against CDF by using Azure
Active Directory. Each notebook contains the relevant instructions.

## Example 01: Create a basic Cognite Function from a Jupyter Notebook

In this example, we deploy a Cognite Function in the simplest possible fashion,
by referring directly to a Python-function. This is sufficient for simple use
cases where your function does not rely on additional dependencies.

## Example 02: Create a Cognite Function from a folder.

In this example, we take it up a notch by deploying a function that is divided
across multiple Python-files. We deploy an entire folder containing our source
code. This method allows you to specify additional Python package dependencies
if neccessary.

We also schedule this Cognite Function to run on a regular interval.

## Example 03: Create a Cognite Function that performs entity matching on time-series and assets.

In this example, we look at something more akin to a real world use case. Here
we deploy a Cognite Function that runs entity matching on some of our assets,
mapping time-series to assets in CDF.

We also schedule this Cognite Function to run on a regular interval.
