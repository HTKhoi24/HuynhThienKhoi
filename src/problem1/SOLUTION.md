Provide your CLI command here:
for orderId in "12346" "12362"; do curl -s "https://example.com/api/${orderId}" >> ./output.txt; done