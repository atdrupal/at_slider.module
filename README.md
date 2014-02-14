AT Slider
===

This is a very simple module that provides slider blocks to your Drupal site.

Built on:

- AT Base — For config, helper functions, …
- Bean module — Block as Entity
- Field Collection — Each slide (bean entity) has image or more information, like
    text, links, … FieldCollection module allow Drupal admin add fields to entity
    field.
- Image — Provide image field for slider item.
- Features — Used for preconfig things.
- jQuery Cycle 2

### Customize

We can provide options for each slider bean rendered on page.

1. In my_module.info, add `dependencies[] = at_slider`
1. Create `/path/to/my_module/config/slider_options.yml
1. Define slider_options.yml like this:

```yaml
options:
    default:
        speed: 600
        manualSpeed: 100
```

jCycle options reference can be found at http://jquery.malsup.com/cycle2/api/#options

Started by Andy Truong for GO1.