* about this blog
* about me
* thoughts:
  * Dec 13: a whale woke up
  * Dec 13: how strong is the ChessCoin network actually?
  * Dec 12: a forking situation
  * Dec 11: created a new website + announcement of first tournament with prizes
  * Dec 10: managing tasks -> prioritize
  * Dec 10: found data on archive.org for Feb 22 blockhashes
  * Dec 10: no uptodate synccheckpoint - for 18 months: 
   * 1. leaves your house open for manipulation attempts + 
   * 2. does not help newcomers (sync speed)
  * Dec 9: motivation

<br><br>

# about this blog

I use this "blog" to show my thoughts on the chess project:
* it should help get things going since the project seems to have not progressed for long time (e.g. [source code](https://github.com/coinforchess/chesscoin) last updated in 2016; I am actually the first one who [reported](https://github.com/COINFORCHESS/ChessCoin/issues/1) a bug in the bug tracker; ...)

You can reply [here](https://github.com/chess-fan/thoughts/issues) (create an issue) or make a [PR](https://github.com/chess-fan/thoughts/pulls), or... just quote me on [bitcointalk](https://bitcointalk.org/index.php?topic=1510517.0) :-)

# about me
* My user account on bitcointalk is [chessfan](https://bitcointalk.org/index.php?action=profile;u=1372252)
* If you like what I do, send me "your appreciation" to this CHESS address: 
  * Ce7kSuKGoS3f5bQkmxLmXKfQjQPH1KyrLc


# thoughts

## Dec 13: a whale woke up

see [here](https://bitcointalk.org/index.php?topic=1510517.msg26245536#msg26245536)

## Dec 13: how strong is the ChessCoin network actually?

see [here](https://bitcointalk.org/index.php?topic=1510517.msg26249572#msg26249572)

## Dec 12: fork situation

This can happen when e.g. there are suddenly jumps in the net weight
* see investigation [here](https://github.com/chess-fan/MCT/issues/15)

## Dec 11: created a new website + announcement of first tournament with prizes

see [here](https://bitcointalk.org/index.php?topic=1510517.msg26137880#msg26137880)

## 2017 Dec 10: managing tasks -> prioritize

I've created today the: [MCT](https://github.com/chess-fan/MCT) (Managing ChessCoin tasks)
* the idea is to priorize tasks, and assign them to willing people
* the other intent is that currently on bitcointalk ideas will just "disappear" over time while here people can respon to each issue directly

## 2017 Dec 10: lucky, b/c found data on archive.org for Feb 22 blockhashes

For past data I could only find for 2017 Feb 22 blockhashes, see [here](https://github.com/chess-fan/blockhashes-of-ChessCoin/issues/1).
* The good thing about it is that it is independent, unmanipulatable data since it's on archive.org


## 2017 Dec 10: no uptodate synccheckpoint - for 18 months - leaves your house open for manipulation attempts + does not help newcomers in terms of sync speed

The current ChessCoin (v1.0.0.0-g32a928e) has as checkpoint only the 18-months-old genesis block #0 (from: 2016 June 5):

![cp](https://user-images.githubusercontent.com/34405095/33800354-b02b1f50-dd3e-11e7-9aed-5d61f48e9b89.png)

Why is it good to have a checkpoint?
* at least until the new checkpoint time, the blockchain can not be manipulated anymore
* the syncing speed for new users will be better 
  * since their clients (which would have a newer checkpoint) will decline clients which are on a fork (and thus would have differing hashes)

Until the [reported bug](https://github.com/COINFORCHESS/ChessCoin/issues/1) is fixed, my bot will add current block hashes in this project (see motivation and more there) to "increase the trust" into ChessCoin's blockchain:
* [blockhashes of ChessCoin](https://github.com/chess-fan/blockhashes-of-ChessCoin)



## 2017 Dec 9: motivation

- replying to:
 > You are exactly the right one who can build us a new wallet... (see [here](https://bitcointalk.org/index.php?topic=1510517.msg26045773#msg26045773))
 - which came on [my statement](https://bitcointalk.org/index.php?topic=1510517.msg26031156#msg26031156):
 > Part of my security analysis shows that the code base is from 2013 (the github version of 2016 is just the upload time).
Anyways, be it 2013 or 2016, when I'd want to "test" something I take the freshest codebase of bitcoin itself and not some old software where security bugs are already known for :-(

<br><br>
me:

I can do that, yes (or also others). The source is free, and can be forked anytime...
As a matter of fact, I have forked it now [here](https://github.com/chess-fan/ChessCoin_source)
* main reason for now: to have the commit comments and with that also: a backup, so the source doesn't disappear

The more important thing would be to "convince" then the majority to USE a possible "new version": e.g. exchanges, ...

And that moment would - short term at least - not be to the benefit of the coin (price goes South... or worse, e.g. coin gets delisted on the exchange(s))
e.g. exchanges would ask: 
* why does the original dev not do this? did he leave?
* can we trust the new wallet and the new dev(s)?
* ...

But let's not forget... first the [current dev](https://github.com/COINFORCHESS) (aka: [Isolani159](https://bitcointalk.org/index.php?action=profile;u=745892)) needs to be contacted about his plans (why he did not update yet; his ongoing plans with ChessCoin; ...) before starting something that brings only negative thoughts, frustration into this all - this is surely not what we all need or want!
* see also my reply [here](https://bitcointalk.org/index.php?topic=1510517.msg26249114#msg26249114)
