# Project Description

**Postman CLI Testing — API test collection for a Library/Books service**

I built this collection to practice writing and running Postman tests for a REST API from the command line, covering the full CRUD flow for a books resource plus a couple of user endpoints against reqres.in.

## Problem

I wanted hands-on practice with Postman test scripting beyond just sending requests manually: writing assertions for status codes, headers, response time, and response body/schema, and running the whole thing as a repeatable suite instead of clicking through requests one at a time.

## Approach

- Started from Postman's own "Library API Reference" onboarding collection and extended it with a working books API (GET list, GET by id, POST, PATCH) plus GET/POST user requests against reqres.in.
- Wrote test scripts under each request using `pm.test` and `pm.expect` to check status code, status message, headers, response time, and response body values/types.
- Ran the collection through the Postman CLI/Newman to execute all requests and their tests in one pass and review the pass/fail results.

## Tech Stack

Postman, Postman CLI (Newman), JavaScript (pm test scripts), reqres.in as a public test API.

## Status

Personal practice project — not a maintained API test suite. See [README.md](./README.md) for the collection layout and how to run it.
