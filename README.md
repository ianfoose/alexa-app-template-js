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

```js
this.response.speak(say).listen('try again');
```

### Session

The session can be accessed by calling ```this.event.session```

To end a session, use ```this.emit(':tell');```

To keep a session open, use ```this.emit(':ask');```

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

More documentation found at https://www.npmjs.com/package/alexa-sdk

and https://github.com/alexa/alexa-skills-kit-sdk-for-nodejs
