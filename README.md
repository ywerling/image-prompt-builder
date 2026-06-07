# Image Prompt Builder

A simple, single-file browser app for composing image generation prompts from reusable templates.

## How to use

1. Open `prompt-builder.html` in any web browser (no installation required).
2. Click **Choose File** and select a `.txt` template file.
3. Fill in the input boxes that appear — one per parameter in the template.
4. The generated prompt updates live as you type.
5. Click **Copy Prompt** to copy the final text to your clipboard.

## Template format

Templates are plain `.txt` files. Wrap each variable part of the prompt in square brackets:

```
a wildlife photography of [animal] in a breathtaking [setting] landscape
```

- Parameter names can be anything: `[animal]`, `[style]`, `[time of day]`, etc.
- Each unique `[parameter]` gets its own input box in the app.
- The same parameter can appear multiple times in the template — editing its box updates all occurrences.
- Parameters are detected automatically; no special syntax beyond the brackets is needed.

### Example template file

```
a [style] photograph of [subject], shot during [time of day], with a [mood] atmosphere
```

This produces four input boxes: `style`, `subject`, `time of day`, and `mood`.

## Tips

- Save your favourite templates as separate `.txt` files and load whichever you need.
- Unfilled parameters stay visible in the output as `[parameter name]` so you can see what's missing before copying.
