<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

  <p align="center">A progressive <a href="http://nodejs.org" target="_blank">Node.js</a> framework for building efficient and scalable server-side applications.</p>
    <p align="center">
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/v/@nestjs/core.svg" alt="NPM Version" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/l/@nestjs/core.svg" alt="Package License" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/dm/@nestjs/common.svg" alt="NPM Downloads" /></a>
<a href="https://circleci.com/gh/nestjs/nest" target="_blank"><img src="https://img.shields.io/circleci/build/github/nestjs/nest/master" alt="CircleCI" /></a>
<a href="https://coveralls.io/github/nestjs/nest?branch=master" target="_blank"><img src="https://coveralls.io/repos/github/nestjs/nest/badge.svg?branch=master#9" alt="Coverage" /></a>
<a href="https://discord.gg/G7Qnnhy" target="_blank"><img src="https://img.shields.io/badge/discord-online-brightgreen.svg" alt="Discord"/></a>
<a href="https://opencollective.com/nest#backer" target="_blank"><img src="https://opencollective.com/nest/backers/badge.svg" alt="Backers on Open Collective" /></a>
<a href="https://opencollective.com/nest#sponsor" target="_blank"><img src="https://opencollective.com/nest/sponsors/badge.svg" alt="Sponsors on Open Collective" /></a>
  <a href="https://paypal.me/kamilmysliwiec" target="_blank"><img src="https://img.shields.io/badge/Donate-PayPal-ff3f59.svg"/></a>
    <a href="https://opencollective.com/nest#sponsor"  target="_blank"><img src="https://img.shields.io/badge/Support%20us-Open%20Collective-41B883.svg" alt="Support us"></a>
  <a href="https://twitter.com/nestframework" target="_blank"><img src="https://img.shields.io/twitter/follow/nestframework.svg?style=social&label=Follow"></a>
</p>
  <!--[![Backers on Open Collective](https://opencollective.com/nest/backers/badge.svg)](https://opencollective.com/nest#backer)
  [![Sponsors on Open Collective](https://opencollective.com/nest/sponsors/badge.svg)](https://opencollective.com/nest#sponsor)-->

## Penting
- pastikan sudah menginstall mongodb server dan mysql
- port yang digunakan didalam service admin 8002
- port yang digunakan didalam service main 8003



## Installation

```bash
$ npm install
```

## Menjalankan aplikasi menggunakan 3 terminal secara bersamaan

```bash
# jalankan local server di dalam direktori src/ pada service admin
$ npm run start:dev

# jalankan local server di dalam direktori src/ pada service main untuk melakukan listen rabbitmq service main
$ npm run listen

# jalankan local server di dalam direktori src/ pada service main
$ npm run start:dev
```
<br/>
<br/>
<br/>


## 🍃 Admin Service http request
<br/>
### 1. Membuat Produk Baru

**URL:** `localhost:8003/api/products`

**Metode:** `POST`

**Deskripsi:** Endpoint ini digunakan untuk membuat produk baru.

**Body Request:**

```json
{
    "title": "isi dengan title",
    "image": "contoh gambar "
}
```
<br/>
<br/>



### 2. Melihat semua product
<br/>
**URL:** `localhost:8003/api/products`

**Metode:** `GET`

**Deskripsi:** Endpoint ini digunakan untuk membuat produk baru.
<br/>
<br/>




### 3. Melihat semua product Berdasarkan ID
<br/>
**URL:** `localhost:8003/api/products/1`

**Metode:** `GET`

**Deskripsi:** Endpoint ini digunakan untuk membuat produk baru.
<br/>
<br/>



### 4. Merubah Produk Baru
<br/>
**URL:** `localhost:8003/api/products/1`

**Metode:** `PUT`

**Deskripsi:** Endpoint ini digunakan untuk merubah produk.

**Body Request:**

```json
{
    "title": "isi dengan title perubahan",
    "image": "contoh gambar perubahan "
}
```
<br/>
<br/>


### 5. Menghapus Produk Baru
<br/>

**URL:** `localhost:8003/api/products/1`

**Metode:** `DELETE`

**Deskripsi:** Endpoint ini digunakan untuk menghapus produk.

<br/>
<br/>
<br/>



## 🍃 Main Service http request
<br/>


### 1. Mengambil semua produk dari service Main

**URL:** `localhost:8002/api/products`

**Metode:** `GET`

**Deskripsi:** Endpoint ini digunakan untuk mengambil semua  produk yang sudah di buat di dalam service admin.
<br/>
<br/>



### 2. Memberikan Like Product
<br/>
**URL:** `localhost:8002/api/products/1/like`

**Metode:** `POST`

**Deskripsi:** Endpoint ini digunakan untuk memberikan nilai like pada produk yang disukai.


### SELESAI















