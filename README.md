# telegram-go-example
Example to interact with telegram api using golang

# Install dependencies
 
*This example is for running on Mac OS, for other os please refer to official [docs](https://github.com/tdlib/td#features)*

```shell
brew install gperf cmake openssl
```

**install tdlib**

```
git clone git@github.com:tdlib/td.git
cd td
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Release -DOPENSSL_ROOT_DIR=/usr/local/opt/openssl/ ..
cmake --build .
make install
```

# Get api_id, api_hash

- Log in to your Telegram core: https://my.telegram.org.
- Go to ‘API development tools’ and fill out the form.
- You will get basic addresses as well as the api_id and api_hash parameters required for user authorization.

# Build example

Using your api_id and api_hash you get above to fill in the code and run. Using get_chats.go to get chat ids, use those id to fill in send_message.go to run send message example.
