# EC2 Metadata Fetcher

This script allows you to query and fetch metadata for an EC2 instance running on AWS using the Instance Metadata Service v2 (IMDSv2). It retrieves metadata like instance ID, instance type, security groups, and more. The script requires an IMDSv2 session token to interact with the metadata service securely.

## Features

- Fetch specific metadata by providing a key (e.g., `instance-id`, `ami-id`).
- Fetch all available metadata if no key is provided.
- Handles token generation and expiration automatically.
- Returns metadata in a clean, readable JSON format.
  
## Requirements

- Python 3.x
- `requests` library (for making HTTP requests)


To install the `requests` library, you can use pip:

```bash
pip install requests
```



## References

References : https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instancedata-data-retrieval.html