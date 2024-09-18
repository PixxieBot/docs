# Run Discord Giveaways using Hangry Games

## What is Hangry Games?

Hangry Games is a tongue-in-cheek parody on the Hunger Games franchise, with a slightly sadistic food theme.

Sign up to a game with your friends, volunteer as a tribute, and sit back and watch you slaughter each other with creative food themed attacks.

May the odds be ever in your flavor!

## Giveaway Mode

{% hint style="info" %}
Giveaway mode is currently in open beta, which means we're actively working to improve it and add more functionality in the future. If giveaway mode doesn't have a feature you'd love to see, feel free to [reach out in our Discord server](https://pixx.ie/invite?ref=docs_hg_giveaways) to share your feedback and suggestions!
{% endhint %}

Many Discord servers use Hangry Games for giveaways. This is why we've created a separate giveaway mode to allow users to have more control over the conditions in which giveaways are run.

To start a giveaway, use the `/hangrygames giveaway` command.

### Command Options

The `/hangrygames giveaway` command has some extra parameters compared to your classic casual game of Hangry Games in order to allow you to customize the game.

- `prize:` All giveaways require a prize to be entered in order to create the giveaway.
- `sponsor:` (optional) If the prize is sponsored by an individual, for example, `@John` if John wants to give away some stickers for Monopoly Go. If you don't set a sponsor then only the prize for the giveaway will be shown in the signup and winner messages.
- `feasts:` (optional, defaults to `False` if not set) Determines whether your giveaway should include [Feasts of the Dead](./in-game-events.md#feasts-of-the-dead). This is off by default in Giveaway mode since most servers prefer to exclude feasts from their giveaways due to their voting. If you start `/hangrygames giveaway` without setting this `feasts` parameter, feasts will not show in your game. If you **do** want feasts in your giveaway, set this parameter to `True`.

{% hint style="info" %}
If a sponsor is set, they will be asked to confirm if they want to join the giveaway as a tribute in order to prevent accidental joins. Please note that once a sponsor enters their own giveaway, they cannot be removed from the list of tributes, similarly to other players.
{% endhint %}

## Launching Hangry Games in Giveaway Mode

To start the giveaway, simply click the fork and knife emoji button in the signup message as you would for a regular round of Hangry Games. The game will run, just like a regular round of Hangry Games but with feasts disabled unless you opted-in to allow feasts when running the `/hangrygames giveaway` command for signup.

{% hint style="info" %}
Please note that Burger Masters cannot start Hangry Games in Giveaway mode. Only the giveaway organiser (the user who ran the initial `/hangrygames giveaway` command) or a server member with `Manage Server` permissions can start a giveaway.
{% endhint %}
