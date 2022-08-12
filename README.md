# DuckLibrary

A collection of prompt effect for image generation AIs applied to ducks

With the rise

The entries are in JSON format inside duckbase.json


These lists will be expanded.

# Services

- dalle2
- craiyon

# Type

- light - Modifies the lighting of the scene.
- style - Applies some style, check the description


Format:
```
{
  "prompt": "A duck, dramatic backlighting",
  "template": "[subject], dramatic backlighting",
  "name": "DramaticBacklighting",
  "effect": "Adds a background light to the image",
  "type": "light",
  "generations": [
    {
      "service": "dalle2",
      "date": "2022-04-23T18:25:43.511Z",
      "images": ["dl_duckDramaticBackgroundLight1.png", "dl_duckDramaticBackgroundLight2.png"]
    },
    {
      "service": "craiyon",
      "date": "2022-04-23T18:25:43.511Z",
      "images": ["cr_duckDramaticBackgroundLight1.png", "cr_duckDramaticBackgroundLight2.png"]
    }
  ]
}
```

# Contributing

There are two ways of contributing, opening a Pull Request or an issue.

The prompt subject needs to be "A duck" unless the effect only works on a different subject.

All fields are required.
