# PyHero 2
A ~~terrible~~ great Guitar Hero III clone made in PyGame

This was made based on [Nethermaker's PyHero](https://github.com/Nethermaker/PyHero) and I had to deal with some old code messing around with me

Thanks to ChatGPT I was able to solve the issues made by Nethermaker way back almost **FIVE YEARS AGO**

Some features include:
* The ability to load almost any chart from GH3, albeit with modifications required
* Controller support (only tested with XBox 360 Xplorer guitar)
* Those are the only two features that are even semi-remarkable
* Mostly un-commented code

If you want to check HIS test, I *highly* suggest watching [this video](https://www.youtube.com/watch?v=MeYfBIGKki8) instead of trying to run it yourself. I have ONLY tested it on Python 3.11, with the PyGame build included in the dependencies folder. You also need to put `pygbutton.py` (also in the dependencies folder) in the same folder as `PyHero.py`. Also of note is that I haven't included any music files, since I would probably be breaking some sort of copyright laws if I did. If you're really desperate for some free guitar hero action, I'd recommend checking out [Clone Hero](https://www.youtube.com/channel/UCc3IfdqGZjhdgQbi_EpfuYg) instead.

I don't intend to ever work on or update this project again. I made some mistakes early on when creating this that would essentially require me to rewrite most of the program if I wanted to develop it further. These include:
* All the calculations I do are framerate-dependent, while the audio continues to play at the same rate regardless of framerate. This means that audio is practically guaranteed to desync if the chart that you are playing is not fiddled with extensively, and the changes needed (namely to the `divisor` value) will vary from computer to computer. 
* I did not fully understand how Guitar Hero calculates note positions based on info in the charts. Namely, I decided to try and ignore tempo, which was a very bad idea. Any song with a tempo change will end up desyncing from the audio 100% of the time, and there is nothing you can do about it.
* Probably more that I can't think of

This is a secondary project aside from my main project, write side stories for a DDLC Mod :)

You can modify this if you want
:D
