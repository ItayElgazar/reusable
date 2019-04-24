---
id: intro
title: Introduction
sidebar_label: Introduction
---

## What?

Reusable is a library for reusing state and business logic.

## Should I use this now?

This is a very early stage alpha. You can start experimenting with it and share feedback.  
It works. but don't use it for production, yet.

## Why do we need Reusable?

Reusable solves the problems that state management is meant for, with a simple and clean API, inspired and based on React hooks API.

React hooks introduced new ways of thinking about state and side-effects.
These new ways made old habits obsolete, and require a new type of state management tool that embraces the same concepts:

- Separation of concerns
- Reusability
- Composability

While still providing the developers with structure and architecture with large-scale apps in mind.

## Features

- managing shareable state
- handling side effects
- memoization
- reactive (subscription)

## Design guidelines
- immutability
- reusability (duh)
- performance
- predictability
- encapsulation (for shared libraries / lazy loading)
- gradually adoptable

# Commonly asked questions

## What about Context API?

Using Context API directly, introduces a few challenges. Deciding where in the component tree to put a certain Context is tricky, and also might change while building your app. It forces you to couple the data tree with the component tree. It might also create a deeply nested component tree with a new provider for each provided context.  
Reusable tries to solve these issues by decoupling the reusable state from the component tree, and by providing other benefits, such as:
- Time Travelling
- Single Store
- Compound Selectors
- Structure

## Is Reusable designed for large apps?

Reusable is built with large-scale apps in mind.
This is what affected most of the considerations when designing the solution:

- The benefits of a single store and immutable data
- The ability to do code reuse using custom hooks to prevent code duplication
- Supporting DevTools for better debugging & QA
- Support lazy-loaded modules


# Feedback:

https://goo.gl/forms/Jza0XsM7F3shvWhD2

# What's missing:

- Tests
- DevTools
- More Docs
- More Examples
  - lazy-loaded modules example
  - API requests
  - Keyed states
  - 3rd party
  - Redux integration
- Time Travelling
- TypeScript Support
- Better error messages