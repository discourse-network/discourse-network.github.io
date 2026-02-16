---
# To make a news item display the file needs to be named like YYYY-MM-DD-brief-name.md, giving the date of the article in the name.
# The title, summary-image and summary-image-desc items are mandatory.
# Categories and tags are optional.
title: "Example news story"
summary-image: "/assets/images/DisCouRSE-Logo-Dark.svg"
summary-image-desc: "DisCouRSE Network+ Logo"  # Used for alt tag on the image; important for accessibility
categories:
  - category 1
  - category 2 etc
tags:
  - example tag 1
  - example tag 2
---

The page title (from the YAML front-matter above) is automatically shown as a level 1 heading.
So we should only use levels 2 and below during the article.

## This is an example sub-heading

You can use normal text, *italics*, **bold**, etc. as desired in Markdown formatting.

- Lists
- work
- too

Images may be embedded like this ![DisCouRSE logo](/assets/images/DisCouRSE-Logo-Dark.svg "Optional title displayed on hover")
