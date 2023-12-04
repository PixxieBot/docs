# Make A Sentence

## What is Make A Sentence?

Users take turns writing one word each in a dedicated channel to make up a sentence together! PixxieBot publishes the finished sentence once a user types a word ending with punctuation, or just punctuation (for example, `word.` or `.`, `!`, or `?`).

{% hint style="info" %}
We do not store your sentence history. Once a sentence is complete, it gets published to the channel of your choice and gets permanently deleted from our database. We only store sentences that are underway in order to be able to publish them once they're complete. We only store the messages from the dedicated writing channel that PixxieBot reacts to with a green check mark like in the demo below.
{% endhint %}

{% hint style="warning" %}
Kicking PixxieBot from your server will also permanently delete all sentence data associated with it.
{% endhint %}

![This is a live demo of the game in action.](../.gitbook/assets/makeasentence\_demo.gif)

## Setup

### 1. Requirements

Before you start, there are a few requirements:

* Create a dedicated channel where your members will write their sentences. This channel cannot be used for anything else. You can name the channel whatever you want.
* Decide where you want the finished sentences to be published. This can be anywhere (some common choices are in general chat, or in another dedicated channel so they can all be found again easily, or in the sentence-writing channel itself).
* Check PixxieBot [has the correct permissions](../setup/setting-up-the-bot/granting-permissions.md#required-text-channel-permissions) in those channels.

### 2. Setting up the Make A Sentence game

![This is a live demo of the explanation below.](../.gitbook/assets/makeasentence\_setup.gif)

1. Run the `-sentence` command in any channel where PixxieBot has permissions.
2. PixxieBot will ask for the name of the channel where members will write their words. Simply type the name of this channel in chat (for example: **#make-a-sentence**).
3. Then PixxieBot will confirm that choice and ask you for the name of the channel where the finished sentences should be posted. Simply type the name of this channel in chat (for example: **#finished-sentences** or **#general-chat**).
4. The setup is complete. PixxieBot will post a confirmation message in the setup channel with the links to the two channels you chose. PixxieBot will also post explainers for your members in each channel.&#x20;

{% hint style="info" %}
To abandon setup, just leave the channel idle for 15 seconds. The command will time out due to inactivity.
{% endhint %}

## Deleting or editing words

It is not currently possible to delete or edit words that PixxieBot has reacted to with a green check mark.

If you would like this feature to be added in the future, please upvote [this suggestion](https://discord.com/channels/675991746856878082/676105287656275968/798286958794899526) in our [support server](https://pixx.ie/support).

## Changing channels

To change the channels where your sentences get written or published, just run the `-sentence` command again and choose the channels you want to use.

{% hint style="info" %}
No data will be lost in this process. Any ongoing sentences will be continued in the new channel.
{% endhint %}

## Removing the Make a Sentence game from your server

If for any reason you would like to permanently remove the Make A Sentence game from your server and wipe all your server's sentence data from our database, use `-sentence delete`.&#x20;

{% hint style="danger" %}
Running this command will permanently delete the following information from our database:

* Your server ID.
* Your writing channel ID
* Your finished sentences channel ID.
* Any sentence that's underway in your server.
* The user ID of the last user to post a word in the writing channel.
* Your server's total sentence count from our database.
{% endhint %}

{% hint style="warning" %}
Kicking PixxieBot from your server will also permanently delete all sentence data associated with it.
{% endhint %}
