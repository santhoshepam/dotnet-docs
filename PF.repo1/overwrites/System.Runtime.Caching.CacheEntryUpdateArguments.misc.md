---
uid: System.Runtime.Caching.CacheEntryUpdateArguments
additional_notes.overrides: *content
---

<p>A callback handler must notify the cache implementation whether to insert a replacement entry into the cache in place of the cache entry that is about to be removed. If you want to exchange cache entries, you must assign a value other than `null` to the <xref href="System.Runtime.Caching.CacheEntryUpdateArguments.UpdatedCacheItem"></xref> property. Cache implementations will interpret a `null` value for the <xref href="System.Runtime.Caching.CacheEntryUpdateArguments.UpdatedCacheItem"></xref> property as a notice that the current cache entry should be removed but not replaced.</p>


