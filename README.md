# Immutos APT Repository

## Usage

```shell
curl -fsL https://apt.immutos.com/signing_key.asc | sudo tee /etc/apt/keyrings/apt-immutos-com-keyring.asc > /dev/null
echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/apt-immutos-com-keyring.asc] http://apt.immutos.com $(. /etc/os-release && echo $VERSION_CODENAME) stable" | sudo tee /etc/apt/sources.list.d/apt-immutos-com.list > /dev/null
```