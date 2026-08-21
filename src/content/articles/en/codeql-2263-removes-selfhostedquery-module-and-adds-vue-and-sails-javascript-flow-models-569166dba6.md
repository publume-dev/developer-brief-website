---
decisionKey: "569166dba6c9e6490757898d4b5f73f864a465bedc44a80820cef6b442b207d0"
language: "en"
title: "CodeQL 2.26.3 Removes SelfHostedQuery Module and Adds Vue and Sails JavaScript Flow Models"
summary: "CodeQL 2.26.3 removes the GitHub Actions SelfHostedQuery module and enhances JavaScript/TypeScript flow modeling."
publishedAt: "2026-08-21T14:06:07.365Z"
score: 0.9
topics:
  - "CodeQL"
  - "Static Analysis"
  - "GitHub Actions"
  - "JavaScript"
topicIds:
  - "codeql-crqmh5"
  - "static-analysis-14v4mof"
  - "github-actions-7tcwgt"
  - "javascript-zxjsqy"
sourceUrls:
  - "https://github.blog/changelog/2026-08-19-codeql-2-26-3-improves-github-actions-queries-and-javascript-modeling"
---

- The `codeql.actions.security.SelfHostedQuery` module is removed because runner labels don't reliably distinguish self-hosted runners from managed runners, requiring updates to custom queries. 
- New JavaScript/TypeScript flow models: support Vue's `ref`, `shallowRef`, `toRef`, `reactive`, and `computed` Composition API helpers, and recognize Vue Router's `useRoute()` as a client-side remote flow source. 
- The `actions/output-clobbering/high` query is improved to not report simple jq path filters, and a performance issue caused by unescaped regular expression input is fixed.

A future GHES release will include this functionality, but the specific version number is not provided in the changelog.
