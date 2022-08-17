<p align="center"><img src='https://sun9-17.userapi.com/impg/RezfgyBkpS_juJs4Wy9kLV6jPkKxKiQk3_y8TQ/zbsbm6INxn4.jpg?size=225x225&quality=96&sign=5be45842c90d1c95631f148718aa48aa&c_uniq_tag=nUvHehKRj7X2DVzokCC-MJEeAK7iZbU6YR8ZSylxqLU&type=album'></img></p>
<p align='center'>
<a href="https://www.npmjs.com/package/vksnake"><img src="https://img.shields.io/npm/v/vksnake.svg?style=flat-square" alt="NPM version"></a>
</p>

<p align='center'><img src='https://img.shields.io/badge/code%20style-standard-brightgreen.svg'></img></p>
<p align='center'><img src='https://img.shields.io/npm/dt/vksnake.svg'></img></p>

## 📦 Installation

> **[Node.js](https://nodejs.org/) 12.20.0 or newer is required**

- **Using `Yarn`** (recommended)
  ```shell
  yarn add vksnake
  ```
- **Using `npm`**
  ```shell
  npm i vksnake
  ```
- **Using `pnpm`**
  ```shell
  pnpm add vksnake
  ```

- ## Usage to methods VK

```javascript
import { Method, VK } from 'vksnake';

const vk = new VK({ 
token: process.env.TOKEN
})

async function method () {

const body = await new Method().use('users.get', {
user_id: 501
})

console.log(body)

}

method ()
```

```javascript
import { Method, VK } from 'vksnake';

const vk = new VK({
token: process.env.TOKEN
})

async function method () {

const body = await new Method().use('wall.get', {
owner_id: 1
})

console.log(body)

}

method ()
```

## Usage to method 
```javascript
import { Method, VK } from 'vksnake';

const vk = new VK({
token: process.env.TOKEN
})

async function method () {

const body = await new Method().getInfoUser(501, { user_id: 501 })

console.log(body)

}

method()
```

## Send message in chat
```javascript
import { Method, VK, getRandomId } from 'vksnake';

const vk = new VK({
token: ''
})

async function method () {

const body = await new Method().use('messages.send', {
random_id: getRandomId(),
peer_id: ...userId or chatId,
message: 'Привет'
})

console.log(body) // Object
}

// or

async function method () {

const body = await new Method().send('Привет', {
senderId: ...userId or chatId
})

console.log(body) // Object
}

```
## Checking token
```javascript
import { Method, VK } from 'vksnake';

const vk = new VK({
token: process.env.TOKEN
})

const body = new Method().secretSnake();

console.log(body) // Boolean
```

- [GitHub](https://github.com/ostrovsky-swedesdart/vksnake)

## Support

<p style="text-align: center" align="center"><a href="https://qiwi.com/p/NODEJSLUPUS"><img scr="https://sun9-83.userapi.com/impg/9JsEyB1iBNukDvQ2k8Vf_jeXNA9fx1Fk3TuhDw/T98hP8JqGug.jpg?size=604x352&quality=96&sign=abfbfb49bd388a2ec020bd96cc7fd62f&c_uniq_tag=u7e5F1ZhrxdV8g2hOAhNEAbdTz-htHPSQlxWCQEoMJk&type=album">Пожертвовать / Support</img></a></p>
<p style="text-align: center" align="center">Ник QIWI: NODEJSLUPUS</p>

## Contacts

<p style="text-align: center" align="center"><a href="https://vk.com/swedesdart_rus">- VK</a></p>
<p style="text-align: center" align="center"><a href="https://github.com/ostrovsky-swedesdart">- GitHub</a></p>