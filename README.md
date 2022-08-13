# DuckLibrary

A collection of prompt effects for image generation AIs applied to ducks

## [Explore the library](https://www.isageek.com.br/DuckLibrary/)
 
![logo created by dalle](https://raw.githubusercontent.com/beothorn/DuckLibrary/main/images/dalle/DALL%C2%B7E%202022-08-12%2023.38.23%20-%20A%20duck%2C%20modern%2C%20pictorial%20mark%2C%20iconic%20logo%20symbol.png)

# What is this?

There has been a surge of services that transform prompts into images, such as [Dalle](https://labs.openai.com/), [Craiyon](https://www.craiyon.com/),
[Midjourney](https://www.midjourney.com/), [Imagen](https://imagen.research.google/), [Stable diffusion](https://stability.ai/blog/stable-diffusion-announcement) and many others.

With time users have realized that some prompt patterns can be used to achieve similar results with different subjects.

Knowing those patterns is important to optimize the resulting images, with as little generations as possible.

This is being called "prompt engineering" and this an ongoing effort to catalog such patterns and their effects.

These patterns are referenced here as "prompt effects"

# The database

This is a collection of prompt templates (prompt effects) and the resulting images from applying them to a duck.

Each prompt effect entry is a JSON file inside the folder duckbase.

The json structure looks like this:

```javascript
{
  
  "template": "[subject], dramatic backlighting", // A template containg at least the token [subject]
  "name": "DramaticBacklighting", // Unique name
  "effect": "Adds a background light to the image, the subject front has low light", // Description of effect. This is intended to be used by a search so it needs to be a direct description what it does to the output
  "tags": ["light", "photography"], // Tags that fit the prompt effect
  "prompt": "A duck, dramatic backlighting", // A string with the prompt used to create the generations
  "generations": [ // An array of generated images using "A duck" as subject
    {
      "service": "dalle", // Service name
      "date": "2022-04-23", // Date of generation, this helps track model changes
      "images": [ // Array with the urls pointing to the generated images
        "https://raw.githubusercontent.com/beothorn/DuckLibrary/main/images/dalle/DALL%C2%B7E%202022-08-12%2021.19.41%20-%20A%20duck%2C%20dramatic%20backlighting.png",
      ]
    },
    {
      "service": "craiyon",
      "date": "2022-08-12",
      "images": [
        "https://github.com/beothorn/DuckLibrary/raw/main/images/craiyon/cr_DramaticBackgroundLight1.jpeg", 
      ]
    }
  ]
}
```


## Tokens

- subject - What will be rendered, on the generations provided here this is always "A duck"
- color - A color name

## Services

- dalle
- craiyon
- midjourney
- imagen
- stable_diffusion

## Tags

- light - Modifies the lighting of the scene.
- photography - Either converts to a photography or affects it
- style - Applies some style, check the description
- illustration - Either converts to an illustration or affects it


# Contributing

You can:

- Open an [issue](https://github.com/beothorn/DuckLibrary/issues) with all required fields.
- Open a Pull Request with the entry.
- Generate an existing prompt effect with a duck and submit it as an [issue](https://github.com/beothorn/DuckLibrary/issues).

## Important

The prompt subject needs to be "A duck" unless the effect only works on a different subject. This way it is easier to see the effect being applied. 