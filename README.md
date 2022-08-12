# DuckLibrary

A collection of prompt effects for image generation AIs applied to ducks
 
![logo created by dalle](https://raw.githubusercontent.com/beothorn/DuckLibrary/main/images/dalle/DALL%C2%B7E%202022-08-12%2023.38.23%20-%20A%20duck%2C%20modern%2C%20pictorial%20mark%2C%20iconic%20logo%20symbol.png)

The entries are in JSON format inside the folder duckbase


These lists will be expanded.

# Services

- dalle
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
  "effect": "Adds a background light to the image, the subject front has low light",
  "type": "light",
  "generations": [
    {
      "service": "dalle2",
      "date": "2022-04-23T19:41:00.000Z",
      "images": [
        "https://raw.githubusercontent.com/beothorn/DuckLibrary/main/images/dalle/DALL%C2%B7E%202022-08-12%2021.19.41%20-%20A%20duck%2C%20dramatic%20backlighting.png",
	"https://raw.githubusercontent.com/beothorn/DuckLibrary/main/images/dalle/DALL%C2%B7E%202022-08-12%2021.19.47%20-%20A%20duck%2C%20dramatic%20backlighting.png",
	"https://raw.githubusercontent.com/beothorn/DuckLibrary/main/images/dalle/DALL%C2%B7E%202022-08-12%2021.19.52%20-%20A%20duck%2C%20dramatic%20backlighting.png",
	"https://raw.githubusercontent.com/beothorn/DuckLibrary/main/images/dalle/DALL%C2%B7E%202022-08-12%2021.19.58%20-%20A%20duck%2C%20dramatic%20backlighting.png",
      ]
    },
    {
      "service": "craiyon",
      "date": "2022-08-12T21:00:00.000Z",
      "images": [
        "https://github.com/beothorn/DuckLibrary/raw/main/images/craiyon/cr_DramaticBackgroundLight1.jpeg", 
	"https://github.com/beothorn/DuckLibrary/raw/main/images/craiyon/cr_DramaticBackgroundLight2.jpeg",
	"https://github.com/beothorn/DuckLibrary/raw/main/images/craiyon/cr_DramaticBackgroundLight3.jpeg",
	"https://github.com/beothorn/DuckLibrary/raw/main/images/craiyon/cr_DramaticBackgroundLight4.jpeg",
      ]
    }
  ]
}
```

# Contributing

There are two ways of contributing, opening a Pull Request or an issue.

The prompt subject needs to be "A duck" unless the effect only works on a different subject.

All fields are required.
