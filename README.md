Tweeter 
=======

Send tweets with bad-word checking and autocorrection

Requires [`python-twitter`](https://code.google.com/p/python-twitter/), which can be installed with `pip`.

To approve dirty tweets, editors require the `approve_tweets` permission.

Words or patterns can be marked as dirty by creating a "DirtyWords" object in
the admin console. Words that need replacing (e.g. for rebranding) can be added as "Replacement"
objects.

Both dirty and replaceable words will be wrapped to match word boundaries and
not preceded by a hashtag (`#`) unless the "Raw regex" option is marked.

Remember to `syncdb` before using.
