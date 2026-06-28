# fetch-hooks-core

<p align="center">
  <img src="./logo.svg" width="65%">
</p>

<h2 align="center">The Modern Fetch Utility Library for JavaScript — Tiny, Typed, Universal</h2>

<p align="center">
  Designed for developers building <strong>Node servers</strong>, <strong>Bun scripts</strong>, 
  <strong>Deno apps</strong>, <strong>Cloudflare Workers</strong>, and <strong>Edge runtimes</strong>.
</p>

---

# 🚀 Introduction

`fetch-hooks-core` brings the ergonomics of React hooks to any JavaScript environment — no framework required.  
If you use `fetch()` often, this library gives you **reactive data**, **retry logic**, **polling**, and **concurrency tools** that feel instantly familiar.

### SEO Keywords:

fetch hooks, TypeScript fetch library, universal fetch utilities, Node fetch wrapper, Bun fetch, Deno fetch, fetch concurrency, fetch retry

---

# ✨ Feature Matrix

| Feature                        | fetch-hooks-core | Ky         | Axios     |
| ------------------------------ | ---------------- | ---------- | --------- |
| Universal runtime support      | ✅               | ❌         | ❌        |
| Hook-style API                 | ✅               | ❌         | ❌        |
| Zero dependencies              | ✅               | ❌         | ❌        |
| Concurrency control            | ✅               | ❌         | ❌        |
| Polling helper                 | ✅               | ❌         | ❌        |
| Retry with exponential backoff | ✅               | ⚠️ limited | ⚠️ plugin |
| TypeScript-first               | ✅               | ⚠️         | ⚠️        |

---

# 📦 Installation

```bash
npm install fetch-hooks-core
```

---

# 🧭 Quick Example

```ts
import { useFetch } from 'fetch-hooks-core';

const { data, loading, error } = await useFetch('https://example.com');
```

---

# 🧠 API Documentation

## useFetch()

Reactive data wrapper for fetch.

## useRetry()

Retries any async function automatically.

## usePoll()

Polling with auto-stop.

## useConcurrent()

Parallel queue processor.

---

# 🛠️ Advanced Example (Premium)

```ts
import { useFetch, useRetry, useConcurrent } from 'fetch-hooks-core';

const api = await useFetch('https://api.example.com/data');
const retryFetch = useRetry(() => fetch('https://api.com/retry'), { retries: 5 });
const { results } = await useConcurrent([() => fetch('/a'), () => fetch('/b')], { concurrency: 2 });
```

---

# ❤️ Community

If you find this useful, star the repo and share it.

# 📎 Links

GitHub: https://github.com/felaur/fetch-hooks-core  
npm: https://npmjs.com/package/fetch-hooks-core

