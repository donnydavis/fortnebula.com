---
layout: post
title:  "OpenStack and IPv6"
date:   2016-09-22 12:00 -0500
categories: articles cloud openstack
---
<img class="img-responsive" style="float: right;" src="/assets/blog/img/openstack.jpg">
OpenStack can do some pretty cool things. For someone who is network savvy, ipv6 is a pretty popular topic.


So to get more down to the point, my public openstack will not create a floating IPv6 address for you. You will get a whole IPv6 subnet thanks to the bgp speaker plugin for neutron.

This thing is just plain awesome. My edge router advertises the subnet you create in neutron, and then all of your machines are available on an ipv6 subnet for direct access. The coolest part is the security group rules still work, so you get all the benefits of ipv6 with a lot less worry.

My next post will be a write-up on how to do it
