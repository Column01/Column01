### Hello, My name is Colin. 
I'm a software developer from Ontario, Canada who specializes in Python development. Below you will see a few pinned repositories, these are my favourite projects I've worked on and are good examples of the code I am capable of writing.

### Projects I am working on/maintain

- [mark2](https://github.com/gsand/mark2) (maintainer) - Minecraft server wrapper written in Python 3 using Twisted

### Favourite Project
My favourite project is my discord moderation bot that uses class loading to allow a user to make the bot their own. Simply adding scripts to a folder with some command or event handler classes allows the user to add to the bot without even restarting the program!

The event handlers are added to the main script using python "reflection" and some clever techniques that enable my code to be an order of magnitude smaller compared to implementing each event function. It takes some info provided by the handler class and [creates a function in the bot](https://github.com/Column01/Discord-Moderation-Bot/blob/master/event_registry.py#L63-L94) using a [template](https://github.com/Column01/Discord-Moderation-Bot/blob/master/bot.py#L46-L56) renamed `on_<event>`. Effectively ~40 lines of code can handle what could have been upwards of thousands of lines and is completely future proof. When new events are added, I don't even need to write any new code to handle their addition.
