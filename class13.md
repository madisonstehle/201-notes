## 12/4/19

## Local Storage

### Limitations of Cookies
- Cookies are included with HTTP request which
    - slows down your app by needlessly tranmitting the same data over and over
    - sends data unencrypted over the internet
- Cookies are also limited to about 4KB of data

### HTML5 Storage

> **HTML5 Storage** set out to provide a standardized API that was implemented _natively_ and _consistently_ in multiple browsers mithout having to rely on third-party plugins.

HTML5 Storage, also referred to as _Local Storage_ or _DOM Storage_, is based on named key/value pairs. The data can be any type supported by JavaScript (strings, Booleans, integers, floats), but the data is actually stored as a string.

Some associated methods include `getItem()`, `setItem()`, `removeItem()`, and `key()`.

### Limitations of HTML5 Storage

- Each origin gets 5 megabytes of storage by default.
- If you exceed the storage quota, `QUOTA_EXCEEDED-ERR` is thrown.

#### [Back to Home](index.md)