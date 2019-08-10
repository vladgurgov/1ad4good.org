# One Ad for Good 

## 1ad4good.org 

index
You can make a difference. One ad at time. 

If you are are serving ads on your site chances that you have some unsold impressions. Fill them with love.
Serve free ads that make a difference. 

## What is it? 

**One Ad for Good** is a [Prebid.js](https://prebid.org) Header Bidding Adapter that serves free ads for imprtant causes on your site.

### What kind of ads are you running?

We get public service advertising from orgs like [www.psacentral.org](https://www.psacentral.org), [www.adcouncil.org](#https://www.adcouncil.org), various non-profits. People can contribute their ads directly to our open source header bidder.

We are currently supporting 300x250 banners and video

### Ads are the worst! You are tracking my data!

No we are not. Our open source [header bidder](https://github.com/vladgurgov/header-bidder) doesn't collect any data and our creatives don't have any tracking either. You can check it by yourself.

### Who is paying for these ads?

All of our ads are 100% free for publishers. Publishers should not expect any payments for running these campaigns, but they don't pay for ad serving either. However ad serving is not free. Currently we are supported by our donors, if your organization can support this project - please consider helping us

### So how do I test your wonderful ads?

Real simple. Just add this one line to your prebid.ord config and make sure you have our adapter in it. (see [Prebid.js](https://prebid.org) for details on prebid configuration. You just need to add our bidder '1ad4good' along with other bidders in your setup. 

You might need to download a newer version of prebid.js with our adapter included: [Prebid Download](http://prebid.org/download.html)
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

### Are you Non-Profit?
We are just getting started as a hobby project and not incorportated yet. We are sponsored by one individual and his businesses. If this will gain momentum we will be incorpotating as a Non profit.

### How can I support this project?

- Consider placing our ads on your sites( we only take inventory that is otherwise unsold to advertisers), 
- Contribute to this project and our open-source [header bidder](https://github.com/vladgurgov/header-bidder). We review all PRs as soon as we can - typically within couple days.
- If you are hosting company consider donating servers for our bidders/content delivery
- Interested in sponsoring this project - please get in touch vlad@aaaudi.com