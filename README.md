# Belajar Golang JSON

## Pendahuluan
JSON (JavaScript Object Notation) adalah format data yang ringan dan mudah dibaca, sering digunakan untuk pertukaran data antar sistem. Golang menyediakan package `encoding/json` untuk bekerja dengan JSON.

## Pengenalan Package JSON
Package `encoding/json` digunakan untuk melakukan encode (mengubah data Go menjadi JSON) dan decode (mengubah JSON menjadi data Go).

## Encode JSON
Proses mengubah data Go (struct, map, slice) menjadi string JSON menggunakan `json.Marshal` atau `json.MarshalIndent`.

## JSON Object
Representasi data dalam bentuk objek `{}`. Biasanya digunakan untuk menyimpan data dengan pasangan key-value.

## Decode JSON
Proses mengubah string JSON menjadi data Go menggunakan `json.Unmarshal`.

## JSON Array
Representasi data dalam bentuk array `[]`. Digunakan untuk menyimpan kumpulan data dengan tipe yang sama.

## JSON Tag
Tag digunakan pada struct untuk menentukan nama field dalam JSON. Contoh:  
```go
type User struct {
    Name string `json:"name"`
    Age  int    `json:"age"`
}
