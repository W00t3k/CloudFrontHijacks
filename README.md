Original post for more information: https://medium.com/@vysec.private/cloudfront-domain-hijacks-under-attack-c15c64607b7c

Disclaimer: No information on any of my repositories should be used for unlawful purposes. All information I publish is to aid and assist the cyber security industry's growth and assist in protection of organisations and individuals.

Note: I am not putting you at further risk that you already are by putting it on GitHub to help you identify it. The attackers / third party have already taken control over an instance that can control your domain name. If you want your domain removed, get in contact with me.


When a CloudFront customer uses the service, but later removes it from their account, it leaves a CNAME record in their Domain. An attacker can go ahead and register that CloudFront CNAME and obtain the necessary access to "hijack" the domain involved and serve content under that domain.

This repository is released to the public. As of 27 March 2018, I found that a large number of the domains had been "reserved" and no longer hijackable. This indicates that an entity had performed similar enumeration and identified this list and took action to weaponise and attack all of these domains, but had not released any public information. The instances had not been activated yet at this point in time but whoever has took control over all of these CNAMEs could "flip the switch" and serve malicious content at any time of their choosing.

I am releasing this list so that the public can check whether they are likely to be suspectible. If not, you should still check that there are no dangling CNAME records pointed to abandoned CloudFront instances. If you are on this list, you should remove your CNAME record immediately if you do not have control over the corresponding CloudFront instance with the matching CNAME.