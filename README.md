angucomplete-alt (with custom HTTP headers)
============

### Remote Usage

```html
<angucomplete-alt id="members"
              placeholder="Search members"
              pause="400"
              selected-object="testObj"
              remote-url="http://myserver.com/api/user/find?s="
              remote-url-data-field="results"
              title-field="firstName,surname"
              description-field="email"
              image-field="profilePic"
              input-class="form-control form-control-small"
              http-headers="getAuthHeaders()"/>
```

```javascript
$scope.getAuthHeaders = function() {
  return {
    Authorization: 'Token qwerty123456'
  }
}
```
