Adds or modifies a group from the system.
The `id` can be retrieved with from the `GET /api/v1/groups` endpoint.

```bash
$ curl -k \
  -u <USER> \
  -H 'Content-Type: application/json' \
  -X POST \
  -d '{"groupName": "wonks", "user": [{"username": "ian"},{"username": "toad"}],"ldapGroup": false,"samlGroup": false,"role": "admin"}' \
  https://<CONSOLE>:8083/api/v1/groups
```
