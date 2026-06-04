# Web Crawler

A command-line web crawler written in Go that analyzes the internal linking structure of a website.

The crawler starts from a given URL, follows internal links within the same domain, and generates a report showing how often pages are linked.

## Features

- Crawls pages within the same domain
- Extracts links from HTML pages
- Normalizes URLs to avoid duplicates
- Uses concurrent workers to improve crawling speed
- Generates a report of the most linked pages

## Usage

```bash
go run . https://example.com
```

With a custom page limit:

```bash
go run . https://example.com 100
```

## Example Output

```text
=============================
REPORT for example.com
=============================

Found 15 internal links to /about
Found 12 internal links to /products
Found 8 internal links to /contact
```
