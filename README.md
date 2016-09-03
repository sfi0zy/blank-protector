![](https://habrastorage.org/files/12c/cb3/88e/12ccb388e1bd4edbb837176aabac2073.png)

When we click on link with target="_blank", a new page in a new tab can change our previous page on the previous tab. To avoid this effect, we can use rel="noopener" but too many websites not using this ability yet. And we can't affect them. This is a very simple Google Chrome extension that does only one thing: sets window.opener on every page to null before page loading is started. Despite the fact that websites use rel="noopener" or not (by the way Google search doesn't use it) we can keep calm - without window.opener this attack can't affect us.

**Intallation instructions**

 - Clone this repository or download zip version and unpack it
 - Go to chrome://extensions/
 - Enable "Developer mode"
 - Click "Load unpacked extension" and load it from the directory where you clone this repository
