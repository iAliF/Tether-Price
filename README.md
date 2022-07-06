# Tether Price

### Tether price is a library that help you to get Tether price from various websites.

## How To Install

#### You can use following command to install it.

```commandline
pip install tether-price
```

## Getting Started

```python
from tether import SourceManager
from tether.sources import Bitbarg

manager = SourceManager()
manager.add(Bitbarg())

if __name__ == '__main__':
    prices_list = manager.get_prices_list()
    for price in prices_list.prices:  # type: Price
        print(f'{price.source} | Buy: {price.buy} | Sell: {price.sell}')
```

## License

[MIT](https://github.com/iAliF/Tether-Price/blob/main/LICENSE)