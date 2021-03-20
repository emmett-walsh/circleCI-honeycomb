# Instrumenting CirclCI builds with honeycomb

I wanna experiment with getting traces from CI using honeycomb's public orb.

## What I did

1. I signed up for a [free honeycomb plan here](https://ui.honeycomb.io/signup?utm_source=product-trial-page&utm_medium=get-started-cta-self&utm_campaign=trial) (the sign up process ends on a page which shows you your honeycomb API key).
2. I created this repo and activated the corresponding project in CirclCI.
3. I followed [the README instructions in the orb repo](https://github.com/honeycombio/buildevents-orb). (At the bottom of the page there are links to several honeycomb repos which claim to make use of buildevents but not all of them do. [This is the one](https://github.com/honeycombio/libhoney-go/blob/master/.circleci/config.yml) I found to be most useful)

You'll see in the circle config that I used `sleep` statements to simulate the time it would normally take to actually build and test your code. The orb README has more realistic examples.
