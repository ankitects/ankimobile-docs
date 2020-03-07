# More Features

## Filtered Decks

Anki is designed to optimize the learning process, so that you study the
minimum amount necessary to remember the majority of your cards. Once
the congratulations screen is reached, further study becomes a case of
diminishing returns: the amount of extra time spent going over the same
cards again is generally not worth the moderate increase in retention
you’ll see.

That said, if you have a test looming, or simply want to pass some time,
it’s possible to keep reviewing once the congratulations screen is
reached.

A 'filtered deck' is a temporary deck that contains cards based on
various criteria, such as "forgotten today", "is tagged 'hard'", and so
on. After studying cards in a filtered deck, or when the filtered deck
is deleted, the cards are automatically returned to their original deck.

The easiest way to create a filtered deck is by using the "custom study"
feature. A custom study link will appear when you’ve finished all
waiting cards in a deck. You can also access custom study ahead of time
by clicking the tools button, and then choosing "Custom Study".

Advanced users can create a filtered deck manually, by clicking the
tools button, then choosing "More" and then "Filter/Cram".

For further information on filtered decks, please see the [computer
version’s
documentation](https://apps.ankiweb.net/docs/manual.html#filtered).

## Text to Speech

AnkiMobile 2.0.56+ supports using TTS tags in card templates. Please see
[the computer
manual](https://apps.ankiweb.net/docs/manual.html#text-to-speech) for
more information.

To get the best quality sound, please go to the iOS Settings app, then:

-   Tap on Accessibility

-   Tap on VoiceOver

-   Tap on Speech

-   Tap on Voice

-   Tap on the voice you want to use

-   If there is an (Enhanced) version available, download it.

Please note that Apple limit Siri to their own apps, so you will need to
pick a voice other than Siri.

The Voice section will only show options for your current language. To
add voices for other languages, tap on "Rotor Languages", and after
selecting another language, you will have a chance to download voices.

Like regular audio, text to speech will not play automatically when your
device’s mute/vibrate switch is enabled.

## Custom Fonts

AnkiMobile allows you to use non-system fonts on your cards. To set them
up, the desktop client is required. Please see [the section in the
desktop
manual](https://apps.ankiweb.net/docs/manual.html#installingfonts) for
more information.

Please note that AnkiMobile has to load the entire font into memory in
order to use it, and fonts for Asian languages can be quite large. If
you have an older device and notice AnkiMobile crashing frequently after
installing a font, you may have exceeded your device’s memory limits.

## Night Mode Styling

By using the Edit Card Template action, it is possible to customize how
cards appear when night mode/dark mode is enabled.

If you wanted a grey background instead of black, you could use
something like:

```css
.card.nightMode { background-color: #555; }
```

If you have a 'myclass' style, the following would show the text in
yellow when night mode is enabled:

```css
.nightMode .myclass { color: yellow; }
```

## URL schemes

AnkiMobile supports URL schemes for opening third party dictionaries,
and for adding content to AnkiMobile from other applications.

### AnkiMobile’s URL Scheme

A 'URL Scheme' is like a link to a website, but it instead links to an
app. A simple example is:

    anki://

If you type this into Safari on your device, you’ll see AnkiMobile open
up.

From 2.0.30 onwards, AnkiMobile provides a scheme for adding new notes
to your collection. This can be used with dictionary apps that support
calling other apps via URL schemes, and with automation apps like
Workflow.

The scheme to add cards looks like this:

    anki://x-callback-url/addnote?profile=User 1&type=Basic&deck=Default&fldFront=front text&fldBack=back text

The first part must always be there:

anki://x-callback-url/addnote?

After the first part, keys and values are separated by an ampersand. The
following keys must always be provided:

-   profile=&lt;profile name&gt;

-   type=&lt;note type name&gt;

-   deck=&lt;deck name&gt;

Fields are entered by prefixing their name with "fld". So if your first
field is called "Text", the key would be "fldText". The field text is
interpreted as HTML, so if you wanted a newline in the text you’d use
something like "line 1&lt;br&gt;line 2".

Special characters in the URL must be escaped. For example, if you have
spaces in a field, they must be represented with `%20`. If you’re using
the Shortcuts app, there is a URL encode action which you may find
useful.

The remaining keys are optional:

-   tags=&lt;tags separated by space&gt;

-   dupes=1 - if provided, allow a note to be added even if the same
    content is on an existing note.

-   x-success=&lt;url scheme for another app&gt; - use to automatically
    return to another app after the note is added.

If a field you provide is a link to an image or audio file, AnkiMobile
will automatically download that media and place a link to it in the
field. Eg:

    fldFront=http://example.com/image.jpg

The link will only be downloaded if it ends with a recognized file
extension. If your link is to a dynamic webpage, you can add a fake
argument with the extension at the end, eg
<http://example.com/getImage?imgID=1234&fakePath=foo.jpg>. Be careful to
escape the URL before including it in the URL scheme, as otherwise ? and
& characters will be interpreted as part of the URL scheme instead of
the URL.

### Dictionary Links

The desktop version of Anki provides the ability to open a web page
based on the contents of a field, for easily creating a link to an
online dictionary site. This is documented [in this
section](https://apps.ankiweb.net/docs/manual.html#_dictionary_links) of
the manual, though please start from the [cards &
templates](https://apps.ankiweb.net/docs/manual.html#templates) section
as the above link assumes you have read it.

Like the desktop, AnkiMobile supports links to dictionary websites. In
addition to that, you can also link to different dictionary apps that
you have installed on your device using a URL scheme.

Some dictionary apps provide a URL scheme that allows you to provide a
particular phrase to search for. For example, an app called iDict+
allows the following type of URL:

    idictplus://?search=mysearchtext

If you have iDict+ installed and type that into Safari, iDict+ should
open up and immediately search for "mysearchtext".

iDict+ also supports passing a return link. We can replace the above
with:

    idictplus://?search=txt&scheme=anki://

If you type that into Safari, it will search for "mysearchtext" like
before, but will also provide a "return" button that when pressed will
open up Anki.

By taking that text and combining it with the instructions for the
desktop version linked above, it’s possible to have a link on your cards
that searches for a word in another app, and then allows you to return
to Anki when you’re done.

Unfortunately, there is no standard for URL schemes: some apps implement
them, some don’t, and the way they implement them can different. For
example, in the app called "Kotoba!", the URL scheme is:

    kotoba://dictionary?word=mysearchtext

Note how not only the app name differs but also the text after it, and
how Kotoba! doesn’t provide the ability to automatically return to the
app that opened it, meaning that you need to double tap the home button
and manually return to AnkiMobile.

Some dictionary apps publish their URL scheme in their documentation. If
you’re using a dictionary app that doesn’t, please contact the authors
and ask them for more information.

## MathJax

AnkiMobile supports MathJax out of the box. Simply place something like
the following on your card:

    This is some text \(x^2\) with an inline equation.

    An equation block:

    \[\sqrt{-1}\]

## Javascript

The [warnings](https://apps.ankiweb.net/docs/manual.html#javascript)
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
<https://apps.ankiweb.net/docs/manual.html#audio-replay-buttons>

## Image Resizing

When you attach an image from the photo gallery it is automatically
resized to have a maximum length of 1024 along its longest edge.

As of 2.0.39, you can customize this limit. For example, to set it to
2048, run the following in the computer version’s [debug
console](https://apps.ankiweb.net/docs/manual.html#debug-console) then
sync to AnkiMobile:

    mw.col.conf["amImageMaxSize"] = 2048
    mw.col.setMod()
    mw.col.save()

## Debug Log

If you’re encountering a problem with Anki and we’ve asked you to
provide a debug log, please follow the following steps:

1.  Connect your device via USB.

2.  Open iTunes if it doesn’t open automatically.

3.  Locate Anki’s file sharing section with [Apple’s
    instructions](http://support.apple.com/kb/HT4094).

4.  Drag the debug.log file on to your desktop, then attach it to your
    support ticket.
