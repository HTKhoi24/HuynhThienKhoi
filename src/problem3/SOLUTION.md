Provide your solution here:
Some of the causes for the issue:
	1. Excessive logging or large log files: log files grow over time or large log being processed in real time.
		Impacts: slow down the server, system become unresponsive and cause high operation cost.
		Fixing: 
			check for log files in disks to prevent,
			use logrotate to automatically rotate and compress log files,
			use AWS S3 or others for offload log files.
	2. Huge amount of cached items or large ones: caching is enabled can lead to memory consuming.
		Impacts: delays in processing requests, increase latency, limit the scalability of server.
		Fixing:
			use monitoring tools for cache memory usage,
			remove unuse entries and clean up temporary files,
			define proper cache expiration times.
	3. NGINX not properly config: NGINX configuration file settings are not optimized.
		Impacts: high memory usage, slower response time. connection failures, crashes and may expose to DDOS attacks.
		Fixing:
			using monitor tools for real-time data and change the configuration.
	4. Using third-party add-ons cause memory leak: bugs in NGINX modules and other extensions causing memory loss.
		Impacts: unstable system, cause server crashes, increase maintenance cost and increase resource used.
		Fixing:
			use monitor tools to monitor memory distribution,
			update NGINX to more stable version,
			check before use extensions.
	5. High traffic volume / system limits: the server need to handle a large number of requests or memory allocation is insufficient.
		Impacts: system crashes, reduce performance.
		Fixing:
			enable connection limit,
			optimize NGINX configuration,
			increase resource.