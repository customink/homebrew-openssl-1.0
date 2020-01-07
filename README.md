# OpenSSL@1.0
Tap to keep supporting the openSSL 1.0 for legacy projects

# Installation

```
brew tap customink/openssl-1.0
brew install "openssl@1.0"
```

# Usage
Since this is now a tap, you'll need to update your paths manually.
This is for example what I use to compile the `mysql2` gem in old projectS:

```
bundle config build.mysql2 "--with-ldflags=-L$(brew --prefix "openssl@1.0")/lib"
```
