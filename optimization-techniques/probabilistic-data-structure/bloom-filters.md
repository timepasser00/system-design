## Intro
A Bloom filter is a space-efficient, probabilistic data structure used to test whether an element is in a set. It can return false positives but never false negatives. It's ideal for scenarios where memory is limited and exact membership isn't required, like caching, databases, or duplicate detection in large systems.

## 🔧 How a Bloom Filter Works

1. **Initialize** a bit array of size *m*, with all bits set to `0`.
2. **Choose** *k* independent hash functions.
3. **Insert an element**:
   - Hash the element using each of the *k* hash functions.
   - Set the *k* corresponding bit positions in the array to `1`.
4. **Check for membership**:
   - Hash the element again with the same *k* hash functions.
   - If **any** of the bits is `0` → element is **definitely not** present.
   - If **all** bits are `1` → element **might be present** (possible false positive).
5. **Note**: Deletion is **not supported** without additional structures (e.g., Counting Bloom Filter).


# Examples

Caching:
Before querying a cache like Redis, use a Bloom filter to check if a key might exist. If not, skip the lookup.

Web Crawlers:
A crawler uses a Bloom filter to avoid re-visiting already seen URLs.

Email Spam Detection:
Maintain a Bloom filter of known spammy IP addresses to quickly filter incoming emails.
