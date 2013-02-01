kb-loops
========
The most low-fidelity soundboard loop machine on the market. Was originally bash but ruby proved faster to prototype.

Starting kb-loops:
- Start the server up: `./kb-loops`
- Now you have a FIFO called `in` which you may send commands to
    * Valid commands are `store`, `samples`, and `play`
    * Storing a sample: `store key,start,end,loops,location`
    * Display loaded samples: `samples`
    * Playing a sample: `play key,loops`

Using the soundboard:
- Start the keyboard soundboard: `./soundboard`
- To play sample named 'a': `a`
- Loop sample named 'b' 10 times: `10b`
- To quit: `\`

Helpful Hints:
- Load list of pre-defined sample `store`s: `cat layouts/progger > in`
- A not REPL, but REL: `tee in`
