---
title: Optimisations
---

# Optimisations

### Eager-load entry template

Eager-load relations on templates with an injected `entry` variable.

```twig
{% do craft.app.elements.eagerLoadElements(
	className(entry),
	[entry],
	['partners', 'partners.partner:logo']
) %}
```
