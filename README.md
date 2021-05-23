# Essentials
This repo includes all the essential codes that I use on a day to day basis...

## ESLINT CONFIG -

#### Dev Dependencies:
*npm install --save-dev eslint-config-react-app @typescript-eslint/eslint-plugin@^4.0.0 @typescript-eslint/parser@^4.0.0 babel-eslint@^10.0.0 eslint@^7.5.0 eslint-plugin-flowtype@^5.2.0 eslint-plugin-import@^2.22.0 eslint-plugin-jsx-a11y@^6.3.1 eslint-plugin-react@^7.20.3 eslint-plugin-react-hooks@^4.0.8*

Then create a file named .eslintrc.json with following contents in the root folder of your project:
```json
{
  "extends": "react-app"
}
```

## PORT FORWARDING FOR EC2 -
```js
sudo iptables -t nat -L
sudo iptables -t nat -A PREROUTING -p tcp --dport 80:443 -j REDIRECT --to-ports 8000 # 8000 -> 8000
```
Response that you will want: `tcp dpts:http:https redir ports 8000`
