# ISP OS License Management

Private repository for ISP OS license verification.

## Structure

```json
{
  "licenses": {
    "XXXX-XXXX-XXXX-XXXX": {
      "hardware_id": "sha256hash...",
      "customer": "Customer Name",
      "status": "active",
      "activated_at": "2026-03-08",
      "last_verified": "2026-03-08",
      "notes": "Optional notes"
    }
  }
}
```

## Status Values
- `active` - License is valid
- `revoked` - License has been revoked
- `suspended` - Temporarily suspended

## How It Works
1. ISP OS device generates hardware ID from disk serial
2. Device checks this repo via GitHub API every 24h
3. If license valid → full access
4. If revoked/missing → features disabled

## Revoke a License
Simply change `"status": "active"` to `"status": "revoked"` and commit.
