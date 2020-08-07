# divinerites-images-asset

## Usage

```go-html-template
{{ $dict := (dict "context" . "path" .image "size" "200x" "action" "Resize" "title" .name )}}
{{ partial "image_asset.html" $dict }}
```

## Need to use a porfolio or any image's url

```go-html-template
{{ $dict := (dict "context" . "path" .image "size" "200x" "action" "Resize" "title" .name "pf" true "pf_size" "800x")}}
{{ partial "image_asset.html" $dict }}
{{ $asset_relurl := partial "image_asset_relurl.html" $dict }}
```

Then Use the `{{ $asset_relurl }}` variable as you want.

### Credits

- Copyright © 2020 onwards, Didier Divinerites
