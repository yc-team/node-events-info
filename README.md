node-events-info
================

## Class: events.EventEmitter

通过require('events').EventEmitter来访问EventEmitter类


### emitter.addListener(event,listener) 和 emitter.on(event,listener)

添加一个listener到给指定的event的listeners数组的最后一个。

```javascript
server.on('connection', function(stream){
	console.log('someone connected');
});
```

返回emitter，方便链式调用。



### emitter.once(event,listener)

给event添加指定一次性的事件，这个事件只会在下一次事件发生时候被触发一次，触发完成后就被删除了

```javascript
server.once('connection', function(stream){
	console.log('one time by zhangyaochun');
});
```

返回emitter，方便链式调用。