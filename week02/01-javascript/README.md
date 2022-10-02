![Image Banner!](../assets/javascript-banner.png "Javascript")
# **Javascript**

## Perulangan/Looping

### Apa itu perulangan ?
> perluangan adalah suatu bentuk kegiatan mengulang suatu statement sampai batas yang diinginkan.

![Image Banner!](../assets/js-looping.png "Javascript")

### Ada berapa Jenis perulangan pada javascript ?
>1. for
>> cetak string 'ayo belajar' sebanyak 10 kali
>>```
>> for(let i = 1; i <= 10; i++){
>>    console.log('ayo belajar' )
>>  };
>>```
>> cetak angka 1 s/d 10 dan temukan angka 7
>>```
>> for(let i = 1; i <= 10; i++){
>>    if (i == 7){
>>        console.log(i + ' nah ini ketemu nih);
>>    } else {
>>        console.log(i);
>>    };
>>};
>>```
>- while
>>  nyalakan mesin jika bensin > 0, bensin akan terus berkurang dan berhenti ketika bensin = 0 atau habis;
>> ```
>> while(bensin > 0){
>>    console.log("Masih ada bensin, nyalakan mesin!");
>>   bensin--;
>>};

>- do while
>>```
>> do{
>>    console.log("Nyalakan mesin!");
>>    bensin--;
>> } while(bensin > 0)

## Javascript Scope
### Apa itu scope ?
> scope adalah konsep data variabel atau bisa di bilang 'jangkauan', menentukan sebuah variabel bisa di akses pada scope tertentu atau tidak.

### Apa itu blocks ?
> block adalah code yang berada di dalam '{}', terdapat pada function, condition, looping

### Global scope vs Local scope
>- **Global scope**
>   - tempat yang membuat variabel kita bisa di akses dimana pun pada seluruh isi file, kita harus menempatkan variabel kita diluar blocks

>- **local scope**
>   - tempat yang membuat kita hanya bisa di akses di dalam blocks saja, variabel kita letakan di dalam bloks code.
