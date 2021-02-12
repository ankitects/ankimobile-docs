# Night Mode Styling

By using the Edit Card Template action, it is possible to customize how
cards appear when night mode/dark mode is enabled.

If you wanted a grey background instead of black, you could use
something like:

```css
.card.nightMode {
  background-color: #555;
}
```

If you have a 'myclass' style, the following would show the text in
yellow when night mode is enabled:

```css
.nightMode .myclass {
  color: yellow;
}
```
