## Go Whatsapp API Multi Device Version

### Required

- Mac OS:
    - `brew install vips`
    - `export CGO_CFLAGS_ALLOW="-Xpreprocessor"`
- Linux:
    - `sudo apt update`
    - `sudo apt install libvips-dev`
- Windows:
    - https://www.libvips.org/install.html

### How to use

1. Clone this repo `git clone https://github.com/aldinokemal/go-whatsapp-web-multi-device`
2. run `go run main.go`
3. open `http://localhost:3000`

You can fork or edit this source code !

Current API

| Feature  | Menu                 | Method | URL            | Payload                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|----------|----------------------|--------|----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ✅        | Login                | GET    | /app/login     |                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ✅        | Logout               | GET    | /app/logout    |                                                                                                                                                                                                                                                                                                                                                                                                                                                        |  
| ✅        | Reconnect            | GET    | /app/reconnect |                                                                                                                                                                                                                                                                                                                                                                                                                                                        | 
| ✅        | User Info            | GET    | /user/info     | <table> <thead> <tr> <th>Param</th> <th>Type</th> <th>Type</th> <th>Example</th> </tr></thead> <tbody> <tr> <td>phone_number</td><td>string</td><td>querystring</td><td>6289685024099</td></tr></tbody></table>                                                                                                                                                                                                                                        |
| ✅        | User Avatar          | GET    | /user/avatar   | <table> <thead> <tr> <th>Param</th> <th>Type</th> <th>Type</th> <th>Example</th> </tr></thead> <tbody> <tr> <td>phone_number</td><td>string</td><td>querystring</td><td>6289685024099</td></tr></tbody></table>                                                                                                                                                                                                                                        |
| ✅        | Send Message (Text)  | POST   | /send/message  | <table> <thead> <tr> <th>Param</th> <th>Type</th> <th>Type</th> <th>Example</th> </tr></thead> <tbody> <tr> <td>phone_number</td><td>string</td><td>form-data</td><td>6289685024099</td></tr><tr> <td>message</td><td>string</td><td>form-data</td><td>Hello guys this is testing</td></tr></tbody></table>                                                                                                                                            |
| ✅        | Send Message (Image) | POST   | /send/image    | <table> <thead> <tr> <th>Param</th> <th>Type</th> <th>Type</th> <th>Example</th> </tr></thead> <tbody> <tr> <td>phone_number</td><td>string</td><td>form-data</td><td>6289685024099</td></tr><tr> <td>caption</td><td>string</td><td>form-data</td><td>Hello guys this is caption</td></tr><tr> <td>view_once</td><td>bool</td><td>form-data</td><td>false</td></tr><tr> <td>image</td><td>binary</td><td>form-data</td><td></td></tr></tbody></table> | 

```
✅ = Available
❌ = Not Available Yet
```

### Mac OS NOTE

Please do this if you have an error (invalid flag in pkg-config --cflags:
-Xpreprocessor) `export CGO_CFLAGS_ALLOW="-Xpreprocessor"`
