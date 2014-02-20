*This repository is a mirror of the [component](http://component.io) module [yields/serialize](http://github.com/yields/serialize). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/yields-serialize`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# serialize

  serialize forms.

## Installation

  Install with [component(1)](http://component.io):

    $ component install yields/serialize

## Example

```html
<input type='text' name='foo' value='baz'>
<input type='text' name='baz' value='foo'>
<select name='select'>
  <option value='1'></option>
</select>

<script>
  var el = document.forms[0];
  assert('foo=baz&baz=foo&select=1' == serialize(el));

  serialize.object(el);
  // => { foo: "baz", baz: "foo", select: "1" }
</script>
```

## License

  MIT
