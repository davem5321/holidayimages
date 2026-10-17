# Holiday Studio

A lightweight holiday image prompt builder. Choose creative details, edit the resulting prompt, and open it in Bing search or copy it to use elsewhere.

**This app builds prompts; it does not generate images.** Bing opens in a new tab with the prompt as its search query.  If the image is not automatically start generating, then select the Bing prompt window and press enter to have your image created.

## Getting started

Open [index.html](index.html) in a modern web browser with JavaScript enabled. No installation, build step, API key, or backend is required.

The page can also be hosted on a static website service, such as GitHub Pages.

## How to use

1. Choose any combination of creative details. Every selection is optional.
2. Review the generated text in **Your prompt**.
3. Edit the prompt directly to add personal touches or refine the instructions.
4. Select **Open in Bing** to search with the edited prompt, or **Copy prompt** to use it in another tool.
5. Select **Reset all** to clear the selections, custom greeting, and prompt.

Changing a dropdown selection or typing in the custom greeting rebuilds the prompt from the form, replacing any manual edits in the prompt box. Make your selections first, then edit the final prompt.

## Creative controls

The builder offers 16 optional controls:

| Section | Controls |
| --- | --- |
| Set the scene | Tone and mood, holiday, subject, setting and context, audience |
| Make it feel like you | Color palette, artistic style, texture and pattern, lighting and shadows |
| Add the finishing touches | Perspective, imagery and symbols, composition, shape and framing, greeting or text, amount of detail, format |

Additional personalization includes:

- **Audience:** anyone, young children, family, a friend, a partner, or colleagues.
- **Shape and framing:** square, portrait, landscape, or wide banner.
- **Greeting or text:** no text, a preset holiday greeting, or a custom message of up to 120 characters.
- **Amount of detail:** simple and minimal, balanced, richly detailed, or highly intricate.

These choices become natural-language instructions, not enforced image-generation settings. Any image tool used afterward may interpret them differently, and text within generated images may need correction.

## Technology

All markup, styling, options, and browser-side JavaScript live in [index.html](index.html). The project has no external package dependencies.

- Responsive layout for desktop and mobile.
- Live prompt preview and selection count.
- Editable prompt submitted through a standard HTML GET form.
- Clipboard copying, with manual-copy guidance if clipboard access is unavailable.

Prompt building works locally. Opening Bing requires an internet connection and sends the prompt in the search URL, so avoid including sensitive information.

## Customization

Edit [index.html](index.html) to change the options or appearance:

- Each dropdown option's `value` supplies its prompt instruction; its visible text is the user-facing label.
- The `updatePrompt()` function assembles the selected instructions and updates the preview and selection count.
- The inline stylesheet controls the layout, colors, and responsive behavior.

There is no automated test suite or build process. After making changes, open the page in a browser and check prompt updates, manual editing, copying, reset behavior, and the Bing handoff.
