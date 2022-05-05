# Cloud Sync

Anki has a free cloud synchronization service called AnkiWeb that makes
it easy to keep your card decks in sync between mobile devices and your
computer. If you are an existing Anki user with cards on your computer,
syncing is the easiest way to start using those cards on your mobile device
as well.

<!-- toc -->

## Intro Videos

Please check out these short videos that explain syncing:

- [Initial Setup](https://www.youtube.com/watch?v=YkiM4DPzSVc&list=PLGgmaKOIHykFoomqkBJAyGiDQ2kyiuTao)
- [Syncing Sounds and Images](https://www.youtube.com/watch?v=phP9GGG-PxY&list=PLGgmaKOIHykFoomqkBJAyGiDQ2kyiuTao&index=2)
- [One-Way Syncs](https://www.youtube.com/watch?v=UEAcpfMQnjo&list=PLGgmaKOIHykFoomqkBJAyGiDQ2kyiuTao&index=3)

If you'd prefer not to watch videos, please read on.

## Creating an Account

To sync with AnkiWeb, you’ll first need to create an account. If you
have used AnkiWeb in the past, you can skip this step.

1.  Visit <https://ankiweb.net> and click the **Sign Up** button.

2.  Type in your email address and a password of your choice.

## Computer to iPhone/iPad

If you have decks on your computer and would like them to be synced to
AnkiMobile:

1.  Open the computer version and click the sync button at the top right
    of the Anki window.

2.  If prompted to upload or download, choose 'upload' to send your
    cards to AnkiWeb. Please make sure you [wait for media files to finish
    syncing](https://faqs.ankiweb.net/media-files-may-take-time-to-sync.html).

3.  Tap Synchronize in AnkiMobile and then 'download' to grab the cards
    from AnkiWeb. Please make sure you [wait for media files to finish
    syncing](https://faqs.ankiweb.net/media-files-may-take-time-to-sync.html).

## iPhone/iPad to Computer

If you have decks in your phone/iPad and would like them to be synced to
the computer version:

1.  Tap Synchronize in AnkiMobile and then 'upload' to send the cards to
    AnkiWeb.

2.  Open the computer version and click the sync button at the top right
    of the Anki window.

3.  If prompted to upload or download, choose 'download' to grab your
    cards from AnkiWeb.

## Subsequent Syncs

If you have a lot of sounds or images on your cards, the first sync may take
some time, and until it completes, [sounds and images may fail to
appear](https://faqs.ankiweb.net/media-files-may-take-time-to-sync.html).

After the first synchronization has completed, you can click the
synchronize button again any time you wish to synchronize your changes
to the cloud. Only changes made since the previous sync will be sent, so
subsequent syncs are a lot faster.

If you add some new cards on the desktop computer and want to sync them
to AnkiMobile, you’d repeat the same process: sync on desktop (or close
the program, as it syncs automatically on close by default), and then
tap the sync button on AnkiMobile.

The sync button will change colour when a normal or full sync is required.

## Missing Images

If you receive a message about an image being missing, the most common cause
is because [media has not finished syncing yet](https://faqs.ankiweb.net/media-files-may-take-time-to-sync.html). Please follow the steps on that page
to confirm that all of your Anki clients have finished syncing media. Remember
that if you've added images on your computer, you'll need to confirm the computer
has finished syncing first, and then check AnkiMobile.

If you have confirmed media has finished syncing, but still receive a message
about a missing image, then it is possible that the author of the shared deck
you are using has accidentally or deliberately failed to include one or more
images.

If you're able to contact the deck author, it may be worth notifying them of the
issue, as they may be able to provide you with the missing image in a deck update.
If you're unable to reach them, and want to make the warning go away, please read on.

If you open the Edit screen and see a broken image icon, one of the images
on that card is missing. You can delete the image icon to make the warning go away.

If you see a warning about the same image name on every card, it means that the
deck author has added an image to the "Card Template", which is shared by multiple
cards. You can make the message go away by tapping on the gear/cog in the bottom right
of the review screen, then scrolling down to "Card Template". In the screen that follows,
search for the image name in both the Front and Back of the card - it will look something
like `<img src="myimage.jpg">`. Remove the text starting with `<img` and ending with `>`,
and it should resolve the problem.
