### Prerequisites

* Windows 11(64GB)
* NVidia video card (RTX3060 12GB)
* WSL2 (32GB and operation confirmed on Ubuntu 20.04)

*Not confirmed in other configurations than those listed above.

### Installing

* Build Docker with the following command
```
docker compose build
```

## Usage

* Access the following after docker compose up -d
* Turn on the PROXY setting of the OS or browser and set localhost:8080.

## Version

* 2024/06/01 Initial commits.

## Acknowledgments

* [docker-composeで作る通信確認用mitmproxy](https://qiita.com/garupon/items/5540ea14809361e92d99)