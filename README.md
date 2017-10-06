# Alexa Skill Node.js Template

## Use

Use with AWS Lambda or on appropriate hosting environment.

### Slots

Be sure to replace 'MySlot' with the actual name of your slot!

```js
this.event.request.intent.slots.MySlot.value
```

### Output

Speech output is set on ```response.speak('text')```  

Reprompt text is set on ```.listen('try again')```

Finally, it's sent back to the client when ```this.emit(':responseReady')``` is called.

```js
this.response.speak(say).listen('try again');
this.emit(':responseReady');
```

### Session

The session can be accessed by calling ```this.event.session```

### Attributes

Session attributes are accessed by calling ```this.event.attributes```

To set a session attribute, make sure you have intialized a session.attributes object.

```js
var attributes = {}
```

or  

```js
var attributes = this.session.attributes;
```

### Setting/Getting Attributes

To set an attribute...

```js
this.attributes['someval'] = someVal;
```

To get an attribute...

```js
var val = this.attributes['someval'];
```
