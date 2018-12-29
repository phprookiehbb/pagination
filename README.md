# pagination
tp5数组分页,可定制样式,稍微修改一下可使用与所有的情形下的数组分页

## Installation
Pagination is available on [Packagist](https://packagist.org/packages/phprookiehbb/pagination).Just add this line to your `composer.json` file:

```json
"phprookiehbb/pagination": "dev-master"
```

or run

```sh
composer require phprookiehbb/pagination
```
### Example

``` php
use Crasphb\Pagination;
$pagination = new Pagination($target,1,['simple'=>false,'allCounts'=>true,'nowAllPage'=>true,'toPage'=>true]);
$item = $pagination->getItem();
$page = $pagination->render();
```

### Show

![Image1 text](http://crasphter.cn/usr/uploads/2018/08/233997006.png)</br>
![Image2 text](http://crasphter.cn/usr/uploads/2018/08/959581326.png)</br>
![Image3 text](http://crasphter.cn/usr/uploads/2018/08/1891541248.png)</br>
![Image4 text](http://crasphter.cn/usr/uploads/2018/08/1913813996.png)</br>