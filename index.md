---
title: One Ad For Good
description: Prebid.js header bidder adapter for free ads.
---

# [1ad4good.org](http://1ad4good.org) 

You can make a difference. One ad at time. 

## What is it? 

If you are are serving ads on your site chances that you have some unsold impressions. Fill them with love.
Serve free ads that make a difference. 

**One Ad for Good** is a [Prebid.js](https://prebid.org) Header Bidding Adapter that serves free ads for imprtant causes on your site.

### Usage

Using our adapter is really simple. I takes adding just one like in ad unit config javascript(see [Prebid.js](https://prebid.org) for details on prebid configuration. You just need to add our bidder '1ad4good' along with other bidders in your setup. Bidder params are the same as popular appnexus bidder -you can pass placementId, etc

```javascript
    var adUnits = [
        {
            code: '/19968336/header-bid-tag-0',
            mediaTypes: {
                banner: {
                    sizes: div_1_sizes
                }
            },
            bids: [{
                bidder: '1ad4good',
                params: {
                    placementId: 13144370
                }
            }]
        }
    ];
```
You might need to download a newer version of prebid.js with our adapter included: [Prebid Download](http://prebid.org/download.html)

Please keep in mind that bidder will return bid with $0.10 CPM by defaul. We do that to match default medium bid granularity ($0.10) (prebid.js does not like $0 bids and removes them, so does DFP line items). If you want bidder to return custom CPM you can pass it on:
```javascript
    var adUnits = [
        {
            code: '/19968336/header-bid-tag-0',
            mediaTypes: {
                banner: {
                    sizes: div_1_sizes
                }
            },
            bids: [{
                bidder: '1ad4good',
                params: {
                    placementId: 13144370,
                    cpm: 0.50
                }
            }]
        }
    ];
```
Its up to your configuration, but please remember that, despite any bid responses, **all of our ads are always free**
### What kind of ads are you running?

We get public service advertising from orgs like [www.psacentral.org](https://www.psacentral.org), [www.adcouncil.org](https://www.adcouncil.org), various non-profits. People can contribute their ads directly to our open source header bidder.

We are currently supporting 300x250 banners and video

### Ads are the worst! You are tracking my data!

No we are not. Our open source [header bidder](https://github.com/vladgurgov/header-bidder) doesn't collect any data, leaves no cookies and our creatives don't have any tracking either.

### Who is paying for these ads?

All of our ads are 100% free for publishers. Publishers should not expect any payments for running these campaigns, but they don't pay for ad serving either. However ad serving is not free. Currently we are supported by our donors, if your organization can support this project - please consider helping us

### Are you Non-Profit?
We are just getting started as a hobby project and not incorportated yet. We are sponsored by one individual and his businesses. If this will gain any momentum we will be incorpotating as a non profit.

### How can I support this project?

- Consider placing our ads on your sites (we only take inventory that is otherwise unsold to advertisers). 
- Contribute to this project and our open-source [header bidder](https://github.com/vladgurgov/header-bidder). We review all PRs as soon as we can - typically within couple days.
- If you are hosting company consider donating servers for our bidders/content delivery
- Interested in sponsoring this project - please get in touch vlad@aaaudi.com
