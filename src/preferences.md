# Preferences

The preferences screen can be accessed by tapping on the gear icon at
the top right of the deck list. It allows you to customize various
application settings and how AnkiMobile appears.

The Preferences screen is divided up into different sections, which are
covered below.

## Syncing

The syncing screen allows you to customize [cloud synchronization](syncing.md) with
AnkiWeb.

**Sync Sounds & Images**  
By default, AnkiMobile will sync sounds and images as well as your cards
and review history. If you disable this option, sounds and images will
not be synced by AnkiMobile.

**Full Sync**  
The full sync button allows you to force a full upload or download of
your cards. This is useful if you accidentally deleted some cards and
want to revert to the local or remote version, instead of having those
deletions propagate to other devices. After tapping the button, you’ll
be given a choice of whether you want to upload your collection or
download it from AnkiWeb. Please note this option only affects how
cards, notes and review history is transferred - it does not change how
sounds and images are synced.

## Review

The review screen allows you to customize how AnkiMobile behaves when
you’re reviewing cards.

**Feedback Ticks**  
Flash a tick or cross in the top right to confirm your answer choice.

**Tools Overlay Button**  
Show the gear/cog icon on the study screen. If you prefer not to see it,
you can assign the tools action to the top bar instead.

**Tools Overlay Position**  
Allows you to put the tools button on the left.

**Audio Buttons**  
Allows you to hide the play button that appears for each audio file
you’ve placed on the card. Useful if you’d rather replay audio via the
"Replay Audio" action bound to a swipe or tap.

**Always Duck + Ignore Mute**  
When enabled, AnkiMobile will quieten any music you have playing in the
background, and will automatically play audio even when the
mute/vibrate/silent switch is turned on.

**Answer Keeps Zoom**  
By default, if you have zoomed in on a card, the screen will zoom out
when you reveal the answer. If you enable this option, AnkiMobile will
not zoom out.

**Never Type Answer**  
If you have set up your cards to ask you to type in the answer (as
explained in [this
section](https://docs.ankiweb.net/templates/intro.html) of the
desktop manual), AnkiMobile will display a keyboard on such cards and
allow you to check your answer. If you find typing on a mobile device
inconvenient, you can use this option to disable the keyboard for all
cards.

**Shake Action**  
Allows you to customize what happens when you shake your device. The
default action is to undo the previous answer.

**Double Tap Prevention**  
This option ignores a second tap when two taps are made in quick
succession, so that you don’t accidentally reveal the answer or advance
to the next card. If you review your cards very quickly, you may wish to
select a shorter detection time.

### Scheduling

These options affect the way Anki schedules cards in all decks.

**New/Review Order**  
Whether Anki should introduce new cards before, after, or together with
review cards.

**Day Starts**  
Controls when a new day starts and new cards become available. Default
is 04:00, which means new cards become available at 4AM.

**Learn Ahead Minutes**  
The number of minutes to look ahead when the only cards remaining to
review with a next repetition time in the future. The default is 20
minutes, which means cards due to show in 10 minutes will be shown
immediately if nothing else is available to show.

### Notifications

When enabled, Anki will display an alert at the selected time of day,
reminding you to study and telling you how many reviews are waiting.

### Top Bar

You can assign frequently used actions to the top bar for convenient
access. For an explanation of the available actions, please see the
[actions list](study-tools.md#actions).

### Bottom Bar

**Show Bottom Bar**  
Hides or shows the bottom area that shows the answer buttons and card
counts.

**Remaining Count**  
Whether to show the card counts when the question side of a card is
being shown.

**Answer Buttons**  
Whether to show the answer buttons on the answer side of a card.

**Next Times**  
Whether to show the next study time above each of the answer buttons.

### Taps

When you’re reviewing, you can tap on different parts of a card in order
to trigger different actions.

Anki divides the screen into 9 sections:

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Top Left</p></td>
<td><p>Top Center</p></td>
<td><p>Top Right</p></td>
</tr>
<tr class="even">
<td><p>Mid Left</p></td>
<td><p>Mid Center</p></td>
<td><p>Mid Right</p></td>
</tr>
<tr class="odd">
<td><p>Bottom Left</p></td>
<td><p>Bottom Center</p></td>
<td><p>Bottom Right</p></td>
</tr>
</tbody>
</table>

Each section can have a different action assigned to it if you wish, and
the taps when the question is shown are also different from the taps
when the answer is shown.

By default, AnkiMobile responds as follows when the question in shown:

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Show Answer</p></td>
<td><p>Show Answer</p></td>
<td><p>Show Answer</p></td>
</tr>
<tr class="even">
<td><p>Show Answer</p></td>
<td><p>Show Answer</p></td>
<td><p>Show Answer</p></td>
</tr>
<tr class="odd">
<td><p>Show Answer</p></td>
<td><p>Show Answer</p></td>
<td><p>Show Answer</p></td>
</tr>
</tbody>
</table>

In other words, tapping anywhere on the screen will show the answer.

When the answer is shown, by default AnkiMobile responds as follows:

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Answer "Again"</p></td>
<td><p>Off</p></td>
<td><p>Answer "Good"</p></td>
</tr>
<tr class="even">
<td><p>Answer "Again"</p></td>
<td><p>Off</p></td>
<td><p>Answer "Good"</p></td>
</tr>
<tr class="odd">
<td><p>Answer "Again"</p></td>
<td><p>Off</p></td>
<td><p>Answer "Good"</p></td>
</tr>
</tbody>
</table>

This allows you to tap on the left side of the screen to trigger the red
button, and the right side of the screen to trigger the green button.
Taps near the middle of the screen will be ignored.

You can assign frequently used actions to taps for convenient access.
For an explanation of the available actions, please see the [actions
list](study-tools.md#actions).

### Swipes

You can also swipe up, down, left or right across a card to trigger an
action.

To ensure swipes don’t interfere with your ability to scroll on a large
card or select text, a swipe must begin from the far left or right side
of the screen. Begin by placing your finger on the left or right side of
the screen, and then move it up, down, left or right to trigger the
relevant swipe.

With the default settings:

- Swiping left displays the tools window

- Swiping right returns to the deck list

You can assign frequently used actions to swipes for convenient access.
For an explanation of the available actions, please see the [actions
list](study-tools.md#actions).

### Scratchpad

**Ignore Fingers**  
When enabled, the scratchpad will only respond to the Apple Pencil.

**Undo Clears All**  
Reverses the behaviour of the undo button, so a quick tap clears
everything, and a long press clears the last stroke.

**Scratchpad Below Buttons**  
Whether the scratchpad should be placed above or below the bottom bar.

### Auto Advance

**Wait for Audio**  
Don’t advance until the current audio stops playing.

**Answer Action**  
Whether to bury the card, answer it, show a popup reminder, or do
nothing.

### Gamepads

From AnkiMobile 2.0.53+, you can control the study screen with a game controller
on iOS 13+. The controller must be supported by iOS, and must provide an
[extended controller
profile](https://developer.apple.com/documentation/gamecontroller/gcextendedgamepad).
Controllers with fewer buttons can not currently be used. For more information
on setup, please see [this page](https://support.apple.com/en-au/HT210414).

The gamepads section of the preferences allows you to configure which
actions are triggered when each button is pressed. You can assign an
action to each direction on the d-pad, but the analog thumbpads can not
be customized - they will always scroll the card up or down.

## General

## Theme

The theme screen allows you to customize the bar colours AnkiMobile
uses. The available options will depend on whether night mode or iOS
13’s dark mode is enabled.

To customize the appearance of your cards, you’ll need to alter your
card templates. You can do this using the Card Template action in the
tools screen, or by using the computer version. For more info, please
see <http://www.youtube.com/watch?v=F1j1Zx0mXME&yt:cc=on>

## Profiles

Profiles allow multiple users to study with the same device. You can add
profiles from the settings screen. To rename or remove a profile, swipe
to the left on it.

Each profile needs to be synced with its own AnkiWeb account. Please be
careful not to sync two profiles with the same AnkiWeb ID, as this could
lead to data loss.

## Backups

AnkiMobile will automatically create backups of your collection for you.
The backups include all your cards and statistics, but do not include
sounds or images, since they take up a lot of space.

To restore from a backup, open the Backups section in the preferences,
and tap on the backup you wish to restore to.

If you’re unable to get AnkiMobile to start due to a serious error, you
can still retrieve the backups from the iTunes file sharing area:

1.  Connect your Apple device to your computer via the USB cable.

2.  Open iTunes if it doesn’t open automatically.

3.  Locate Anki’s file sharing section with [Apple’s
    instructions](http://support.apple.com/kb/HT4094).

4.  Drag the your backup folder from iTunes to your desktop.

5.  With the computer version of Anki, create a new, empty profile via
    File&gt;Switch Profile, and then File&gt;Import the latest backup
    colpkg from within that profile to confirm that it’s ok. If it is
    corrupt, you can try a previous backup. You'll need Anki 2.1.50+ to
    open the backups.

## Check Database

This will check your collection for a number of possible errors and fix
them if possible.

It also will remove any tags that are no longer used by any cards.

## Check Media

This scans all your notes for references to sounds and images, and then
checks to make sure that the sounds and images are available. It will
display a report letting you know of any sounds or images that are
missing, and any sounds or images that are not used by any cards. If you
tap the delete button, the unused sounds or images will be deleted.
