# setup-imagemagick

This action downloads the latest ImageMagick binary and adds it to the PATH.

## Inputs

| Name               | Type    | Description                                                                          |
| ------------------ | ------- | ------------------------------------------------------------------------------------ |
| `cache`            | Boolean | Cache the `magick` download (Ubuntu runners only)                                    |
| `install-libfuse2` | Boolean | Automatically install `libfuse2` so `magick` AppImage works on Ubuntu out-of-the-box |

## Outputs

## Example usage

```yaml
steps:
  - uses: Sonic853/setup-imagemagick@v5mod1
  - run: magick input.pdf -resize 100x100 output.jpg
```
