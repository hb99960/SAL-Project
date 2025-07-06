# Assignment S15

## Problem Statement 1: **URL Shortener**

**Design and implement a scalable URL shortening service.**

You are tasked with building a backend system that takes a long URL (e.g., `https://www.example.com/some/very/long/link`) and returns a shorter version like `short.ly/abc123`. When a user accesses the short URL, they should be redirected to the original URL.

### Requirements:

- `POST /shorten` → Accepts a long URL and returns a unique short URL.
- `GET /:shortID` → Redirects to the original URL.
- Ensure the short IDs are **unique** and **not predictable**.
- Handle a large number of requests per second (read-heavy).
- Support analytics tracking (optional): e.g., click count, location, time.
- Ensure the system is **scalable**, **highly available**, and can handle **millions of URLs**.

---

## Problem Statement 2: **Scalable Keyword-Frequency Search API**

**Design an API to search for keyword frequency across very large files.**

You are given 50 to 100 text files, each around 50GB in size. Millions of users will query your API to find how many times a word (e.g., `"data"`) appears in total across all files.

### Requirements:

- `GET /search?word=data` → Returns the total count of the word “data”.
- API response time should be **under 50 milliseconds**.
- The system should handle **millions of API calls per day**.
- System must support **adding or updating files** dynamically.
- Normalize words (case-insensitive, punctuation-free).
- Design the system to support future enhancements like **phrase search**.
- Ensure **fault tolerance**, **horizontal scalability**, and **cache efficiency**.