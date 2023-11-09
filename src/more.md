# More Features

## Javascript

The [warnings](https://docs.ankiweb.net/templates/styling.html#javascript)
that apply to the computer version also apply to AnkiMobile.

In addition to the above, another thing to be aware of in AnkiMobile is
that your code also needs to play nicely with AnkiMobile’s tap
detection. Taps on A/BUTTON elements, or elements that have an onclick
handler should work as you expect.

If you have other elements that must receive tap events, give them the
class 'tappable' to tell AnkiMobile 2.0.39 or later that it should pass
taps through to the element.

## Play Buttons

To change the styling of the audio replay buttons, please see
<https://docs.ankiweb.net/templates/styling.html#audio-replay-buttons>

## Image Resizing

When you attach an image from the photo gallery it is automatically
resized to have a maximum length of 1024 along its longest edge. 

Recent Anki versions allow you to customize this limit in the **Preferences >
General** screen, and control whether the limit should also be applied to
images pasted from the clipboard.
