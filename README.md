# Browsersync wants my <body>

I find that Browsersync does not get injected automatically when there is not `<body>` tag is not in the HTML file. With my use-case, I am live-editing lots of HTML partials, which do no contain body tags, so this is awkward to have to inject a `<body>` tag when the system knows I'm editing a partial, and not inject a `<body>` tag when I'm loading a full page.

## Instructions

1. `git clone git@github.com:f1lt3r/browsersync-body-demo.git`
1. `cd browsersync-body-demo`
1. `npm install`
1. `browser-sync start -s --startPath test-working.html`
	1. Check Browsersync works with a `<body>`
1. `browser-sync start -s --startPath test-broken.html`
	1. Check Browsersync fails without a `<body>`


