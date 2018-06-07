
Execute Script Packed Extensions Local Files Chrome 67
======================================================

Ever since Chrome v67 `chrome.tabs.executeScript` does not work on local files (e.g., file:///foo.index.html) for packed extensions with the `activeTab` permission.

It leads to a `chrome.runtime.lastError` error of:

> Cannot access contents of the page. Extension manifest must request permission to access the respective host.

This was first reported by various folks using the beta version of Chrome. I have since experienced it running:

*   Version  67.0.3396.79 (Official Build) (64-bit)
*   Mac OS X 10.13.2
