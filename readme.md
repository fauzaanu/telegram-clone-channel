# Telegram Clone Channel

Telegram user bot to clone messages from one channel to another.

The cloning is done after downloading the message and uploading it to the target channel. This means it is possible to
clone messages from channels that do not allow forwarding.

---

### Usage

In the same directory you run the application from create a file called `.env` with the following content:

```
API_ID: Your Telegram API ID
API_HASH: Your Telegram API Hash
MON_CHANNEL: The ID of the channel to monitor and forward messages from
TARGET_CHANNEL: The ID of the channel to forward messages to
```

### Where to get each item

`API_ID` and `API_HASH` can be obtained by creating a Telegram application at https://my.telegram.org/apps

`MON_CHANNEL` and `TARGET_CHANNEL` can be obtained by forwarding a message to @jsondumpbot and getting the `chat_id`
from the JSON response that is related to the channel.

> `MON_CHANNEL` is the channel you are monitoring for new messages.

> `TARGET_CHANNEL` is the channel you are forwarding messages to. (Your own channel)

## Limitations

Currently supports simply between two channels. (Because I made this for a specific use case)

### TODO
- [ ] Add support for multiple channels
- [ ] UI ?
- [ ] Improve CLI