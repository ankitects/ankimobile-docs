# Adding & Editing

## Adding

To add cards to a deck, tap the "Add" button while reviewing.

The "Type" button at the top allows you to select the type of note you’d
like to add. For more information about note types, please see the
introduction in the [computer version’s manual](https://docs.ankiweb.net/getting-started.html#note-types).

When you tap on a field, a keyboard will come up, allowing you to type
in information. You can use the next and previous buttons to move
between fields.

The toolbar has the following icons:

**B I U**\
Mark the text as bold, italics or underline.

**Fx**\
Remove formatting.

**Paintbrush**\
Only available in iOS 13+. Sets the text color.

**Paperclip/Camera**\
Allows you to add media files from the camera, microphone, photo library
or from a file. On iPads, the mic button is shown separately.

**Pen**\
Only available on iPads on iOS 13+. Allows you to draw an image and
attach it to the card. You can later edit a drawn image by holding two
fingers on it.

**Square root**\
Only available in iOS 13+. Shortcuts to subscript/superscript, and
[MathJax](mathjax.md).

**Eye**\
Shows a preview of how the card will appear when reviewed.

**&lt;/&gt;**\
Reveals the underlying HTML that fields are comprised of.

When you’ve typed in the content of a note, hit the save button to add
it to your collection.

## Editing

To edit a note, tap the "Edit" button while reviewing.

The edit screen is similar to the adding screen mentioned above, with
some key differences:

- There is no note type selection button or deck selection button. If
  you want to change the type of an existing note, you currently need
  to do so with the computer version of Anki.

- There is a "Tools" button at the top of the screen. Tapping on it
  will allow you to perform actions on the current card or note.
  Please see the [action descriptions](study-tools.md#actions) for more information
  on what each action does.

## Browsing

You can search or browse your deck by tapping the "Browse" button while
reviewing.

The browse screen will show all the cards in the current deck by
default.

You can type text into the search box in order to limit the cards
further. If you only wanted to show cards in the current deck that
contain the text "hello" for example, you’d modify the text so it says
`deck:current hello` and then tap return. If you wish to search across
multiple decks, you can remove the `deck:current` part.

AnkiMobile supports all the search strings that the desktop version of
Anki does, allowing you to perform quite complex searches. Some
examples:

`tag:marked` show cards that with the tag "marked"

`is:due` show only cards that are waiting for review

`front:rabbit` show only cards where the front field is exactly "rabbit"

For a full list of the possibilities, please see the section in the
[desktop manual](https://docs.ankiweb.net/searching.html).

Tapping the Filter button will reveal a list of filters you can apply,
like the side bar in the computer version. Tapping on a line will
replace the current search; you can also swipe on a line to add to the
existing search instead.

The Options button will allow you to change what is shown in the left
and right columns, and change the order cards are shown in.

The Select button allows you to select multiple cards at once, and then
perform actions on them like changing their deck, or suspending them.
