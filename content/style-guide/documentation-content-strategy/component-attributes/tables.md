---
pcx_content_type: reference
title: Tables
---

# Tables

Tables make complex information easier to understand by presenting it in a clear structure.

{{<Aside type="warning">}}

Limit tables to three columns (or four if the information is very condensed). Otherwise, mobile users will have a hard time consuming tabular information.

{{</Aside>}}

## Use cases

Use tables for:

- Simple mappings of data and values
- Categories of things with examples
- Collections of things with different attributes

## Usage

We use standard Markdown tables for our documentation.

### Example

| Category | Range |
| ---- | ---- |
| **Not computed** | Bot scores of 0. |
| **Automated** | Bot scores of 1. |
| **Likely automated** | Bot scores of 2 through 29. |
| **Likely human** | Bot scores of 30 through 99. |
| **Verified bot** | Non-malicious automated traffic (used to power search engines and other applications). |

```txt
---
header: Markdown table
---
| Category | Range |
| ---- | ---- |
| **Not computed** | Bot scores of 0. |
| **Automated** | Bot scores of 1. |
| **Likely automated** | Bot scores of 2 through 29. |
| **Likely human** | Bot scores of 30 through 99. |
| **Verified bot** | Non-malicious automated traffic (used to power search engines and other applications). |
```

### Guidelines

When using tables:

- Check whether the tables work for both desktop and mobile users.
- Limit tables to three columns (or four if the information is very condensed).
- Avoid long sentences or information that is so dense that it defeats the purpose of having tabular displays.

### Alternatives

If your information does not fit within the [guidelines](#guidelines), consider using the following methods of presentation:

- Lists
- Subsections
- Tabs

### Large tables

As stated in the [guidelines](#guidelines), we generally avoid large tables in our documentation.

However, if you have a unique use case, use the `{{</*table-wrap*/>}}` shortcode to make your table responsive and scrollable.

{{<table-wrap>}}

| Header 1 | Header 2 | Header 3 | Header 4 |
| --- | --- | --- | --- |
| test | test | test | test |

{{</table-wrap>}}

```txt
---
header: table-wrap example
---

{{</*table-wrap*/>}}

| Header 1 | Header 2 | Header 3 | Header 4 |
| --- | --- | --- | --- |
| test | test | test | test |

{{</*/table-wrap*/>}}
```