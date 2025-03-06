Provide your solution here:

- Trading system features:
	1. User Management: Authorization, authentication, account details.
	2. Order Matching Engine: Process buy and sell orders.
	3. Market Data Feeds: Real time updates on prices and trades.

- Services Used:
	1. Frontend: Using a Content Delivery Network like AWS CloudFront.
	2. Backend Services: 
		AWS API Gateway to handle and route incoming requests, 
		AWS Lambda for backend logic, 
		Amazon Cloud Watch tracking performance.
	3. Database: Amazon DynamoDB for low latency and high throughput storage. 
	4. Network: Elastic Load balancer for routing requests.
- Why use these services:
	1. AWS CloudFront and API Gateway to reduce load on backend caching responses closer to users.
	2. AWS Lambda adjust automatic to demand and ensure throughput limit around 1000.
	3. Amazon DynamoDB for high throughput and global tables for low latency.
	4. Amazon CloudWatch provide realtime metrics.
- Plans for scaling:
	1. API Scaling:
		perform load testing to identify bottlenecks and optimize Lambda performance,
		add API Gateway for manage API requests efficiently.
	2. Database Scaling:
		upgrade hardware and distribute data across multiple server,
		divide large tables into smaller, manageable partitions,
		optimize queries with query tuning.
	3. Disaster Recovery: 
		set up a database cluster with failover node, 
		implement monitoring tools to detect anomalies,
		divine database into smaller manageable parts or on multiple server.