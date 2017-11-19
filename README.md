# ReminderFather

_Plugable Reminder to connect with different apps_

ReminderFather is an idea of create a piece of software that listen to manual input events and connect with multiples services. It' s something like the Slack's `/remind` command but in your browser, your phone, etc.

I think `recordium` (https://github.com/facundobatista/recordium) it's a great idea but it's just an example, not a real program. It works, but it's not polished and it misses a lot of features that I consider important.

I would like to have these features:

* When you are navigating a Issue on Github, have the same behaviour than in Slack `Remind me about this in` with a couple of options. So, you read an issue in Github right now, but you already know that the solution won't be in the next month and you don't want to forget to take a look in two month from now.

* Once you send a reminder to the app, it would check the metadata of event (URL, Website, Name, Hour, GPS, etc) and will decide which method of reminder this event should be: email, SO notification, Telegram message, recordium light, Slack message, or another and will send them when the reminder happens

* Each of the this type of notifications should be a plugin and can be enabled/disabled depending on each user

* Systray icon with a persistent color when there are messages unread


## Integration with your phone

I think this can be handled by a Telegram bot and the "Share" option in most of the applications. The Telegram bot will receive a message and will decide what to do with it.

I'm thinking this as a first approach. For example, after sharing the YouTube video with your bot you send a text message with the command `/remind me in 10 minutes` or you can even send an audio saying that and use a third party voice recognition to set the reminder properly.

## Integration in the browser

We will probably need an addon that adds an icon next to each of the element that we want to be able to have a reminder (Github issue, for example)
