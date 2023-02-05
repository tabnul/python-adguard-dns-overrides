# Description
A simple wrapper around the DNS Override funtionality of Adguard DNS.
Can be used to set local DNS Names in your deployment pipelines (e.g. give your server a DNS name)

# Usage
The Adguard API isn't a proper REST api. It does not editing records, it only supports ADD or DELETE and it will happily add multiple of the same records.
To edit a record, delete and re-create. 

    manage_overrides.py --fqdn exampleserver.localdomain --ip 10.100.10.10 --adguardurl https://adguard.localdomain --adguarduser adguarduser --adguardpassword adguardpassword --action add
