# This fork will be an updated version of the userscript with some improvements. The plans are to add password hashing to make the script more secure, as well as to add support for TOTP. I am also looking at replacing bw with rbw.

## How to install

- Install [Bitwarden CLI](https://bitwarden.com/help/article/cli/) with the command `brew install bw`. Then you have to login before using the user script. Run in terminal `bw login`

- Install [Choose Gui](https://github.com/chipsenkbeil/choose) with the command `brew install choose-gui`

### Intel macs

- Install pip packages: `pip3 install osascript` and `pip3 install tldextract`

### M1 macs

***There seems to be issues if you have both intel and m1 version of homebrew installed***

---

The problem is the qutebrowser uses the `/usr/local/bin/python3` version of python and you can also have python3 install
on `/opt/homebrew/bin`. So I just installed the  `pip3 install osascript` and `pip3 install tldextract` in both `/opt/homebrew/bin/pip3` and
on the `/usr/local/bin/pip3`. You can also just try the `/usr/local/bin/pip3` version. Mine was on the /usr/local/bin. But if that doesn't work you can try to install it on `/usr/bin/pip3`


### Installing for qutebrowser

- Copy bitwarden script to `$HOME/.qutebrowser/userscripts`

Then when you are in a page run `spawn --userscript bitwarden` 

And that's all folks 

![image](https://media1.tenor.com/images/03e054d9928b5137884289352d9ae9cb/tenor.gif)
