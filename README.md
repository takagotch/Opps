### opps
---
http://opps.github.io/opps/

```py
from django.db import models
from opps.containers.models import Container

class Musics(Container):
  music = models.CharField(_(u"Music"), max_length=140)
  author = models.CharField(_(u"Author"), max_length=140)
  studio = models.CharField(_(u"Studio"), max_length=200)

  class META:
    verbose_name = _('Music')
    verbose_name_plural = _('Musics')

from django.contrib import admin
from opps.containers.admin import ContainerAdmin
from .models import Musics
admin.site.register(Musics, ContainerAdmin)
```

```
{% set containerbox.ordered_box-containers as items %}
{{items.0}}
{{items.0.container}}

{% if context.fields.articlespost_checkbox_show_main_image_yes == 1 %}
{% get_custom_field_value context 'articlespost-checkbox-show-main-image_yes' as new_name_you_var %}
{% if new_name_your_var == 1 %}
```

```
```


