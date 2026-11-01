# migvpn-bootstrap

Signed list of MigVPN API addresses. The apps read `endpoints.json` only when
none of the addresses they already know answers, and accept it only with a
valid P-256 signature and a higher `seq` than the list they have.

The file contains no secrets. It is updated with
`scripts/api-endpoints-publish.py` from the main repository.
