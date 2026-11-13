# whatsapp-chat-to-pdf

Convert a WhatsApp chat export (`_chat.txt`) into a clean, printable HTML file, then save it as PDF from your browser. Offline, no upload, one Python file, no dependencies.

Works with iPhone (`[dd/mm/yyyy, hh:mm:ss] Name: text`) and Android (`dd/mm/yyyy, hh:mm - Name: text`) export formats, multi-line messages, 12h and 24h clocks.

## Usage

1. In WhatsApp: open the chat, then *Export chat* (without media). You get `_chat.txt` (inside a zip on iPhone).
2. Run:

```bash
python3 whatsapp_to_html.py _chat.txt > chat.html
```

3. Open `chat.html` in a browser and use *Print > Save as PDF*.

## Need it as evidence?

For court, HR, insurance, landlord or police files, the free script is not enough: you usually need numbered messages, a cover sheet, page numbers and a hash so the document can be shown to be unaltered.

**[ChatExhibit](https://martincrescenzo-dotcom.github.io/chatexhibit/)** does that in the browser (nothing is uploaded): numbered transcript, cover sheet, page "x of y", SHA-256 of the original export. Also supports Telegram, Signal, Messenger, Instagram, Discord, Slack, Google Chat, LINE and KakaoTalk. Preview free, €9 one-time for the full PDF.

## License

MIT

See also: [telegram-chat-to-pdf](https://github.com/martincrescenzo-dotcom/telegram-chat-to-pdf), [discord-chat-to-pdf](https://github.com/martincrescenzo-dotcom/discord-chat-to-pdf).
