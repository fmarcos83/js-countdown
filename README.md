# js-countdown

A library for easy countdown management

## Examples

#### instantiating

```javascript
    //countdown to 5 seconds in the future
    //will output the deadline object
    var countdown = new Coundown({
        deadLineDate : new Date(Date.now()+5000)
        callback: function(deadLineDate){console.log(deadLineDate);}
        [startDate : new Date(Date.now()+4000)],
        [repeatInterval : 1000]
    });
```

#### init countdown

```javascript
    //init countdown will
    countdown.init();
```

#### signal listener addition

```javascript
    //init countdown will
    countdown.updated.add(function(){});
    countdown.stopped.add(function(){});
```

## License

[MIT](http://opensource.org/licenes/mit-license.php)

## Dependencies

> js-signals is the defacto signal library for this component
> nevertheless the plan is to create a wrapper so
> anyone can inject it's custom signal library

[js-signals](https://github.com/millermedeiros/js-signals)

## Installing

### bower

```bash
bower install js-countdown
```
