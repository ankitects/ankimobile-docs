# Getting Started

To start using AnkiMobile, we need to add some cards to study. We can
either download card decks that other people have shared, or add
existing decks from the computer.

## Shared Decks

To download a shared deck directly to your mobile device:

1.  Ensure you’re connected to the internet.

2.  Tap **Add/Export** on the bottom left.

3.  Choose **Shared Deck List**. AnkiWeb will open.

4.  Select a category, or type in a search.

5.  Tap on a deck you’d like to study.

6.  Scroll down and tap **Download**.

7.  Safari will start downloading the file

8.  When it’s done, it will display a button near the top right labeled
    **Open in Anki**. Tap this button.

9.  When the import completes, your deck should be ready to study.

Information on reviewing is available further below.

## Cloud Sync

Anki has a free cloud synchronization service called AnkiWeb that makes
it easy to keep your card decks in sync between mobile devices and your
computer.

To sync with AnkiWeb, you’ll first need to create an account. If you
have used AnkiWeb in the past, you can skip this step.

1.  Visit <https://ankiweb.net> and click the **Sign Up** button.

2.  Type in your email address and a password of your choice.

### Computer to iPhone/iPad

If you have decks on your computer and would like them to be synced to
AnkiMobile:

1.  Open the computer version and click the sync button at the top right
    of the Anki window.

2.  If prompted to upload or download, choose 'upload' to send your
    cards to AnkiWeb.

3.  Tap Synchronize in AnkiMobile and then 'download' to grab the cards
    from AnkiWeb.

### iPhone/iPad to Computer

If you have decks in your phone/iPad and would like them to be synced to
the computer version:

1.  Tap Synchronize in AnkiMobile and then 'upload' to send the cards to
    AnkiWeb.

2.  Open the computer version and click the sync button at the top right
    of the Anki window.

3.  If prompted to upload or download, choose 'download' to grab your
    cards from AnkiWeb.

### Subsequent Syncs

If you have a lot of sounds or images on your cards, the first sync may
take some time.

After the first synchronization has completed, you can click the
synchronize button again any time you wish to synchronize your changes
to the cloud. Only changes made since the previous sync will be sent, so
subsequent syncs are a lot faster.

If you add some new cards on the desktop computer and want to sync them
to AnkiMobile, you’d repeat the same process: sync on desktop (or close
the program, as it syncs automatically on close by default), and then
tap the sync button on AnkiMobile.

The sync button will change colour when a normal or full sync is required.

## iTunes Import/Export

If you don’t have regular internet access, it’s still possible to copy
decks back and forth to your device, by using iTunes.

The iTunes import/export works by importing or exporting **all your
decks at once**, in a special file called collection.apkg or .colpkg.
This means that unlike syncing via AnkiWeb, you can’t make changes from
two locations at once and then merge them - you need to make sure you’ve
imported any recent changes from your other device before you make
changes, or you’ll end up losing the changes made on one device.

Thus the workflow you would typically use is to export your collection
from your mobile device and import it into the computer version, make
modifications (such as importing a shared deck you downloaded to your
computer), and then export your collection and import it back into your
mobile device.

AnkiMobile can’t directly import text files. If you wish to do that,
you’ll need to do that with the computer program, and then import your
collection into AnkiMobile.

### Computer to iPhone/iPad

On your computer:

1.  Open the computer version of Anki.

2.  Choose File&gt;Export from the menu.

3.  Click the 'Export…​' button. Make sure to leave "all decks"
    selected, and "Include scheduling information" must also remain
    checked.

4.  Anki will automatically create a collection.apkg or .colpkg file on
    your desktop. If the file is named something else like
    'deckname.apkg', please see the previous step again.

5.  Connect your Apple device to your computer via the USB cable, or
    wi-fi if you have wi-fi syncing set up in iTunes.

6.  Open iTunes if it doesn’t open automatically.

7.  Locate Anki’s file sharing section with [Apple’s
    instructions](http://support.apple.com/kb/HT4094).

8.  Drag the collection.apkg or .colpkg file from your desktop into
    iTunes.

9.  Click the sync button inside iTunes.

Then in AnkiMobile, in the deck list screen:

1.  Tap the Add/Export button on the bottom left.

2.  Choose **Import from iTunes**, then confirm the replacement.

3.  If you receive a message about "No file found to import", please
    read the "on the computer" section above again.

Once complete, the decks on your device will have been replaced with the
decks from your desktop.

When you import a collection.apkg or .colpkg file, Anki will avoid
copying any sounds or images if they already exist on your mobile
device, and are the same file size. This will make imports after the
first one considerably faster if you have a lot of media files.

### iPhone/iPad to Computer

On AnkiMobile:

1.  Tap the Add/Export button on the bottom left.

2.  Choose **Export to iTunes**, and tap **Export**

Then on your computer:

1.  Connect your Apple device to your computer via the USB cable.

2.  Open iTunes if it doesn’t open automatically.

3.  Locate Anki’s file sharing section with [Apple’s
    instructions](http://support.apple.com/kb/HT4094).

4.  Drag the collection.apkg or .colpkg file from iTunes to your
    desktop.

5.  If you’re still using Anki 2.0 on your computer, rename the file to
    'collection.apkg'. This step is not required if you’re using the
    Anki 2.1.

6.  Use File&gt;Import in Anki to import the file.

7.  Confirm you wish to replace, so that the deck from your mobile
    device overwrites the old data on your desktop.

8.  After importing, you can delete the file on your desktop if you
    wish.
