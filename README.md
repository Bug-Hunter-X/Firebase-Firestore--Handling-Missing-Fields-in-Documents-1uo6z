# Firebase Firestore: Handling Missing Fields

This repository demonstrates a common error in Firebase Firestore: attempting to access fields that don't exist in a document.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a robust solution.  This issue is crucial for building resilient applications and preventing unexpected crashes.

## Problem

The `bug.js` file showcases an example of trying to access a field (`city`) that is not present in all Firestore documents. This causes an error if the field is missing.

## Solution

The `bugSolution.js` file demonstrates the use of the `?.` optional chaining operator and the `||` nullish coalescing operator for safely accessing potentially missing fields. These techniques allow you to gracefully handle missing fields without causing errors.

## How to run

1.  Clone this repository
2.  Install Firebase: `npm install firebase`
3.  Configure your Firebase project.
4.  Run `bug.js` and observe the error.
5.  Run `bugSolution.js` and observe that the code handles missing fields gracefully.