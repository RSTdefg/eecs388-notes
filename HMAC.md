- Input: key, arbitrary length data
- Output: fixed size digest
- Design protects against length extension
- For practical purposes, we (think/hope) we can treat HMAC-SHA256 as a #PRF
- 