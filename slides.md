% Command-Line Fluency
% John Mark Schofield
% jms@schof.org
% http://schof.org
% This presentation built using BigPY https://github.com/harperreed/bigpy



# Command-Line Fluency:
# How to avoid *Repetitive Strain Injury*
# (How to use the BASH command-line with a minimum of keystrokes and a maximum of speed.)

# This presentation: [schof.org/clfp](http://schof.org/clfp)

# By John Mark Schofield

# [schof.org](http://schof.org)
# [jms@schof.org](mailto:jms@schof.org)
# [@schof](https://twitter.com/schof)

# Shameless Plug: I work at [Citrusbyte](http://citrusbyte.com). It's a great place to work, and we're always looking for great people.

# Let's do this.

# Everybody starts out the same when they learn the command line.
# *I'm typing so much, I must be good at this!*

# ![Cat Typing](typing_cat.jpg "Cat Typing")
# ![Cat Typing](typing_cat.jpg "Cat Typing") Not so fast, kitty!

# Do more with less.
# Get these shortcuts in your muscle memory.

# Build habits using just one of these.
# Then, once you're using that regularly, add another one.
# Don't try to start doing all of these at once.

# ![Juggling Fail](juggling_fail.jpg "Juggling Fail")

# These work in BASH on Linux or OS X. Use a different shell? Some of these *may* work.

# The biggies: (Get that low-hanging fruit.)
# ![Low Hanging Fruit](low_hanging_fruit.jpeg)

# *up-arrow*
# up-arrow is your friend.
# Repeats the previous command.
# Hit it as many times as you like to cycle back through commands.
# Down arrow works too.
# Edit a command, then hit *ENTER* to run it.
# If you're all the way back in history and need to get back to the most recent, use
# *SHIFT-ALT->*
# If you use a Mac desktop, you'll need to click the checkbox in your Terminal preferences for "use alt as meta key."
# If you use Linux as your desktop, you're probably not listening because you're recompiling your kernel right now.
# Hey now. I kid because I love.

# *Tab*
# *Tab* is your *other* friend.
# Use *Tab* to autocomplete paths, filenames, or anything else BASH can figure out how to autocomplete.
# Hit *Tab* twice to see all the possibilities, if more than one matches what you've typed.

# Seriously, I stand behind people yelling "*Up arrow! Up arrow! Tab! Tab!*" when I see them needlessly re-type stuff.
# (I don't have many friends.)

# *CTRL&nbsp;-&nbsp;r*
# Searches through your history
# Very powerful
# *CTRL-r* then start typing. It will display the most recent match.
# *CTRL-r* again to display the next match.
# Then edit the command, or hit *ENTER* to run it.

<!---
Tell the Fog Creek Remote Support Story.
-->

# Daaaaaaaaaamn.





# *!!*
# *!!* repeats the previous command.
# So does up-arrow. So this is useless.
# ![Or is it?](or_is_it.jpg "Or is it?")Or is it...
# How many times have you done this?
    rm&nbsp;/var/cache/foobar
# ![Sad clown](sad_clown.jpg "Sad clown") Permission Denied.
# ![Sad clown](sad_clown.jpg "Sad clown") You should have typed "sudo".
# What do you do?
# *sudo&nbsp;!!*
# Hell yeah!


# Changing Directories
# *cd ~* switches to your home directory. BORING. Everyone knows that.
# *cd -* switches to the last directory you were in. Excited yet?


# You SSH'd to a server, but don't remember which one?
# *history&nbsp;|&nbsp;grep&nbsp;ssh*

# Use aliases for common commands. (Put them in your .bashrc or .profile in your ~.)
# alias ll='ls -Flah'



# Editing the current command.
# Backspace is *not* your friend! Backspace thinks you wear funny shoes!
# *CTRL-a* to go to the beginning of the line
# *CTRL-e* to go to the end of the line
# *CTRL-w* to kill the word before the cursor
# *CTRL-k* to clear the line after the cursor
# *CTRL-u* to clear the line before the cursor
# *ALT-f* and *ALT-b* move forward and back one word
# *CTRL+SHIFT+-* (CTRL-Underscore): Freaking *undo*!
# *CTRL-xx* to toggle between the current cursor position and the start of the line.
# These are based on *Emacs*. If you want you can use Vi keybindings: *set -o vi*. Bring back correct (cough) keybindings with *set -o emacs*.


# *find* is your friend.
# (Actually, I guess I have a lot of friends.)
# Want to remove all .svn directories from a tree?
# *find . -type d -name ".svn" -exec echo rm -rf {} \;*
# Remove the "echo" when you get serious.




# Know a trick I missed? Send it to me! *jms@schof.org*
# Thank you!

