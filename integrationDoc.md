# Connect your web app or product
## Option 1. Code snippet (Recommended)

Just add this snippet to your website and we'll automatically capture page views, sessions and all relevant interactions within your website. Learn more.

### Install the snippet

Insert this snippet in your website within the <head> tag.

 <pre>

   <script>

    !function(t,e){var o,n,p,r;e.__SV||(window.posthog=e,e._i=[],e.init=function(i,s,a){function g(t,e){var o=e.split(".");2==o.length&&(t=t[o[0]],e=o[1]),t[e]=function(){t.push([e].concat(Array.prototype.slice.call(arguments,0)))}}(p=t.createElement("script")).type="text/javascript",p.async=!0,p.src=s.api_host+"/static/array.js",(r=t.getElementsByTagName("script")[0]).parentNode.insertBefore(p,r);var u=e;for(void 0!==a?u=e[a]=[]:a="posthog",u.people=u.people||[],u.toString=function(t){var e="posthog";return"posthog"!==a&&(e+="."+a),t||(e+=" (stub)"),e},u.people.toString=function(){return u.toString(1)+".people (stub)"},o="capture identify alias people.set people.set_once set_config register register_once unregister opt_out_capturing has_opted_out_capturing opt_in_capturing reset isFeatureEnabled onFeatureFlags getFeatureFlag getFeatureFlagPayload reloadFeatureFlags group updateEarlyAccessFeatureEnrollment getEarlyAccessFeatures getActiveMatchingSurveys getSurveys".split(" "),n=0;n<o.length;n++)g(u,o[n]);e._i.push([i,s,a])},e.__SV=1)}(document,window.posthog||[]);
    posthog.init('phc_ySCF4YinUf6DxprJ5B0jXtzgijeTqFkWPsIIfC3yTrC',{api_host:'https://e.abla.io'})

</script>

</pre>

### Send events

Visit your site and click around to generate some initial events.

## Option 2. Javascript Library

Use this option if you want more granular control of how PostHog runs in your website and the events you capture. Recommended for teams with more stable products and more defined analytics requirements.

### Install the package

<pre>
npm install ablaevent-js
# OR
yarn add ablaevent-js
# OR
pnpm add ablaevent-js

</pre>

### Configure & initialize 

<pre>
import posthog from 'ablaevent-js'

posthog.init('phc_ySCF4YinUf6DxprJ5B0jXtzgijeTqFkWPsIIfC3yTrC', { api_host: 'https://e.abla.io' })

</pre>