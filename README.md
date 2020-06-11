# Apps.Dialogflow-develop-gsoc

This Dialogflow Livechat connector app is modified to support custom payloads for message-action responses. Connector apps uses the payload from Dialogflow and sends message action buttons as attachments to the Live Chat widget.

## Sample Custom Payload

![](https://user-images.githubusercontent.com/41849970/84405117-5bac3000-ac25-11ea-8263-3b3bfa330944.png)

```
{
  "actions": [
    {
      "type": "button",
      "msg": "getSessionId",
      "msg_processing_type": "sendMessage",
      "text": "Contact Salesforce Agent",
      "msg_in_chat_window": true
    },
    {
      "text": "Send Random String",
      "msg_in_chat_window": true,
      "type": "button",
      "msg_processing_type": "sendMessage",
      "msg": "randomWord"
    },
    {
      "msg_processing_type": "sendMessage",
      "msg_in_chat_window": true,
      "msg": "closeChat",
      "text": "Close Chat",
      "type": "button"
    }
  ]
}
```

