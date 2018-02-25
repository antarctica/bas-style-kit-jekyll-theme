# BAS Style Kit Jekyll Theme

## Attribute configuration options

### `bas_style_kit_jekyll_theme.attributes.container`

Allowed values:

* `fixed`
* `fluid`

Default value: `fixed`

Used to determine which [layout container](https://style-kit.web.bas.ac.uk/core/layout/#containers) to use.

### `bas_style_kit_jekyll_theme.attributes.head_title.default`

Allowed values: *Any string*

Default value: `site title`

Used to set the page `<title>` meta element if a value isn't set on a per-page basis (using `page.title`).

It is recommended to use the name of the website for this value.

### `bas_style_kit_jekyll_theme.attributes.head_title.appended`

Allowed values: *Any string*

Default value: *None*

If set, this value will be appended to the site title, if set on a per-page basis (using `page.title`).

**Note:** This value is not appended if the `head_title.default` value is used.

It is recommended to use the name of the website for this value with a separator such as ` - `. No whitespace is added 
before this value - i.e. if the page title is `foo` and this value is `- bar` a title of `foo- bar` will be set.

### `bas_style_kit_jekyll_theme.attributes.head_description`

Allowed values: *Any string*

Default value: `site description`

Sets the `<meta name="description" ..>` meta element.

### `bas_style_kit_jekyll_theme.attributes.site_brand.text`

Allowed values: *Any string*

Default value: `site title`

Sets the navbar brand (i.e. the site name left of the site main navigation) to a text value (i.e. the name of the site).

This option **MAY** be used in conjunction, or instead of, the `site_brand.img` option. If used in conjunction the image
will be shown before the text.

### `bas_style_kit_jekyll_theme.attributes.site_brand.img`

Allowed values: *Any image source (URL)*

Default value: *None*

Sets the navbar brand (i.e. the site name left of the site main navigation) to an image value (i.e. the logo of the 
site).

This option **MAY** be used in conjunction, or instead of, the `site_brand.text` option. If used in conjunction the 
image will be shown before the text.

This option **MUST** be used in conjunction with the `site_brand.img_size` option.

### `bas_style_kit_jekyll_theme.attributes.site_brand.img_size`

Allowed values:

* `32`
* `48`
* `64`
* `96`

Default value: *None*

Sets the navbar image size class to apply the navbar image. These sizes are 
[preset](https://style-kit.web.bas.ac.uk/components/navbar/#brand-image).

This option **MUST** be used if the `site_brand.img` option is used, otherwise it **SHOULD NOT** be used.

### `bas_style_kit_jekyll_theme.attributes.site_brand.href`

Allowed values: *Any URL*

Default value: `/`

The destination for the navbar brand link (which is a `<a>` element container an image and/or text value).

This value **SHOULD NOT** be changed as it is a convention that the site name leads to the site homepage.

### `bas_style_kit_jekyll_theme.attributes.site_development_phase`

Allowed values:

* `backlog`
* `discovery`
* `alpha`
* `beta`
* `live`
* `live-stable`
* `experimental`

Default value: `alpha`

Sets the value for the site development phase banner/notice, except `live-stable` value, where this is hidden. 
This can also be set to show a notice about experimental/testing websites using the `experimental` value.

This option **should** reflect the development phase for the current website.

This option **SHOULD NOT** be set to the `backlog` or `discovery` phase as no code should be written until the `alpha`
phase.

### `bas_style_kit_jekyll_theme.attributes.site_feedback_href`

Allowed values: *Any URL*

Default value: `/feedback.html`

Specifies the value for links to the site feedback page.

**Note:** The default value for this option assumes the site has a feedback page. If it doesn't parts of the standard
layout won't work.

### `bas_style_kit_jekyll_theme.attributes.site_analytics.id`

Allowed values: *Any Google Analytics property ID*

Default value: *None*

If set, Google Analytics page view tracking will be enabled.

### `bas_style_kit_jekyll_theme.attributes.head_favicon`

Allowed values: *Any image source (URL)*

Default value: `data:;base64,iVBORw0KGgo=`

**Note:** This configuration option is rarely changed.

If set, a site favicon will be set.

The default value for this option sets an 'empty' image which will prevent requests for the conventional `favicon.ico`.

### `bas_style_kit_jekyll_theme.attributes.site_back_to_top_target_href`

Allowed values: *Any URL*

Default value: `#site-top`

**Note:** This configuration option is rarely changed.

Sets the destination for 'back to link' links.

This option **SHOULD** be set to an anchor in the current page.

### `bas_style_kit_jekyll_theme.attributes.site_footer.ogl.href`

Allowed values: *Any URL*

Default value: `http://www.nationalarchives.gov.uk/doc/open-government-licence`

**Note:** This value **SHOULD NOT** be changed.

Sets the destination of the OGL symbol and text link used on the site.

### `bas_style_kit_jekyll_theme.attributes.site_footer.ogl.img`

Allowed values: *Any image URL*

Default value: `https://cdn.web.bas.ac.uk/bas-style-kit/0.3.0/img/logos-symbols/ogl-symbol-inverse-transparent-32.png`

**Note:** This value **SHOULD NOT** be changed.

Sets the image to use for the OGL symbol used on the site.

### `bas_style_kit_jekyll_theme.attributes.site_footer.ogl.text_version`

Allowed values: *Any string*

Default value: ``v3.0``

**Note:** This value **SHOULD NOT** be changed.

Sets the version of the OGL license used on the site.

### `bas_style_kit_jekyll_theme.attributes.legal_policies.copyright_href`

Allowed values: *Any URL*

Default value: `/legal/copyright.html`

**Note:** This configuration option is rarely changed.

Sets the value for links to the site copyright policy page.

**Note:** The default value for this option assumes the site has a feedback page. If it doesn't parts of the standard
layout won't work.

### `bas_style_kit_jekyll_theme.attributes.legal_policies.cookies_href`

Allowed values: *Any URL*

Default value: `/legal/cookies.html`

**Note:** This configuration option is rarely changed.

Sets the value for links to the site cookies policy page.

**Note:** The default value for this option assumes the site has a feedback page. If it doesn't parts of the standard
layout won't work.

### `bas_style_kit_jekyll_theme.attributes.legal_policies.privacy_href`

Allowed values: *Any URL*

Default value: `/legal/privacy.html`

**Note:** This configuration option is rarely changed.

Sets the value for links to the site privacy policy page.

**Note:** The default value for this option assumes the site has a feedback page. If it doesn't parts of the standard
layout won't work.