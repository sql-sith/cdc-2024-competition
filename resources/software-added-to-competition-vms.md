# Software added to competition VMs

I had to add some software to competition VMs that was not part of the scenario requirements and I though I should make a note of that in a central place.

## AD Server

1. MS Edge

   I needed a browser that could function. Since Microsoft apparently can't remove IE (yet), they really make it hard to use. The make it a lot easier to get to the Edge installation page than to get to the others, so that's what I installed. I needed this to use VirusTotal while I investigated Tristan's observation about the DNS service being bound to many ports. For some reason, I could not copy the file hash from the VM to my local machine, so I decided to use a local browser to look up the hash on VirusTotal instead.

2. `sigcheck`

   This was also needed as part of my investigation of the DNS service on the AD server. After verifying that no antivirus software flagged the local copy of `dns.exe` as malware, I still had to validate that it was actually from Microsoft. `sigcheck` from sysinternals (which is owned by Microsoft) let me validate that the file was properly signed by Microsoft.
   
