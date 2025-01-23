# TypeScript Type Guard Issue with undefined in string | null

This repository demonstrates a subtle issue with TypeScript's type guards when dealing with the `string | null` type and `undefined` values.

## The Problem

The `greet` function is designed to accept either a string or `null`.  If a string is provided, it greets the user; if `null` is provided, it provides a default greeting.  However, if `undefined` is passed, a runtime error occurs because the type guard `name === null` doesn't handle the `undefined` case.