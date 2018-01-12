---
layout: page
title: "iCloud Drive + Backblaze"
subheadline: ""
teaser: "Using iCloud Drive with zero-knowledge client-side encryption, and Backblaze for unlimited encrypted cloud backup."
author: Morgan
categories:
  - tech
image:
    title:
    homepage:
    thumb:
    caption:
    caption_url:
breadcrumb: true
comments: true
---
![](https://imgur.com/pEDSdXL.jpg)

Last year I wrote a [post]({{ site.baseurl }}/tech/2016-10-03-Cloud-Storage) detailing my solution for zero-knowledge unlimited cloud backup. The solution was reliant upon [Amazon Cloud Drive](https://amazon.com/clouddrive) for storage, [ODrive](https://www.odrive.com/) for sync, and [Boxcryptor](https://www.boxcryptor.com/en/) for client-side encryption of content before it was uploaded to the cloud.

#### The End

This three-pronged backup solution was excellent for a long time. I've been very happy with Boxcryptor, especially as its mobile app has improved significantly since that original blog post. Like all good things, this solution had to come to an end - specifically because Amazon [killed](https://twitter.com/morganspeck/status/874716152680902656) the 'unlimited' storage option for Cloud Drive at the beginning of this year. ACD moved from $60/year to $60 per _terabyte_ per year. This pricing is still extremely competitive, but not budget friendly for me. I have a media server with  ~8TB of content, if I'd stayed with Amazon my yearly bill would be nearly $500 a year! It was time to change providers, and I needed something for both backup, and day-to-day cloud storage.

Fortunately, I was able to find an alternate solution: [Backblaze](https://secure.backblaze.com/r/01ky72) & [iCloud Drive](https://www.apple.com/icloud/icloud-drive/). I had initially hoped to find some other vendor who could give me a single unlimited platform for storage + backup. There are options out there, but none of them were practical for what I wanted - namely ease of using while mobile. In the end it was necessary to use two different providers to achieve what I wanted. 

#### iCloud Drive

I ended up deciding to roll all my day-to-day storage needs into iCloud drive. The $2.99/month plan is very competitive, offering 200GB of storage. iCloud drive has come a long way since I tried it out as a cloud storage solution a few years ago. The sync is now fast, and reliable. Boxcryptor is also compatible with iCloud drive, so I was able to continue using that to encrypt my content before it was uploaded to the cloud.

#### Backblaze  

Backblaze offers several cloud-storage and backup solutions. Their [B2](https://www.backblaze.com/b2/cloud-storage.html) service is comparable to Amazon's [S3](https://aws.amazon.com/s3/) offerings, and they've got a great consumer product that is billed as 'unlimited backup, including external hard drives, for only $5/month'. B2 is in many ways focused on business clients - those who will be uploading and downloading a lot of content regularly. For the backup needs on my media server, I only ever plan on downloading data in the event of a total drive failure, so I opted for the $5 backup product instead.

Backblaze bills their backup service as unlimited, but I figured that at a cost of a mere $5/month it was too good to be true. It turns out, they mean what they say. It really is only $5/month, and it really is unlimited. I've been using Backblaze for several months now, and have thus far uploaded multiple terabytes. With as much content as I have, and with limited upload speed (10 megabits), I'm actually still performing the initial backup. Backblaze's UI is pretty easy to use. Following installation there is a preference pane in System Preferences. From there you can configure which drives you want backed up (yes, they'll also backup your external drives as long as they're connected at least once a month), what you want excluded, and how much upload speed you want to use. The preference pane is a set-it-and-forget-it deal. Once you get the initial backup going, Backblaze's client just does its thing, there's no need to think about it.

For a security wonk like me, moving to a platform like Backblaze was a big leap. They offer very [good security](https://www.backblaze.com/backup-encryption.html) though. By default, all content uploaded is encrypted in transit. There is also the option to set your own [custom key](https://www.backblaze.com/backup-encryption.html) so that content is encrypted at rest, unreadable by Backblaze. Naturally, as with any encrypted platform, you have to place trust in the provider that the security claims they make are true. I'm still wary that Backblaze might have some way of seeing content at rest, but I'm mostly trusting.

In the event that one _does_ need to recover data from a Backblaze backup, they offer several options. One can download files that need to be recovered using their web interface, or there is an option to have a drive (up to 4TB) shipped to you. With the drive option, there is a [$190](https://www.backblaze.com/restore.html) fee, but Backblaze says they'll refund that to you if you return the drive back to them after you've gotten what you need off of it. I'm not quite sure how they handle situations where you need _more_ than 4TB of data recovered - I can't imagine too many of their customers have that much data backed up. I'd assume that they just ship multiple drives. I hope I never need to find out.

If you want to try backblaze, they have 1 month trials available [here](https://secure.backblaze.com/r/01ky72).

**Full Disclosure:** This is not a sponsored post. The above link is a referral link. In the event you sign up for Backblaze using this link, I will receive 1 free month of service.

---
<p align="right">Typed on Kinesis Advantage</p>
