# pagination
数组分页,可定制样式,内置3种样式,稍微修改一下可使用与所有的情形下的数组分页

## Installation
Pagination is available on [Packagist](https://packagist.org/packages/phprookiehbb/pagination).Just add this line to your `composer.json` file:

```json
"phprookiehbb/pagination": "dev-master"
```

or run

```sh
composer require phprookiehbb/pagination:dev-master
```
### Example

``` php
use Crasphb\Paginate;
$pagination = new Pagination($target,1,['style' => 1,'simple'=>false,'allCounts'=>true,'nowAllPage'=>true,'toPage'=>true]);
//数组的分页后的元素
$item = $pagination->getItem();
//分页样式的渲染
$page = $pagination->render();
```

### Explanation
|  参数 |  类型 |  说明 |
| ------------ | ------------ |------------ |
| target  | array  | 需要分页的数组  |
| defaultPageSize  | int  | 每页的数目  |
|  style | int  | 分页样式，可选值1,2,3  |
|  simple | boolean  |  true:简单的分页样式,false:复杂的分页样式 |
|  allCounts | boolean  |  显示总页数 |
| nowAllPage  | boolean  |  显示现在的页码 |
|  toPage |  boolean | 跳转页码的功能  |

### Show

#### simple模式
![Image1 text](http://crasphter.cn/usr/uploads/2018/08/233997006.png)
#### style = 1,2,3
![Image1 text](http://crasphter.cn/usr/uploads/2018/08/233997006.png)
![Image1 text](http://crasphter.cn/usr/uploads/2018/08/233997006.png)
![Image1 text](http://crasphter.cn/usr/uploads/2018/08/233997006.png)
#### allCount,nowAllPage,toPage模式
![Image1 text](http://crasphter.cn/usr/uploads/2018/08/233997006.png)