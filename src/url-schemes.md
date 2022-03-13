# URL Schemes

AnkiMobile supports URL schemes for opening third party dictionaries,
and for adding content to AnkiMobile from other applications.

## AnkiMobile’s URL Scheme

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

    anki://x-callback-url/addnote?profile=User%201&type=Basic&deck=Default&fldFront=front%20text&fldBack=back%20text

The first part must always be there:

    anki://x-callback-url/addnote?

After the first part, keys and values are separated by an ampersand. The
following keys must always be provided:

- `profile=<profile name>`

- `type=<note type name>`

- `deck=<deck name>`
    - Separate nested decks with `::` 
      - `deck=<deck name>::<sub deck name>`

Fields are entered by prefixing their name with "fld". So if your first
field is called "Text", the key would be "fldText". The field text is
interpreted as HTML, so if you wanted a newline in the text you’d use
something like "line 1&lt;br&gt;line 2".

Special characters in the URL must be escaped. For example, if you have
spaces in a field, they must be represented with `%20`. If you’re using
the Shortcuts app, there is a URL encode action which you may find
useful.

The remaining keys are optional:

- `tags=<tags separated by space>`

- `dupes=1` - if provided, allow a note to be added even if the same
  content is on an existing note.

- `x-success=<url scheme for another app>` - use to automatically
  return to another app after the note is added.

If a field you provide is a link to an image or audio file, AnkiMobile
will automatically download that media and place a link to it in the
field. Eg:

    fldFront=http://example.com/image.jpg

The link will only be downloaded if it ends with a recognized file
extension. If your link is to a dynamic webpage, you can add a fake
argument with the extension at the end, eg
`http://example.com/getImage?imgID=1234&fakePath=foo.jpg`. Be careful to
escape the URL before including it in the URL scheme, as otherwise ? and
& characters will be interpreted as part of the URL scheme instead of
the URL.

## Dictionary Links

The desktop version of Anki provides the ability to open a web page
based on the contents of a field, for easily creating a link to an
online dictionary site. This is documented [in this
section](https://docs.ankiweb.net/templates/fields.html#dictionary-links) of
the manual, though please start from the [cards &
templates](https://docs.ankiweb.net/templates/intro.html) section
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
