## Sending Form Data
[Sending Form Data](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Sending_and_retrieving_form_data)

Additional Resources
[HTML5 Forms Reference](https://htmlreference.io/forms/) Pay special attention to the “action” and “method” attributes.
[Video Series on Styling HTML5 Forms](https://www.youtube.com/playlist?list=PL4cUxeGkcC9g5_p_BVUGWykHfqx6bb7qK) Note that this video series is approximately 40 minutes long. You do not need to watch every video from the series, but should keep it handy for reference as you style your book app during lab time.

### [Sending Form Data](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Sending_and_retrieving_form_data)
Client Side - sending data
- client computers and servers communitcate through HTTP(S)
- info sent at `name=value` pairs
- on the `form` we tell the computer how to send the data using `action` and `method`
  - `action ` says where to send the data
  - `method` defines how data is sent, most commonly `GET` or `POST`
    - `GET` asks the server to send back a given resource
    - `POST` method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request
  - View requests through web dev tools in the Network tab
Server Side - retrieving data
- 
Special case - sending files
- `<input type="file">` allows users to select the file(s) that will be uploaded.
Security Issues
- It's possible to perform client-side form validation, but the server can't trust this validation because it has no way to truly know what has really happened on the client-side
- Never trust users...All data that comes to your server must be checked and sanitized
  - Escape potentially dangerous characters
  - Limit the incoming amount of data to allow only what's necessary
  - Sandbox uploaded files