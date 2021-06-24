# CloudyDev

## Updates:
purchased used hardware to start migrating the site off github pages, this will be our metal server to host the website and the basic cloud platform.
I hate dell but they seem to be less worse than HP in terms of exploiting Palestine directly so...
```
https://www.marktplaats.nl

New blazing fast Dell XPS 8940, i7-11700, 16GB, 512GB SSD
Lightning fast dell pc, new in box. 
Separate video card has been removed, 
but there is still a good video card on the motherboard.… 
```
basically a Standard_B16ms with less RAM (that's an easy upgrade down the line that still saves money) or a bit batter than four Standard_B4ms

with storage, premium ssd w/ redundancy costs 125eu/yr per 1 TB, so we can add that as well to bradley since we have a ssd + hdd we can use to do the same thing.

Name | Price | Cores | Threads | Generation| RAM | SSD | HDD | GPU 
--- | --- | --- | --- | --- | --- | --- | --- | --- |
Big Bradley | 558 one time  | 8 | 16 | Rocket Lake 14nm | 16 | 512GB | 2TB | none
1x Standard_B16ms |  3294.55/yr | - | 16 | - | 64 | x | x | none
4x Standard_B4ms | 3293.74/yr | - | 4 | - | 16 | x | x | none

Cloud platforms are computer landlords


Azure's pricing formula for B series:Credits 
```
accumulated/credits used in an hour is equivalent to: ((Base CPU perf of VM - CPU Usage) / 100) * 60 minutes.

For a D16s_v3 which has 16 vCPUs and 64 GiB of memory the hourly rate is $0.936 per hour (monthly $673.92) and for B16ms with 16 vCPUs and 64 GiB memory the rate is $0.794 per hour (monthly $547.86).

Q: How do you get 135% baseline performance from a VM?

A: The 135% is shared amongst the 8 vCPU’s that make up the VM size. For example, if your application uses 4 of the 8 cores working on batch processing and each of those 4 vCPU’s are running at 30% utilization the total amount of VM CPU performance would equal 120%. Meaning that your VM would be building credit time based on the 15% delta from your baseline performance. But it also means that when you have credits available that same VM can use 100% of all 8 vCPU’s giving that VM a Max CPU performance of 800%.


```


Azure Disk pricing
https://azure.microsoft.com/en-us/pricing/details/managed-disks/
