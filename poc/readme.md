# CWF Proof-of-concept

## Overview

An application this complex, you don't want to try writing it in its final form all at once.

This project is a prototype of Cloud Workflow Foundation. It should contain:

* a CLI application that scaffolds a basic workflow application
* a module of that application that allows me to add the necessary cloud components to the workflow for a simple application with one use case.
* a frameword (SDK) that, when run, provides the ligatures between the described components to enable the workflow and a REST API gateway for triggering the steps of the workflow.
* a module of the framework that creates a UI for kicking off the workflow and performing basic tasks via the web.
* a workflow application that is scaffolded by the CLI and describes the workflow described below

## Proof-of-concept workflow

The proof of concept workflow describes the following parts.

* Any authorized user can upload a text file to storage.
* If the user who uploaded the text file is not an author, the text file must be edited by a proofreader.
* All text files must be approved by an approver.

## Limitations

* This is a POC prototype. It should be built to be thrown away.
* At least initially, CWF should be able to work in parallel with Terraform. It should not duplicate any terraform features.
