# Expo CLI Dependency Version Mismatch

This repository demonstrates a common error encountered when using the Expo CLI: dependency version mismatches. The error arises when the dependencies specified in `package.json` don't match the installed versions in `node_modules`. This often leads to build failures during the Expo build process.

## Problem

The Expo CLI throws an error indicating a dependency version mismatch.  The error message isn't always clear about the specific conflict.

## Solution

The primary solution involves ensuring consistent dependency versions. This can involve:

* **Cleaning the `node_modules` folder:** Delete the `node_modules` folder and reinstall dependencies using `npm install` or `yarn install`.
* **Resolving dependency conflicts:** This might require carefully examining `package.json` and `package-lock.json` (or `yarn.lock`) to identify conflicting version ranges.  You might need to adjust version ranges or use specific versions to ensure compatibility.
* **Using a newer version of Expo CLI:** An outdated Expo CLI could sometimes contribute to these issues. Upgrading might resolve the conflict. 
* **Checking for typos in package.json:** Ensure all dependencies are correctly spelled and their versions are specified accurately.

This repository provides example code demonstrating the problem and its solution.