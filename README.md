# okashii-karuta
可笑しいカルタ - Japanese version of "Apples to Apples" or "Cards against Humanity"

"Cards against Humanity" is more well known, but I made Okashii Karuta more kid-friendly like "Apples to Apples". You might still be able to combine question and answer into a double-entendre, but nothing should be naughty on its own.

These PDFs -- one card face per page -- were the basis of a deck I build using MakePlayingCards, as a conversation and learning toy for our Japanese meetup. Printing one pack for yourself will cost more than 60 USD.

Your printing service may require individual image files. Here's how to do that:

* install ghostscript
* run: ``gs -dNOPAUSE -sDEVICE=png16m -r2400 -sOutputFile=page%03d.png name-of-multi-page-card-file.pdf``

To make multiple copies of an image such as aback-001.png: ``for i in `seq 1 186\`; do cp answer.png backs-186-48/aback-$(printf '%03d' $i).png; done``
