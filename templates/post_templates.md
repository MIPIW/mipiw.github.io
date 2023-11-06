---
# every file
# static
layout: default
sidebar: mydoc_sidebar
search: include

# variable
categories: # must be length 2 list
subcategories: # optional, must be a singleton list. if no subcategory filled, it will regareded in listed page in sidebar page

title: template
date:
rank:
published_year:
author:
author_full:
keywords:
summary:
---

<!-- content file head -->

|-|-|
| Author | {{page.author_full}} |
| Published | {{page.published_year}} |
| Keywords | {{page.keyword}} |
| Importance | {{page.rank}} |

{{page.summary}}
