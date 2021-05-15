# bitburner-scripts

At start of Augment

exec.acquire-root-access.ns
This runs forever and acquires root access on servers as new ports and skill are available

exec.hack-dist.ns
This runs forever and runs programs on all servers that root has been acquired on

exec.autocontract.ns
Runs forever and solves contracts that it finds on servers.

stock-buyer-2.ns
Once all stock APIs are available and there is enough money to bother.
Cannot run until all the stock market stuff is purchased.
Generally I don't run this until I have already bought all but the most
expensive attack program.

exec.purchase-servers.ns
Purchases 1 server of 8g, then one of 16g, then one of 32, and continues to go up in size
for the next purchase until it reaches the max (of 2^20).
Will evenutally buy all servers at the max.

exec.notify.ns
Trigger exec.hack-dist.ns to reconfigure what's running where.

exec.deepscan.ns
Generates a scan of all servers in the system. Outputs serves in red (not currently rootable),
blue (rootable, but not currently rooted), or green (rooted).

exec.commit-crimes.ns
Commits the most efficient crime, by a very poor metric.
Useful if you have the singularity 3, or are in it currently, and are trying to put some
cash together at the beginning of the BN.

purchase-server-8gb.script
Run only once, it will purchase 25 8g servers.
Deprecated: I don't use this one anymore

upgrade-servers.ns <size>
Upgrade all servers to a size of <size>, where size is log2 of RAM size (so 8 is 3, 1024 is 10). Will run
it upgrades all purchased servers, then trigger exec.hack-dist.ns to reconfigure what's running where.
Deprecated: I don't use this one anymore
