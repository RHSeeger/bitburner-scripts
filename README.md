# bitburner-scripts

At start of Augment

exec.acquire-root-access.ns
This runs forever and acquires root access on servers as new ports and skill are available

exec.hack-dist.ns
This runs forever and runs programs on all servers that root has been acquired on

exec.autocontract.ns
Runs forever and solves contracts that it finds on servers.
Doesn't actually run forever.. need to look into that.

stock-buyer-2.ns
Once all stock APIs are available and there is enough money to bother. Generally after

purchase-server-8gb.script
Run only once, it will purchase 25 8g servers. Each server costs 400,000, so it's worth waiting until
several times that is available. It will run until it purchases all 8 serverss.

upgrade-servers.ns <size>
Upgrade all servers to a size of <size>, where size is log2 of RAM size (so 8 is 3, 1024 is 10). Will run
it upgrades all purchased servers, then trigger exec.hack-dist.ns to reconfigure what's running where.

exec.notify.ns
Trigger exec.hack-dist.ns to reconfigure what's running where.

exec.deepscan.ns
Generates a scan of all servers in the system. Outputs serves in red (not currently rootable),
blue (rootable, but not currently rooted), or green (rooted).

