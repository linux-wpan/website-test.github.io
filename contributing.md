---
layout: page
title: Contributing
---

## Developing

Current developing repository is [bluetooth-next](http://git.kernel.org/cgit/linux/kernel/git/bluetooth/bluetooth-next.git). All patches should be send to <[linux-wpan@vger.kernel.org](mailto:linux-wpan@vger.kernel.org)\> and based on bluetooth-next.

For wpan-tools checkout the [wpan-tools](https://github.com/linux-wpan/wpan-tools) repository. Also send patches to <[linux-wpan@vger.kernel.org](mailto:linux-wpan@vger.kernel.org)\> for it with a "wpan-tools" tag. The same for [wpan-misc](https://github.com/linux-wpan/wpan-misc).

## Open Tasks

*   rework

    *   missing features in nl802154, crypto etc.
    *   new frame parsing style in mac802154 and ieee802154 based on mac80211 frame parsing design. Draft is [mac802154 rx](https://github.com/linux-wpan/linux-wpan-next/blob/wpan_rework_rfc/net/mac802154/rx.c). Crypto need to be done at first, otherwise I can’t test it.
    *   remove cb context from dev\_hard\_header and introduce generic header generation functions like [header_ops](https://github.com/linux-wpan/linux-wpan-next/blob/wpan_rework_rfc/net/ieee802154/header_ops.c#L80). Here too, crypto need to be done at first.

*   devicetree extended addr setting, draft is here [ieee802154: add usual way to get extended address via device tree](http://www.spinics.net/lists/linux-wpan/msg01503.html)

*   RPL? - not our job, need to go through ipv6 netdev community, but we should do something to have a "started" mainline solution.
*   cleanup/fix 802.15.4 af raw/dgram socket code. We should use bluetooth socket code as example.
*   In wireless exists a "station dump", we need something similar "node dump" with all neighbour nodes and their last LQI value, addresses, etc. information.

## Changing the Website

If you want to take part in developing this website, do the following:

```
git clone https://github.com/linux-wpan/wpan-misc.git
cd wpan-misc/website
git checkout -b myproposal
\# Change this page to whatever you like.
$EDITOR index.txt
git commit -s -a
\# be sure to be registered to linux-wpan@vger.kernel.org before sending the
\# patch
git send-email --to linux-wpan@vger.kernel.org -1
```
Next wait for the reactions on the mailinglist and if your change is integrated.
