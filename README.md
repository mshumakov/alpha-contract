### Alpha Contract

[![build](https://github.com/mshumakov/alpha-contract/workflows/build/badge.svg)](https://github.com/mshumakov/alpha-contract/actions)

A set of common decisions, agreements and practices for further implementation.

## Installation

To install, download the package using the following command.

```shell script
composer require mshumakov/alpha-contract
```

## Example

An example implementation of a DTO request agreement.

```php
<?php
declare(strict_types=1);

namespace Path\To\Class;

class ExchangeRequest implements RequestInterface
{
    /**
     * @var float $price
     */
    protected $price;

    /**
     * @param float $price
     */
    public function setPrice(float $price): void
    {
        $this->price = $price;
    }

    /**
     * @return float
     */
    public function getPrice(): float
    {
        return $this->price;
    }
}
```