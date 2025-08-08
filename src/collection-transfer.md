# Collection Transfer

If you don’t have regular internet access, it’s still possible to copy
your collection back and forth between devices, though the process is
not as convenient.

Collection transfer works by importing or exporting **all your
decks at once**, in a special file called `collection.colpkg`.
You can export that file on one device, copy it to another device, and
import it there.

When you import a collection file, any existing content you have is
replaced with the contents of the file - it is a one-way transfer
from your other device.

This means that unlike syncing via AnkiWeb, you can’t make changes from
two locations at once and then merge them - you need to make sure you’ve
imported any recent changes from your other device before you make
changes, or you’ll end up losing the changes made on one device.

A workflow you would typically use is to export your collection
from your mobile device and import it into the computer version, make
modifications (such as importing a shared deck you downloaded to your
computer), and then export your collection and import it back into your
mobile device.

## Computer to iPhone/iPad

### Export the File

On your computer:

1. Open the computer version of Anki.

2. Choose **File>Export** from the menu.

3. Click the **Export​** button. Make sure to leave "All decks"
   and "Include scheduling information" turned on.

4. Anki will automatically create a `collection.colpkg` file on
   your desktop. If the file is named something else like
   `deckname.apkg`, please see the previous step again. If it
   is called `collection.apkg`, that will work - your Anki version
   is just old.

### Transfer the File

If your devices are on the same wifi network and signed in to iCloud, you can
use the AirDrop option in Finder to
[AirDrop](https://support.apple.com/en-au/HT204144) the `collection.colpkg` file
to your mobile device.

If you do not have access to AirDrop, you can use
[Finder](https://support.apple.com/en-us/HT210598) or
[iTunes](http://support.apple.com/kb/HT4094) to drop the .colpkg file into
Anki's file sharing area.

### Import the File

If you AirDropped the file, AnkiMobile should have automatically
popped up and imported the file when you accepted it.

If you transferred the file via iOS file sharing, go to AnkiMobile's
deck list screen, and then:

1. Tap the **Add/Export** button on the bottom left.

2. Choose **Import from iTunes**, then confirm the replacement.

3. If you receive a message about "No file found to import", please
   check to make sure you put the `collection.colpkg` file in AnkiMobile's
   file sharing section.

Once complete, the decks on your device will have been replaced with the
decks from your desktop.

When you import a `collection.colpkg` file, Anki will avoid
copying any sounds or images if they already exist on your mobile
device, and are the same file size. This will make imports after the
first one considerably faster if you have a lot of media files.

## iPhone/iPad to Computer

On AnkiMobile, tap the **Add/Export** button on the bottom left of
the decks list.

### AirDrop

1. Choose **Export to Share**, and then choose **AirDrop**.
2. Select your computer. If your computer doesn't appear, make
   sure you have AirDrop open on your computer.
3. Once the file has arrived on your computer, use **File>Import**
   inside Anki to import the file.

### Finder/iTunes

1. Choose **Export to iTunes**, and tap **Export**.

Then on your computer:

1. Connect your Apple device to your computer via the USB cable.

2. Open Finder or iTunes.

3. Locate Anki’s file sharing section with [Apple’s instructions](http://support.apple.com/kb/HT4094).

4. Drag the `collection.colpkg` file from Finder or iTunes to your
   desktop.

5. Use File>Import in Anki to import the file.

6. After importing, you can delete the file on your desktop if you
   wish.
