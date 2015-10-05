The default validation error messages are imported in your app's `validators` folder. If you want to change or extend them, all you need to do is create a `messages.js` file under `app/validators`.

```javascript
// app/validators/messages.js

import Messages from 'ember-cp-validations/validators/messages';

export default Messages.extend({
  uniqueUsername: '{attributeDescription} {username} already exists'
});
```

Within this object, you can overwrite the [default messages](https://github.com/offirgolan/ember-cp-validations/blob/master/addon/validators/messages.js) or create new messages just like in the example above. If a message of a given type is not found, it will default to the `invalid` message. Usage examples can be found [here](validators/common/#createerrormessage)

# I18n Solutions

* __Ember-Intl__

_**Notice**: Supports Ember-Intl v2.x and above_

```bash
ember install ember-intl-cp-validations
```

Setup instructions can be found on the [github page](https://github.com/jasonmit/ember-intl-cp-validations).

* __Ember-I18n__

```bash
ember install ember-i18n-cp-validations
```

Setup instructions can be found on the [github page](https://github.com/jasonmit/ember-i18n-cp-validations).
