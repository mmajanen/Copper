Copper (Cu) CoAP user-agent
===========================

Implements [RFC7252](http://tools.ietf.org/html/rfc7252)

Also see [Copper (Cu4Cr)](https://github.com/mkovatsc/Copper4Cr)

A Firefox add-on to browse the Internet of Things
-------------------------------------------------

### How to integrate the Copper sources into Firefox:
0. Copy the .xpi file to your Linux computer, then select Tools – add-ons – install from file in Firefox. You may have to allow unsigned add-ons by opening about:config and setting xpinstall.signature.required to false. If everything works, skip the rest of the steps. (MiM)

1. Get the sources from Github: `clone git://github.com/mkovatsc/Copper.git`
2. Add a text file named `copper@vs.inf.ethz.ch` to your extension directory of your profile:
 - Windows: `C:\Users\<username>\AppData\Roaming\Mozilla\Firefox\Profiles\xxxxxxxx.default\extensions\`
 - Linux: `~/.mozilla/firefox/xxxxxxxx.default/extensions/`
 - MacOS: `~/Library/Application Support/Firefox/Profiles/xxxxxxxx.default/extensions/`
3. Write the path to the Copper sources (i.e., the directory that contains `install.rdf` and `chrome.manifest`) with (back)slash at the end to the file (e.g., `D:\Projects\Git\Copper\`).
4. Since Firefox 43 you need to **allow unsigned add-ons** by opening [about:config](about:config) and setting `xpinstall.signatures.required` to false.
5. Restart Firefox.
6. Optionally use [about:config](about:config) with the filter "copper" to clean up old configurations.

Copper should show up in the add-ons list. You can now enter CoAP URIs (e.g., [coap://californium.eclipse.org/](coap://californium.eclipse.org/)) into the address bar and will have a user interface to interact with the CoAP resources on a server. The detailed log output is available through the rectangular button on the top right, next to the preferences button.

### See also:

 - [Setting up Extension Development Environment](https://developer.mozilla.org/en/setting_up_extension_development_environment)
 - [Firefox Profile Manager](https://support.mozilla.org/en-US/kb/profile-manager-create-and-remove-firefox-profiles)
 
