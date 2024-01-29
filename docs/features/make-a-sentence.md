# Make A Sentence

## What is Make A Sentence?

Users take turns writing one word each in a dedicated channel to make up a sentence together! PixxieBot publishes the finished sentence once a user types a word ending with punctuation, or just punctuation (for example, `word.` or `.`, `!`, or `?`).

{% hint style="info" %}
We do not store your sentence history. Once a sentence is complete, it gets published to the channel of your choice and gets permanently deleted from our database. We only store sentences that are underway in order to be able to publish them once they're complete. We only store the messages from the dedicated writing channel that PixxieBot reacts to with a green check mark like in the demo below.
{% endhint %}

{% hint style="warning" %}
Kicking PixxieBot from your server will also permanently delete all sentence data associated with it.
{% endhint %}

![This is a live demo of the game in action.](../.gitbook/assets/makeasentence-demo.gif)

## Setup

### 1. Requirements

Before you start, there are a few requirements:

- Create a dedicated channel where your members will write their sentences. This channel cannot be used for anything else. You can name the channel whatever you want.
- Decide where you want the finished sentences to be published. This can be anywhere (some common choices are in general chat, or in another dedicated channel so they can all be found again easily, or in the sentence-writing channel itself).
- Check PixxieBot [has the correct permissions](../setup/setting-up-the-bot/granting-permissions.md#required-text-channel-permissions) in those channels.

### 2. Setting up the Make A Sentence game

1. Run the `/makeasentence setup` command in any channel where PixxieBot has permissions.
2. PixxieBot will ask for the options `writing` & `finished`.
3. Mention the channel you want users to form the sentence in `writing` and Mention the channel where you want PixxieBot to post finished sentences in `finished`
4. The setup is complete. PixxieBot will post a confirmation message in the setup channel with the links to the two channels you chose. PixxieBot will also post explainers for your members in each channel.

## Deleting or editing words

You can delete a word or edit it, PixxieBot will post an embed showing the updated current sentence.

## Changing channels

Run the command `/makeasentence setup` and edit the options.

{% hint style="info" %}
No data will be lost in this process. Any ongoing sentences will be continued in the new channel.
{% endhint %}

## Removing the Make a Sentence game from your server

If for any reason you would like to permanently remove the Make A Sentence game from your server and wipe all your server's sentence data from our database, use `/makeasentence delete`.

{% hint style="danger" %}
Running this command will permanently delete the following information from our sentences database:

- Your server ID.
- Your writing channel ID.
- Your finished sentences channel ID.
- Any sentence that's underway in your server.
- The user ID of the last user to post a word in the writing channel.
- Your server's total sentence count.
  {% endhint %}

{% hint style="warning" %}
Kicking PixxieBot from your server will also permanently delete all sentence data associated with it.
{% endhint %}
