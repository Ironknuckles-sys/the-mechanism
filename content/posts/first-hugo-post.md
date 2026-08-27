+++
date = '2026-08-27T11:52:15Z'
draft = false
title = 'First Hugo Post'
+++

# A site built with Hugo

Creating content with markdown in hugo is easy.

### Make a list

Favourite fruits:
1. Banana
2. Passion fruit

Static site generators I have tried:
- Astro
- Hugo
- Jekyll

### Output highlighted code

Some python code:
```python
from django.db import models
from django.utils import timezone


class Article(models.Model):
    title = models.CharField(max_length=200)
    slug = models.SlugField(unique=True)
    published_at = models.DateTimeField(null=True, blank=True)

    class Meta:
        ordering = ["-published_at"]

    @property
    def is_published(self):
        return self.published_at is not None and self.published_at <= timezone.now()

    def __str__(self):
        return self.title
```

### Display an image with figure shortcode

{{< figure src="images/hadada-ibis.jpeg" alt="Image of the hadada ibis bird" >}}



