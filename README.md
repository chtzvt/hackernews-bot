#hackernews-bot

A bot that grabs a random story from [The Hacker News](https://news.ycombinator.com) and posts it to [Slack](https://slack.com) (or another service of your choice).

You can schedule this script to run at a regular interval, or have it triggred by an interesting event.

Configuration is straightforward, simply edit CONFIG to taste. After that, you can get your HN fix however you like!

```
var CONFIG = {
	"webhook_url": "https://hooks.slack.com/services/<webhook URL here>", // The URL for your Slack webhook (see below) 
	"channel": "#general", // The channel to which the bot will post.
	"bot_username": "HackerNewsBot", // The username of the bot.
	"bot_icon_emoji": ":newspaper:", // The emoji icon of the bot that appears in the chat. 
	"post_color": "#FF6600", // The accent color of the posts (HN Orange by default :) )
	"fallback": "Newsbot: Your automated news aggregator." // The default fallback, should the client be unable to display the messsage.
};
```

For more information about configuring incoming webhooks in Slack, see [the documentation](https://api.slack.com/incoming-webhooks). 
You may also be interested in the [attachment formatting rules](https://api.slack.com/docs/attachments) for the Slack API. 

Enjoy!
