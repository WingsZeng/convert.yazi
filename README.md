# convert.yazi

A yazi plugin utilizing ImageMagick's convert to transform unsupported image formats for previewing.

# Requirements

[ImageMagick](https://imagemagick.org/index.php)

# Installation

```
git clone https://github.com/WingsZeng/convert.yazi.git ~/.config/yazi/plugins/convert.yazi
```

# Usage

Here's an example configuration to enable SVG previewing, which isn't supported by yazi yet.

```
[plugin]
prepend_preloaders = [
	{ mime = "image/svg+xml", run = "convert" },
]

prepend_previewers = [
	{ mime = "image/svg+xml", run = "convert" },
]
```

